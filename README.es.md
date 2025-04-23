# redstar upscaler
Potente herramienta de escalado de vídeo que utiliza FFmpeg, Real-ESRGAN y Flowframes - ¡ahora soporta **UI multilingüe**!

🌐 Idioma:
[English](README.en.md) | [Korean](README.md) | [日本語](README.ja.md) | [中文](README.zh.md) |
Français](README.fr.md) | [Deutsch](README.de.md) | [Español](README.es.md) | [Português](README.pt.md) | [English](README.es.md)
[Русский](README.ru.md) | [Italiano](README.it.md) | [Tiếng Việt](README.vi.md) | [Bahasa Indonesia](README.id.md) | [Bahasa Indonesia](README.id.md) | [English](README.pt.md)
[ภาษาไทย](README.th.md) | [العربية](README.ar.md)

<p align="center">
  <img src="https://github.com/user-attachments/assets/632c3a83-5416-46c3-8d38-0e1bf153b633" height="250"/>
</p>

<p align="center">
  <strong>Herramienta de escalado de vídeo basada en fmpeg, realesrgan, flowframes</strong><br>
  <em>Moderno basado en GUI, ajustes preestablecidos, soporte para procesamiento de múltiples archivos</em>.
</p>

---.

Descarga: [Release](https://github.com/redstar-programmer/upscaler/releases/)

## ✨ Please support 'redstar' upscaler

¿Te gusta este proyecto o quieres apoyar su desarrollo?
¡Haga una pequeña donación para ayudarnos a construir mejores características y actualizaciones fiables!

- <img src="https://img.shields.io/badge/Donate-PayPal-blue.svg?logo=paypal" height="20"/><br>**PayPal** : [https://paypal.me/redstarprogrammer?country.x=KR&locale.x=ko_KR](https://paypal.me/redstarprogrammer?country.x=KR&locale.x=ko_KR)
- <img src="https://img.shields.io/badge/Sponsor-GitHub%20Sponsors-ff69b4?logo=githubsponsors" height="20"/><br>**Patrocinadores de GitHub** : [https://github.com/sponsors/redstar-programmer](https://github.com/sponsors/redstar-programmer)


> 💡 Su patrocinio de los costos del servidor, el tiempo de desarrollo, y una taza de café va un largo camino. Muchas gracias.

## Índice

- [👋 Introducción](#Introducción)
- 💾 Instalación y preparación](#Instalación-y-Preparación)
- 🔧 Características principales](#Características-Principales)
- Cómo utilizarlo (inicio rápido)](#How-to-use-quick-start)
- [⚙️ Descripción detallada de las características](#detailed-feature-description)
- 🙏 Agradecimientos](#Agradecimientos)
- 📜 Historia](#history)

## 👋 Introducción
**redstar upscaler es una herramienta GUI basada en Python para escalar automáticamente videos a resoluciones más altas usando `ffmpeg`, `Real-ESRGAN` y `Flowframes`.

- Extrae fotogramas de vídeo → escala → fusiona vídeo en un solo paso
- Soporta varios modelos real-ESRGAN
- Interpolación opcional a través de Flowframes
- Extracción y procesamiento automático de códecs de audio
- Trabaja en la ubicación de origen o en una ruta especificada

> ⚠️ Desarrollado y probado en un entorno Windows.

A continuación se muestra una sencilla demostración de uso:<br>
![미디어1](https://github.com/user-attachments/assets/ba601a08-6749-45fd-ae21-f1a2a52987f6)

## 💾 Instalación y preparación

1. instale y localice las siguientes herramientas externas (tenga en cuenta que el archivo de distribución incluye los instaladores de ffmpeg, Real-ESRGAN y Flowframes (consulte la carpeta Programas en la ruta))
   - [ffmpeg](https://www.ffmpeg.org/download.html)
   - Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN/releases)
   - Flowframes](https://github.com/n00mkrad/flowframes) *(opcional)*.
2. descomprimir y ejecutar upscaler.exe de readstar
3. en el caso de Flowframes, los modelos cargados pueden ser diferentes dependiendo de tu entorno, así que asegúrate de ejecutar Flowframes y de que la Interpolation AI y AI Model en la pestaña Interpolation coinciden con la versión de resources/flowframes_models.ini de redstar upscaler. <br>Comenta los modelos que no están cargados marcándolos con # y asegúrate de que el orden de los modelos en la ventana de ajustes de redstar upscaler coincide con el orden de los modelos en <br>Flowframes antes de continuar.

## 🔧 Características principales.

![Image](https://github.com/user-attachments/assets/072af636-e967-4e4b-b194-33b96f580780)
- ✅ Selección múltiple de vídeo y funcionamiento secuencial.
- ✅ Añadir vídeo de arrastrar y soltar
- ✅ Disponibilidad del programa principal y selección directa
- Modo de ahorro de disco
- ✅ Soporte multilingüe (15 idiomas)
<br><br>
![Image](https://github.com/user-attachments/assets/23dd7e8a-0e01-409f-b162-a9512fda09fc)
- Almacenamiento y aplicación automática de preajustes
- Detección automática de códecs de audio y ajuste de bitrate
- Detección y selección automática de modelos realesrgan
- ✅ Ajustes detallados para FFMPEG, real-ESRGAN y Flowframes
- ✅ Cambio de la configuración de opciones según la versión de Flowframes<br>(La versión se puede cambiar especificando la ruta de la versión en flowframes en la página principal)
<br><br>
![Image](https://github.com/user-attachments/assets/ab7d9410-1fb4-450b-92d5-56a6d583a64c)
- ✅ Comprobar el comando de ejecución upscale (se puede copiar y ejecutar por separado en CMD)
<br><br>
![Image](https://github.com/user-attachments/assets/4898904a-bb23-4dba-997d-23ca744fed93)
- Supervisar el progreso general de la operación de upscale
- ✅ Comprobar el registro de upscale (los archivos de registro se crean por fecha en la carpeta log de la carpeta live)
- Limpiar automáticamente los entregables tras la finalización del trabajo (con el prefijo [REDSTAR])
- ✅ Establecer acción tras la finalización de la tarea<br>(No hacer nada / Salir del programa / Modo de suspensión / Modo de hibernación / Cerrar ventana)
<br><br>
## 🚀 Cómo usar (Inicio rápido)

1. añadir archivos de vídeo (MP4, MKV, AVI, MOV, FLV, WMV, MPG, WEBM, 3GP, OGV compatibles)
2. especifique la ubicación de trabajo o marque la casilla "Usar ruta de archivo original
3. haz clic en el botón "Configuración" del vídeo añadido
4. Ajustes detallados de ffmpeg, realESRGAN, Flowframes
5. Haga clic en Aplicar por lotes a todos los archivos / Aplicar sólo a los archivos seleccionados
6. Haga clic en el botón "Confirmar
7. marque los comandos a ejecutar y haga clic en el botón Iniciar tarea

> ✨ El resultado del trabajo serán dos archivos: vídeo reescalado y vídeo interpolado por fotogramas en la carpeta seleccionada.
> ✨ Los archivos completados se guardarán con el prefijo [REDSTAR]
---]

## ⚙️ Descripción detallada de la función

| Elemento Descripción
|------|------|
| **Configurar ruta de trabajo** | Proporcionar ruta por defecto u opción "Usar ruta de archivo original
| **Soporta formatos de vídeo** | Soporta la mayoría de formatos, incluyendo MP4, MKV, AVI, MOV, FLV, WMV, MPG, WEBM, 3GP, OGV, etc.
| Detecta automáticamente realesr-animevideov3, realesr-general, 4xplus, etc.
| **Procesamiento de audio** | Soporte para codificar varios formatos como `aac`, `mp3`, `flac`, etc.
| **Integración de fotogramas de flujo** | Posibilidad de interpolación (FPS ×2, ×4, ×8)
| **Modo de ahorro de disco** | Eliminación automática de imágenes intermedias

## 🙏 Agradecimientos

- realrgan por [xinntao](https://github.com/xinntao/Real-ESRGAN)
- flowframes por [n00mkrad](https://github.com/n00mkrad/flowframes)
- Si quieres contribuir a este proyecto o sugerir alguna característica, por favor deja un comentario en [Issues](https://github.com/redstar-javscraper/redstar_upscaler/issues).

# Historia

v 1.1.0
 > 1. configuración del menú (abrir archivo, cerrar archivo, configuración de registro, configuración de idioma)
 > 2. añadidos ajustes multilingües (idiomas disponibles: coreano, inglés, 日本語, 中文, Français, Deutsch, Español, Português, Русский, Tiếng Việt, Bahasa Indonesia, ไทย, Italiano, العربية)
 > 3. Cambiados mensajes y algo de código para acomodar la configuración de idioma añadida.
 > 4. algunos cambios en la configuración de la interfaz de usuario
 > 5. ffmpeg, real-ESRGAN, Flowframes información de la versión mostrada (pantalla principal)
 > 6. Soporta la versión Flowframes 1.41.0 (actualmente sólo están disponibles las versiones 1.40.0, 1.36.0 debido a un problema con el comando cmd en la versión 1.41.0)
 > 7. Se ha corregido un problema por el que los elementos de AI Models se mostraban en minúsculas
 > 8. Añadidas opciones FFMPEG (píxeles, códec de vídeo) - las opciones se muestran en función del PC del usuario
 > 9. Mejorada la comprobación de CUDA para el PC de cada usuario - comprueba la disponibilidad y el tipo de GPU (pantalla principal)

v 1.0.0
 > 1. Reescritura completa del código
 > 2. Cambios en la interfaz de usuario
 > 3. Incrementado el rango de video/audio que puede ser procesado
 > 4. Añadido el modo de ahorro de disco
 > 5. Distribución que incluye los principales programas

v 0.1.92
 > 1. Se ha corregido un problema que provocaba el fallo de la interpolación debido a entradas duplicadas en el cuadro combinado del modelo AI al cambiar la ruta de Flowframes.
 > 2. Añadido un código de comprobación del estado de selección del cuadro combinado al interpolar.

v 0.1.91
 > 1. Añadidas algunas funciones de actualización del cuadro combinado relacionadas con Flowframes.
 > 2. Ajustados algunos archivos de distribución

v 0.1.9
 > 1. Aplicar cambios en el modelo Flowframes
 > 2. Nuevo modelo Flowframes 1.36.0, implementación del modelo 1.40.0
 > 3. Ya no se producen fallos en la línea de comandos de Flowframes
 > 4. Ahora se pueden añadir archivos arrastrando/soltando
 > 5. Corregidos los ajustes de Flowframes que no se aplicaban

v 0.1.8
 > 1. Corregido nuevo error de comprobación de versión al comprobar la versión
 > 2. Si flowframes está instalado en la ruta por defecto (ej. C:³³Administrador³AppData³Local³Flowframes³), establezca la ruta por defecto antes de iniciar.
 > 3. Al añadir múltiples selecciones de archivos, la aplicación se bloquea debido a un error.
 > 4. Corregido un error al iniciar la tarea después de añadir múltiples archivos.

v 0.1.7
 > 1. Se puede cambiar el tamaño del programa
 > 2. Corregido un error al trabajar con archivos sin voz
 > 3. Cambiada toda la configuración de la interfaz de usuario (reconfigurada para adaptarse al cambio de tamaño)

v 0.1.6
 > 1. Solucionado un problema con diferentes tamaños de fuente dependiendo de la resolución de pantalla
 > 2. Solucionado un problema por el que el título del programa no mostraba la información de la versión como una nueva versión
 > 3. Solucionado un problema por el que el archivo config.ini se guardaba en una ruta diferente
 > 4. Al cambiar el multiplicador de escalado de realrgan, también se cambia el cuadro combinado del modelo de escalado.
 > 5. Añadida la función de comprobación de actualización
 > 6. Corregida alguna lógica
 > 7. Cambiado el color de las tablas de resolución y fps
 > 8. Permitir al usuario editar la resolución (debe introducirse como 1024x768)

v 0.1.5
 > 1. Solucionado un problema por el que el modelo de IA no se cambiaba automáticamente al seleccionar la interpolación de IA FLOWFRAMES
 > 2. Solucionado un problema por el que la interpolación de flowframes no se interpolaba según la opción seleccionada
 > 3. Añadido el cuadro combinado "Método de cálculo de FPS" para evitar el cálculo incorrecto de FPS en algunos vídeos.
        -> r_frame_rate / avg_frame_rate, por defecto es r_frame_rate
 > 4. mostrar el progreso de obtención de información de vídeo al seleccionar un archivo de vídeo
 > 5. cambiar el valor por defecto para abrir la última carpeta seleccionada al seleccionar un archivo de nuevo después de abrir el archivo

v 0.1.4
 > 1. cambiado el modo de lectura del archivo config.ini
 > 2. cambiado el modo de obtener información de vídeo de Python AV a ffmpeg
 > 3. añadido el cierre de la ventana cuando la tarea ha finalizado
 > 4. Mostrar el nombre completo del archivo como tooltip al pasar el ratón por encima en la lista de tareas
 > 5. mostrar resolución(antes) / resolución(después) / FPS(antes) / FPS(después) para cada archivo en la lista de tareas
 > 6. eliminar el cuadro de entrada FPS (debido al etiquetado anterior para cada archivo)
 > 7. eliminar el tamaño estimado de FPS de salida (eliminado debido al etiquetado anterior para cada archivo)
 > 8. Mostrar el progreso como dos barras de progreso para todos los archivos/trabajos

v 0.1.3
 > 1. Corregido el error de cálculo de los FPS de los archivos donde alguna información de los FPS era errónea al cargar los archivos

v 0.1.2
 > 1. Cambios en la configuración de la interfaz de usuario
 > 2. cambios en la lógica interna
 > 3. Solucionado el problema por el que el modelo realrgan no se ejecutaba al seleccionar dos de los siguientes modelos
 > 4. cambiado la forma de utilizar los modelos realesrgan
 > -> Copie el nuevo archivo de modelo (*.param) en la carpeta de modelos de la carpeta de instalación de realesrgan y podrá utilizarlo.
 > 5. mostrar la información de anchura, altura y tamaño estimado del último archivo de la imagen de destino con el que se va a trabajar
 > 6. escribir el código para migrar el archivo config.ini
 > 7. cambiar la imagen de descomposición FFMPEG AAC -> FLAC
 > 8. otras correcciones de errores

v 0.1.1
 > 1. Escribir por primera vez, programa de escalado de video con ffmepg, realesrgan y flowframes