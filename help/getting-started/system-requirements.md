---
breadcrumb-title: ""
description: Revise los requisitos del sistema de Substance 3D Painter para asegurarse de que su equipo cumple las especificaciones de hardware y software.
title: Requisitos del sistema
user-guide-description: ""
user-guide-title: ""
source-git-commit: fbfe7e52b226b5a92f5b46ebbf82728f0ff9e3c5
workflow-type: tm+mt
source-wordcount: '814'
ht-degree: 1%
---

# Sistemas compatibles

A continuación se muestra una lista de hardware y sistemas compatibles con la aplicación:

## Windows

|  | Mínimo | Recomendado | Óptimo |
| --- | --- | --- | --- |
| **SO** | Windows 11 de 64 bits, versión 23H2 | Windows 11 Versión de 64 bits 24H1 | Windows 11 de 64 bits, versión 24H2 |
| **CPU** | Intel Core i5 AMD Ryzen 5 | Intel Core i7 AMD Ryzen 7 | Intel Core i9 AMD Ryzen 9 |
| **GPU** | NVIDIA GeForce RTX 2060 Super NVIDIA Quadro RTX 4000 AMD Radeon RX 5700 XT AMD Radeon Pro W5700 | NVIDIA GeForce RTX 3080 NVIDIA Quadro RTX A4000 AMD Radeon RX 6800 XT AMD Radeon Pro W7700 | NVIDIA GeForce RTX 4090 NVIDIA Quadro RTX 5000 Ada Generation AMD Radeon RX 7900 XTX AMD Radeon Pro W7800 |
| **VRAM** | 8 GB | 16 GB | 24 GB |
| **RAM** | 16 GB | 32 GB | 64 GB |
| **Almacenamiento** | SSD con 30 GB de espacio disponible | SSD con 50 GB de espacio disponible | SSD con 70 GB de espacio disponible |

### macOS

|  | Mínimo | Recomendado | Óptimo |
| --- | --- | --- | --- |
| **SO** | macOS 15 Sequoia | macOS 27 Golden gate | macOS 27 Golden Gate |
| **CPU** | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| **GPU** | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| **RAM** | 16 GB | 32 GB | 64 GB |
| **Almacenamiento** | SSD con 30 GB de espacio disponible | SSD con 50 GB de espacio disponible | SSD con 70 GB de espacio disponible |

>[!WARNING]
>
> Para las canalizaciones creadas teniendo en cuenta la [plataforma de referencia VFX](https://vfxplatform.com/), Substance 3D Painter se puede instalar en macOS 14 Sonoma. Sin embargo, Painter ya no se prueba en versiones de sistemas operativos que no cumplan los requisitos mínimos del sistema, por lo que no se garantiza su estabilidad.

### Linux

| Empresas | Vapor |
| --- | --- |
| RHEL 8<br>RHEL 9 | Ubuntu 22.04 |

## Recomendaciones generales

Para obtener un buen rendimiento al utilizar el flujo de trabajo de Mosaico de UV, recomendamos utilizar:

* 32 GB de RAM
* GPU con 8 GB de VRAM
* SSD para almacenar la caché del proyecto y de la aplicación.

Varios:

* Muchas aplicaciones de Substance dependen de OpenSSL 1.1.1 para la compatibilidad con RHEL8/9. En el caso de los sistemas con versiones más recientes de OpenSSL, el cliente deberá proporcionarlo manualmente
* Para trabajar en condiciones cómodas, recomendamos un monitor con una resolución vertical superior a 1000 píxeles y más ancho que 1280 píxeles.
* La exportación a **8K** (8192\*8192 píxeles) requiere una GPU con **más de** 2 GB de VRam.
* Solo se han notarizado las versiones 2019.x y superiores para poder ejecutarse en MacOS 10.15 (Catalina).
* Para usar el software mediante RDP (Escritorio remoto), consulte la [página de documentación](../pipeline-and-integration/configuration/remote-desktop.md) dedicada.
* El bloqueo de la CPU Ryzen al hacer un bake se puede corregir actualizando el BIOS.

## Configuraciones no compatibles

**Windows**

* No se admiten máquinas virtuales.
* Windows Server no es compatible.

**Mac**

* Solo se admiten configuraciones oficiales de Apple.
* Las eGPU no son compatibles actualmente y pueden presentar problemas de estabilidad.

**Linux**

* Los controladores Mesa en Linux no son compatibles.

**Cualquier plataforma**

* Las GPU integradas no son compatibles con las CPU x86-64 (Intel, AMD).

## Versiones mínimas del controlador de GPU

A continuación se muestra una lista de las versiones mínimas del controlador de la GPU necesarias para que la aplicación se ejecute sin problemas. Esta lista está sujeta a cambios a medida que se lancen nuevas versiones.

Para descargar nuevos controladores, consulte: [La GPU tiene controladores obsoletos](../technical-support/technical-issues/gpu-issues/gpu-has-outdated-drivers.md).

| SO | NVIDIA | AMD | Intel |
| --- | --- | --- | --- |
| **Windows** | GeForce 442.50 Quadro 442.50 | Radeon 19.7.1 Radeon Pro / FirePro 18.Q4 | 15.33 |
| **Linux** | 535.171.04 o posterior | Radeon 22.40.6 | No admitido |

>[!NOTE]
>
> En **Mac OS**, el controlador de la GPU lo proporciona el propio sistema operativo. Actualice a la versión más reciente del sistema operativo para acceder al controlador más reciente.

### Problemas de compatibilidad de controladores

Para obtener una lista detallada de los problemas de controladores de GPU por constructor, consulte la [página de documentación dedicada](../technical-support/technical-issues/gpu-issues/gpu-drivers-compatibility.md).

## Trazado de rayos de GPU para hacer un bake

Para habilitar el Trazado de rayos de GPU a través de Optix o DXR se deben instalar los controladores mínimos recomendados anteriormente.

**DXR** también requiere la siguiente configuración mínima:

* **Windows 10** versión 1809, consulte [esta página](https://experienceleague.adobe.com/es/docs/substance-3d/bakers/features/gpu-raytracing) para obtener más información
* **GPU con arquitectura Pascal** (NVIDIA GeForce 10XX)

>[!TIP]
>
> El trazado de rayos de GPU se ejecuta de forma óptima en hardware de trazado de rayos dedicado, como las GPU NVIDIA GeForce RTX o NVIDIA Quadro RTX.

## Tabletas gráficas compatibles

A continuación se muestra una lista de tabletas gráficas compatibles que se han probado con la versión **7.4.2** de Substance 3D Painter:

+++Wacom

**Modelos:** Intuos Pro (tamaño M), Intuos (tamaño S)

| SO | Versión del controlador |
| --- | --- |
| Windows | 6.3.45-1 |
| macOS | 6.3.45-3 |

+++

+++XPen

**Modelo:** Deco 01

| SO | Versión del controlador |
| --- | --- |
| Windows | XP-PENWin_3.2.2.211027 |
| macOS | XP-PENMac_3.2.3_211203 |
| Linux | XP-PEN-pentablet-3.2.1.211019-1 |

+++

+++Huion

**Modelo:** Q11K

| SO | Versión del controlador |
| --- | --- |
| Windows | XP-PENWin_3.2.2.211027 |
| macOS | XP-PENMac_3.2.3_211203 |

+++

+++Xencelabs

**Modelo:** Pluma - Tableta Media

| SO | Versión del controlador |
| --- | --- |
| Windows | XencelabsWin_1.2.1-14 |
| macOS | XencelabsMac_1.2.1-18 |
| Linux | XencelabsLinux_1.1.0-2 |

+++

## Modelos de SpaceMouse de conexión 3D compatibles

A continuación se muestra una lista de versiones de controlador compatibles para el [Ratón espacial de conexión 3D](https://3dconnection.com/us/spacemouse/) que se han probado con la versión **8.1.** de Substance 3D Painter

Las versiones de controlador se aplican a los modelos **Compact**, **Pro** y **Enterprise**.

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
