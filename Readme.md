# Libertad GPT

![Licencia de GitHub](https://img.shields.io/badge/license-GNU-blue.svg)

![Lanzamiento de GitHub](https://img.shields.io/github/release/ohmplatform/freedom-gpt-electron-app.svg)

![Estrellas de GitHub](https://img.shields.io/github/stars/ohmplatform/freedom-gpt-electron-app.svg)

![GitHub All Releases](https://img.shields.io/github/downloads/ohmplatform/freedom-gpt-electron-app/total.svg)Esta base de código es para una aplicación basada en React y Electron que ejecuta FreedomGPT LLM localmente (sin conexión y privada) en Mac y Windows utilizando una interfaz basada en chat (basada en Alpaca Lora)


## Introducción

Este es el repositorio de la aplicación Freedom GPT. Esta aplicación está construida usando
[Electrón](https://www.electronjs.org/) y [React](https://reactjs.org/). Es una aplicación de escritorio que
permite a los usuarios ejecutar modelos de alpaca en su máquina local.

## Requisitos previos

- [Node.js](https://nodejs.org/en/download/)
- [Hilo](https://classic.yarnpkg.com/en/docs/install/#windows-stable)
-[Git](https://git-scm.com/downloads)

# Si quieres contribuir al proyecto

## Trabajando con el repositorio

```sh
git clone --recursivo https://github.com/ohmplatform/FreedomGPT.git freedom-gpt
cd libertad-gpt
instalación de hilo
```

# Construyendo la biblioteca llama.cpp

## Construyendo desde el código fuente (MacOS/Linux)

```sh
cd llama.cpp
hacer
```

## Construyendo desde la fuente (Windows)

- Descargue e instale CMake: <https://cmake.org/download/>
- Ejecute los siguientes comandos uno por uno:

```ps1
cd llama.cpp
cmake.
cmake-build. --config Lanzamiento
```

- Ahora deberías tener una carpeta `Release` con un archivo `main.exe` dentro. Puede ejecutar este archivo para probar el cliente de chat.

## Cambiando la URL de la API

Estamos usando `http://localhost:8889` como URL de API, puede cambiarlo en el archivo
`src/index.ts`

## Ejecutando la aplicación

Para ejecutar la aplicación, ejecute el siguiente comando en su terminal:

```sh
inicio del hilo

⦻ Asegúrese de estar en el directorio raíz del proyecto.
```

## Dockerizando la aplicación

Para ejecutar la imagen de la ventana acoplable, ejecute el siguiente comando en su terminal:

```sh
ventana acoplable tire freedomgpt/freedomgpt
ventana acoplable ejecutar -d -p 8889:8889 freedomgpt/freedomgpt
```

Si desea crear la imagen de la ventana acoplable usted mismo, ejecute el siguiente comando en su terminal:

```sh
ventana acoplable build -t freedomgpt/freedomgpt.

O

estibador de hilo
```

<!-- ## Vídeo de trabajo

https://user-images.githubusercontent.com/54356944/233825525-d95accf3-a26b-4f37-8fc1-6e922f782a66.mov -->

# Créditos

Este proyecto utiliza varios paquetes y bibliotecas de código abierto, sin los cuales este proyecto no habría sido posible:

"llama.cpp" - Biblioteca C++. https://github.com/ggerganov/llama.cpp

"LLAMA" de Facebook Research: un algoritmo de búsqueda de vecino más cercano aproximado a gran escala y de baja latencia. https://github.com/facebookresearch/llama

"Interfaz de usuario de Chatbot" - https://github.com/mckaywrigley/chatbot-ui

Nos gustaría expresar nuestro agradecimiento a los desarrolladores de estos paquetes y a sus colaboradores por poner su trabajo a disposición del público bajo licencias de código abierto. Sus contribuciones nos han permitido construir un proyecto más sólido y eficiente.

# LICENCIA

Consulte el archivo <a href="/LICENSE"> LICENCIA </a>.
