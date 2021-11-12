# ContenedoresTelematica

## Paso a paso para visualizar pagina de noticias:
1. Se debe clonar este repositorio, para ello se necesita la consola de git bash, se escribe el siguiente codigo:
  * "git clone https://github.com/JulianG91012/ContenedoresTelematica.git"
2. Se abre la carpeta clonada en su dispositivo, para poder copiar facilmente la ruta donde se encuentra.
3. Se abre una consola con permisos de administrador (Puede ser cmd, powershell, etc), lo importante es que acceda a la carpeta donde está descargado el repositorio
   Hay dos opciones para esto:
   * Se abre la consola directamente en la carpeta, usando el click derecho -> abrir terminal.
   * Se abre la consola y se escribe: "cd + [ruta para llegar a la carpeta]"
4. Se usa el comando "docker build .", este comando es para ejecutar el archivo DockerFile que se encuentre en la carpeta
5. Se necesita saber el ID de la iagen de contenedor creado para el siguiente paso, así que en la misma terminal donde se creó, se escrib: "docker images"
6. Teniendo en cuenta los primeros 4 caracteres de la ultima imagen creada vamos a escribir el siguiente codigo:
   * "docker run -d -p 80:80 [ID de la ultima imagen] apache ctl -D FOREGROUND"
7. Cuando este proceso finalice, vamos a nuestro navegador y escribimos "localhost" o la IP de nuestro navegador, con esto nos mostraría la pagina web creada.
