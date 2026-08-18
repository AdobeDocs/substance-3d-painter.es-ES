---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/getting-started/system-requirements.html"
breadcrumb-title: ''
description: Revise los requisitos del sistema de Substance 3D Painter para asegurarse de que su equipo cumple las especificaciones de hardware y software.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > System requirements
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Requisitos del sistema
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 1%

---


# Sistemas compatibles

A continuación se muestra una lista de hardware y sistemas compatibles con la aplicación:

## Windows

|  | Mínimo | Recomendado | Óptimo |
| --- | --- | --- | --- |
| <b>SO</b> | Windows 11 de 64 bits, versión 23H2 | Windows 11 Versión de 64 bits 24H1 | Windows 11 de 64 bits, versión 24H2 |
| <b>CPU</b> | Intel Core i5 AMD Ryzen 5 | Intel Core i7 AMD Ryzen 7 | Intel Core i9 AMD Ryzen 9 |
| <b>GPU</b> | NVIDIA GeForce RTX 2060 Super NVIDIA Quadro RTX 4000 AMD Radeon RX 5700 XT AMD Radeon Pro W5700 | NVIDIA GeForce RTX 3080 NVIDIA Quadro RTX A4000 AMD Radeon RX 6800 XT AMD Radeon Pro W7700 | NVIDIA GeForce RTX 4090 NVIDIA Quadro RTX 5000 Ada Generation AMD Radeon RX 7900 XTX AMD Radeon Pro W7800 |
| <b>VRAM</b> | 8 GB | 16 GB | 24 GB |
| <b>RAM</b> | 16 GB | 32 GB | 64 GB |
| <b>Almacenamiento</b> | SSD con 30 GB de espacio disponible | SSD con 50 GB de espacio disponible | SSD con 70 GB de espacio disponible |

### macos

|  | Mínimo | Recomendado | Óptimo |
| --- | --- | --- | --- |
| <b>SO</b> | macOS 12 Monterey | macOS 13 Ventura | macOS 14 Sonoma |
| <b>CPU</b> | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| <b>GPU</b> | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| <b>RAM</b> | 16 GB | 32 GB | 64 GB |
| <b>Almacenamiento</b> | SSD con 30 GB de espacio disponible | SSD con 50 GB de espacio disponible | SSD con 70 GB de espacio disponible |

### Linux

| Empresas | Vapor |
| --- | --- |
| RHEL 8</br>RHEL 9 | Ubuntu 22.04 |

## Recomendaciones generales

Para obtener un buen rendimiento al utilizar el flujo de trabajo de azulejo UV, recomendamos utilizar:

* 32 GB de RAM
* GPU con 8 GB de VRAM
* SSD para almacenar la caché del proyecto y de la aplicación.

Varios:

* Muchas aplicaciones de Substance dependen de OpenSSL 1.1.1 para la compatibilidad con RHEL8/9. En el caso de los sistemas con versiones más recientes de OpenSSL, el cliente deberá proporcionarlo manualmente
* Para trabajar en condiciones cómodas, recomendamos un monitor con una resolución vertical superior a 1000 píxeles y más ancho que 1280 píxeles.
* La exportación a <b>8K</b> (8192\*8192 píxeles) requiere una GPU con <b>más de</b> 2 GB de VRam.
* Solo se han notarizado las versiones 2019.x y superiores para poder ejecutarse en MacOS 10.15 (Catalina).
* Para usar el software mediante RDP (Escritorio remoto), consulte la [página de documentación](../pipeline-and-integration/configuration/remote-desktop.md) dedicada.
* Bloqueo en la CPU Ryzen durante el procesamiento, se puede solucionar mediante la actualización del BIOS.

## Configuraciones no compatibles

<b>Windows</b>

* No se admiten máquinas virtuales.
* Windows Server no es compatible.

<b>Mac</b>

* Solo se admiten configuraciones oficiales de Apple.
* Las eGPU no son compatibles actualmente y pueden presentar problemas de estabilidad.

<b>Linux</b>

* Los controladores Mesa en Linux no son compatibles.

<b>Cualquier plataforma</b>

* Las GPU integradas no son compatibles con las CPU x86-64 (Intel, AMD).

## Versiones mínimas del controlador de GPU

A continuación se muestra una lista de las versiones mínimas del controlador de la GPU necesarias para que la aplicación se ejecute sin problemas. Esta lista está sujeta a cambios a medida que se lancen nuevas versiones.

Para descargar nuevos controladores, consulte: [La GPU tiene controladores obsoletos](../technical-support/technical-issues/gpu-issues/gpu-has-outdated-drivers.md).

| SO | NVIDIA | AMD | Intel |
| --- | --- | --- | --- |
| <b>Windows</b> | GeForce 442.50 Quadro 442.50 | Radeon 19.7.1 Radeon Pro / FirePro 18.Q4 | 15.33 |
| <b>Linux</b> | 535.171.04 o posterior | Radeon 22.40.6 | No admitido |

>[!NOTE]
>
> En **Mac OS**, el controlador de la GPU lo proporciona el propio sistema operativo. Actualice a la versión más reciente del sistema operativo para acceder al controlador más reciente.

### Problemas de compatibilidad de controladores

Para obtener una lista detallada de los problemas de controladores de GPU por constructor, consulte la [página de documentación dedicada](../technical-support/technical-issues/gpu-issues/gpu-drivers-compatibility.md).

## Trazado de rayos de GPU para hornear

Para habilitar el Trazado de rayos de GPU a través de Optix o DXR, deben instalarse los controladores mínimos recomendados anteriormente.

<b>DXR</b> también requiere la siguiente configuración mínima:

* <b>Windows 10</b> versión 1809, consulte [esta página](https://experienceleague.adobe.com/en/docs/substance-3d/bakers/features/gpu-raytracing) para obtener más información
* GPU <b> con arquitectura Pascal</b> (NVIDIA GeForce 10XX)

>[!TIP]
>
> Trazado de rayos de GPU funciona de forma óptima con hardware de trazado de rayos como las GPU NVIDIA GeForce RTX o NVIDIA Quadro RTX.

## Tabletas gráficas compatibles

A continuación se muestra una lista de tabletas gráficas compatibles que se han probado con la versión <b>7.4.2</b> de Substance 3D Painter:

+++Wacom
<b>Modelos:</b> Intuos Pro (tamaño M), Intuos (tamaño S)


| SO | Versión del controlador |
| --- | --- |
| Windows | 6.3.45-1 |
| macOS | 6.3.45-3 |


+++

+++XPen
<b>Modelo:</b> Deco 01


| SO | Versión del controlador |
| --- | --- |
| Windows | XP-PENWin\_3.2.2.211027 |
| macOS | XP-PENMac\_3.2.3\_211203 |
| Linux | XP-PEN-pentablet-3.2.1.211019-1 |


+++

+++Huion
<b>Modelo:</b> Q11K


| SO | Versión del controlador |
| --- | --- |
| Windows | XP-PENWin\_3.2.2.211027 |
| macOS | XP-PENMac\_3.2.3\_211203 |


+++

+++Xencelabs
<b>Modelo:</b> Pluma - Tableta Media


| SO | Versión del controlador |
| --- | --- |
| Windows | XencelabsWin\_1.2.1-14 |
| macOS | XencelabsMac\_1.2.1-18 |
| Linux | XencelabsLinux\_1.1.0-2 |


+++

## Modelos de SpaceMouse de conexión 3D compatibles

A continuación se muestra una lista de versiones de controlador compatibles para el [Ratón espacial de conexión 3D](https://3dconnection.com/us/spacemouse/) que se han probado con la versión <b>8.1.</b> de Substance 3D Painter

Las versiones de controlador se aplican a los modelos <b>Compact</b>, <b>Pro</b> y <b>Enterprise</b>.

| SO | Versión del controlador |
| --- | --- |
| Windows | 10.8.6.3431 |
| macOS | 10.7.2.3454 |

## Idiomas

La interfaz de software está disponible en los siguientes idiomas:

* Inglés (Estados Unidos)
* Alemán
* Español
* francés
* Italiano
* Japanese
* Coreano
* Portugués (Brasil)
* Chino (simplificado)
