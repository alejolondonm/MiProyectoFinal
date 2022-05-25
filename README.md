# Mi Proyecto Final
### Tema Del Proyecto
Mi Proyecto Final es un portal WiKi sobre mi artista favorita (Taylor Swift), que incluye con algunos datos generales de su vida y carrera artística, su discografía y su impacto en la industria musical.

## ¿Qué comandos se deben de ejecutar para el correcto uso del script?
###### Convierte el archivo ejecutable
```
sudo chmod u+x Alejo_Script.sh
```
###### Ejecuta el script
```
sudo ./Alejo_Script.sh
```

## Comandos que ejecuta Script "Alejo_Script.sh"

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

###### Crea el contenedor y lo enciende.
`docker run -d -p 80:80 mipagina:v1 apachectl -D FOREGROUND`
