---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/scripting-and-development/scripts-and-plugins/remote-control-with-scripting.html"
breadcrumb-title: ''
description: Aprenda a utilizar las secuencias de comandos de control remoto en Substance 3D Painter para automatizar flujos de trabajo y controlar la aplicación mediante programación.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > Scripts and plugins > Remote control with scripting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Control remoto con secuencias de comandos
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---


# Control remoto con secuencias de comandos

Esta página describe cómo controlar la aplicación de forma remota para ejecutar comandos de JavaScript o Python.\
Esto requiere un argumento de línea de comandos específico, luego una simple secuencia de comandos de Python puede ejecutar cualquier comando disponible de las API de Javascript y Python existentes.

## Inicio de la aplicación

Para controlar de forma remota la aplicación, Substance 3D Painter debe iniciarse con la siguiente línea de comandos:

```
"Adobe Substance 3D painter.exe" --enable-remote-scripting
```


>[!NOTE]
>
> Asegúrese de que la aplicación esté en funcionamiento con este comando antes de ejecutar cualquier script. Las secuencias de comandos pueden fallar si la aplicación aún se está iniciando o no está lista.

## Script de control remoto

La siguiente secuencia de comandos de Python puede servir como biblioteca para comunicarse con la aplicación.

Guarde el siguiente script en un archivo denominado **lib\_remote.py** para que los ejemplos siguientes funcionen correctamente.

```
import sys 

import json 

import base64 

import subprocess 

 

if sys.version_info >= (3, 0): 

 import http.client as http 

else: 

 import httplib as http 

 

class RemotePainter() : 

 def __init__(self, port=60041, host='localhost'): 

  self._host = host 

  self._port = port 

 

## Json server connection

  self._PAINTER_ROUTE = '/run.json' 

  self._HEADERS = {'Content-type': 'application/json', 'Accept': 'application/json'} 

 

## Execute a HTTP POST request to the Substance Painter server and send/receive JSON data

 def _jsonPostRequest( self, route, body, type ) : 

  connection = http.HTTPConnection(self._host, self._port, timeout=3600) 

  connection.request('POST', route, body, self._HEADERS) 

  response = connection.getresponse() 

 

  data = response.read() 

  connection.close() 

 

  if type == "js" : 

   data = json.loads( data.decode('utf-8') ) 

 

   if 'error' in data: 

    OutJson = json.loads( body.decode() ) 

    print( base64.b64decode( OutJson["js"] ) ) 

    raise ExecuteScriptError(data['error']) 

  else : 

## Python can return nothing, so decoding can fail

   try: 

    data = data.decode('utf-8').rstrip() 

   except: 

    pass 

 

  return data 

 

 def checkConnection(self): 

  connection = http.HTTPConnection(self._host, self._port) 

  connection.connect() 

 

## Execute a command

 def execScript( self, script, type ) : 

  Command = base64.b64encode( script.encode('utf-8') ) 

 

  if type == "js" : 

   Command = '{{"js":"{0}"}}'.format( Command.decode('utf-8') ) 

  else : 

   Command = '{{"python":"{0}"}}'.format( Command.decode('utf-8') ) 

 

  Command = Command.encode( "utf-8" ) 

 

  return self._jsonPostRequest( self._PAINTER_ROUTE, Command, type ) 

 

class PainterError(Exception): 

 def __init__(self, message): 

  super(PainterError, self).__init__(message) 

 

class ExecuteScriptError(PainterError): 

 def __init__(self, data): 

  super(PainterError, self).__init__('An error occured when executing script: {0}'.format(data)) 

 
```


## Ejemplos

A continuación se muestran dos ejemplos sencillos que muestran cómo ejecutar comandos en ambas API admitidas por la aplicación:

### Ejecución de comandos de Javascript

La mayoría de las funciones de Javascript en la API devuelven datos de String o Json que facilitan su manipulación dentro de la secuencia de comandos de Python. No debería haber ningún problema importante para enviar y recibir datos.

Cree un archivo de script python denominado **example\_js.py** y agregue el código siguiente:

```
import lib_remote 

 

Remote = lib_remote.RemotePainter() 

Remote.checkConnection() 

 

## Print the API version

Version = Remote.execScript( "alg.version.painter", "js" ) 

print( Version ) 

 

## Get a list of all the files in the default shelf/library:

Files = Remote.execScript( 'alg.resources.findResources("starter_assets", "*")', "js" ) 

 

for File in Files : 

 print( File )
```


Si la aplicación se ejecuta con la línea de comandos, al ejecutar esta secuencia de comandos, se ejecutarán comandos y se recuperarán sus resultados.

### Ejecución de comandos de Python

La mayoría de las funciones de Python pueden devolver objetos que no se pueden pasar a la secuencia de comandos remota, lo que significa que, para recibir datos, deben convertirse explícitamente en cadenas o diccionarios Json.

Para facilitar las cosas, es posible crear script python personalizado que se carga durante el inicio de la aplicación y llamar a funciones que manejan este tipo de conversión sin tener que confiar en conversiones en línea.

Cree un archivo de script python denominado **example\_py.py** y agregue el código siguiente:

```
import lib_remote 

 

Remote = lib_remote.RemotePainter() 

Remote.checkConnection() 

 

## import the substance_painter module to make

## its API available to us

Remote.execScript( "import substance_painter", "python" ) 

 

## Print the API version

Version = Remote.execScript( "substance_painter.__version__", "python" ) 

print( Version ) 

 

## Get a list of all the files in the default shelf/library

## Because the search function return objects, we have to convert

## the information into a string within the same command (inline)

Command = 'substance_painter.resource.search( "p:starter_assets/" )' 

Command = '"|||".join( [ x.identifier().url() for x in {0}] )'.format( Command ) 

 

Files = Remote.execScript( Command, "python" ) 

Files = Files.split( "|||" ) 

 

for File in Files : 

 print( File )
```


Si la aplicación se ejecuta con la línea de comandos, al ejecutar esta secuencia de comandos, se ejecutarán comandos y se recuperarán sus resultados.
