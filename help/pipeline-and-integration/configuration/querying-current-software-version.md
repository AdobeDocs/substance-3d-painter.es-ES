---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/configuration/querying-current-software-version.html"
breadcrumb-title: ''
description: Aprenda a consultar la versión actual del software de Substance 3D Painter mediante programación para la integración y automatización de la canalización.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Configuration > Querying Current Software Version
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Consultar la versión actual del software
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---


# Consultar la versión actual del software

La comprobación de la versión actual de la aplicación se puede realizar de varias maneras según las necesidades (sin necesidad de iniciar el software, por ejemplo).

## Comprobando la versión a través del ejecutable

El ejecutable de Substance Painter en Windows contiene poca información que puedan consultar las herramientas externas (como Python).

Ejemplo de **Python 3** ([tomada de aquí](https://stackoverflow.com/questions/580924/python-windows-file-version-attribute)) :

```
import os 

import imp 

import pip 

import win32api #pypiwin32 

 

 


## Reader


def getFileProperties(fname): 

 """ 

 Read all properties of the given file return them as a dictionary. 

 """ 

 propNames = ('Comments', 'InternalName', 'ProductName', 

  'CompanyName', 'LegalCopyright', 'ProductVersion', 

  'FileDescription', 'LegalTrademarks', 'PrivateBuild', 

  'FileVersion', 'OriginalFilename', 'SpecialBuild') 

 

 props = {'FixedFileInfo': None, 'StringFileInfo': None, 'FileVersion': None} 

 

 try: 

## backslash as parm returns dictionary of numeric info corresponding to VS_FIXEDFILEINFO struc

  fixedInfo = win32api.GetFileVersionInfo(fname, '\') 

  props['FixedFileInfo'] = fixedInfo 

  props['FileVersion'] = "%d.%d.%d.%d" % (fixedInfo['FileVersionMS'] / 65536, 

   fixedInfo['FileVersionMS'] % 65536, fixedInfo['FileVersionLS'] / 65536, 

   fixedInfo['FileVersionLS'] % 65536) 

 

## VarFileInfoTranslation returns list of available (language, codepage)

## pairs that can be used to retreive string info. We are using only the first pair.

  lang, codepage = win32api.GetFileVersionInfo(fname, '\VarFileInfo\Translation')[0] 

 

## any other must be of the form StringfileInfo%04X%04Xparm_name, middle

## two are language/codepage pair returned from above

 

  strInfo = {} 

  for propName in propNames: 

   strInfoPath = u'\StringFileInfo\%04X%04X\%s' % (lang, codepage, propName) 

   ## print str_info 

   strInfo[propName] = win32api.GetFileVersionInfo(fname, strInfoPath) 

    

  props['StringFileInfo'] = strInfo 

 except: 

  pass 

 

 return props 

 

 


## Check exe


Path = "E:/Software/Painter/Substance Painter.exe" 

 

FileInfo = getFileProperties(Path) 

 

print( FileInfo )
```


Se generará :

```
E:SoftwarePainter>query.py 

{'FixedFileInfo': {'Signature': -17890115, 'StrucVersion': 65536, 'FileVersionMS': 132251649, 'FileVersionLS': 65536, 'ProductVersionMS': 132251649, 'ProductVersionLS': 65536, 'FileFlagsMask': 0, 'FileFlags': 0, 'FileOS': 0, 'FileType': 1, 'FileSubtype': 0, 'FileDate': None}, 'StringFileInfo': {'Comments': None, 'InternalName': 'Substance Painter', 'ProductName': 'Substance Painter', 'CompanyName': 'Allegorithmic', 'LegalCopyright': 'Copyright (C) 2017 Allegorithmic', 'ProductVersion': '2018.1.1', 'FileDescription': 'Substance Painter 2018.1.1', 'LegalTrademarks': None, 'PrivateBuild': None, 'FileVersion': '2018.1.1', 'OriginalFilename': 'Substance Painter.exe', 'SpecialBuild': None}, 'FileVersion': '2018.1.1.0'}
```


Comprobar la versión mediante la línea de comandos

Puede usar la línea de comandos de la siguiente manera: **substance painter.exe** command\_name *[option]*

Para preguntar a la versión, use **—version**, **-v**.

>[!NOTE]
>
> Tenga en cuenta que las acciones de línea de comandos de Substance Painter generarán una ventana de salida.

## Comprobación de versiones mediante scripts

La API de scripts (disponible a través del menú de ayuda) permite consultar la versión actual de la aplicación.

Consulte el espacio de nombres &quot;**alg**&quot; para obtener más detalles.

Ejemplo :

```
//Print current version in the log window (string) 

alg.log.info( alg.version.painter );
```
