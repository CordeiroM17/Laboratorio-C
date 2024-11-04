# Laberinto del Desafío (Nombre del juego)

Este proyecto es un videojuego en lenguaje C desarrollado para la materia Algoritmos y Estructuras de Datos. El objetivo del juego es guiar a un personaje a través de un laberinto aleatorio, evitando trampas y recolectando llaves para llegar a la salida antes de que se acabe el tiempo.

## Instalación

1. **Instalar el compilador GCC**  
   Si aún no tienes GCC, puedes instalarlo ejecutando el siguiente comando en tu terminal:

   - [Instalación de MinGW para compilar en C](https://www.youtube.com/watch?v=GEZLjRSY_m8).
   - [MinGW - Minimalist GNU for Windows](https://sourceforge.net/projects/mingw/).

2. **Configurar GCC**

   Abrir la seccion de terminal dentro de visual studio code y deleccionar la opcion `Configure Tasks...`

   Elegir la opcion de MinGW si es que se tienen otros compiladores.

   ![](/img_readme/c_terminal.png)

   Esto creara un archivo tasks.json en la carpeta `.vscode`.

   Dentro de este archivo colocar la siguiente configuracion

   ```js
   {
      "version": "2.0.0",
      "tasks": [
         {
            "type": "shell",
            "label": "C/C++: gcc.exe build active file",
            "command": "C:\\MinGW\\bin\\gcc.exe",
            "args": [
            "-fdiagnostics-color=always",
            "-g",
            "${file}",
            "-o",
            "${fileDirname}\\${fileBasenameNoExtension}.exe"
            ],
            "options": {
            "cwd": "${workspaceFolder}"
            },
            "problemMatcher": ["$gcc"],
            "group": "build"
         }
      ]
   }
   ```

   Instalar las siguientes extensiones en visual studio code.

   ![](/img_readme/c_ext1.png)

   ![](/img_readme/c_ext2.png)

3. **Clonar el Repositorio**  
   Clona este repositorio en tu máquina local:
   ```bash
   git clone [URL del repositorio]
   cd Laberinto-del-Desafio
   ```

## Compilación y Ejecución

1. **Compilar el Proyecto**  
   En el directorio del proyecto, compila el juego con el siguiente comando:

   ```bash
   gcc -o laberinto laberinto.c -Wall
   ```

2. **Ejecutar el Juego**  
   Una vez compilado, puedes iniciar el juego ejecutando:
   ```bash
   ./laberinto
   ```

## Contribuciones y Créditos

Este proyecto fue desarrollado por [Tu Nombre] y equipo como parte del curso de Algoritmos y Estructuras de Datos.
