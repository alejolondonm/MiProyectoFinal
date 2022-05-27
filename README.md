# Mi Proyecto Final :dvd:
### Tema Del Proyecto :minidisc: 
Mi Proyecto Final es un portal WiKi sobre mi artista favorita (Taylor Swift), :woman_singer: que incluye algunos datos generales de su vida y carrera artística, su discografía y su impacto en la industria musical.

## ¿Qué comandos se deben de ejecutar para el correcto uso del script? :musical_keyboard:
###### Convierte el archivo ejecutable
```
sudo chmod u+x Alejo_Script.sh
```
###### Ejecuta el script
```
sudo ./Alejo_Script.sh
```

## Comandos que ejecuta el script (Alejo_Script.sh) :banjo:

###### Actualiza los paquetes. 
`apt update`

###### Instala Docker, para poder crear el contenedor.
`apt install docker-compose -y`

###### Insata Git, para poder manejar repositorios de git.
`apt install git-core -y`

###### Se translada de ubicación al home.
`cd /home/`

###### Clona todos los archivos y carpetas del repositorio que responde a esa URL.
`git clone https://github.com/alejolondonm/MiProyectoFinal.git`

###### Construye la imagen, como plantilla para crear el contenedor.
`docker build -t mipagina:v1 MiProyectoFinal/`

###### Crea el contenedor, lo enciende y lo asigna al puerto 80.
`docker run -d -p 80:80 mipagina:v1 apachectl -D FOREGROUND`

## Contenido Del Repositorio :guitar:
#### 1. Carpeta MiPaginaWeb: Contiene el archivo index.html, junto de recursos e imagenes que utiliza la página web. 
###### Cabe resaltar que la página web es una edición de una plantilla encontrada en internet, por ende no es de mi propiedad; yo solo la edité a mi gusto, para el proyecto final de telemática, con fines educativos.
#### 2. Dockerfile: Archivo que contiene todos los comandos que se van a ejecutar para crear una imagen.
#### 3. ReadMe: Archivo que contiene las instrucciones para ejecutar efectivamente el script y el contenido del repositorio.
