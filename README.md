# Creacion de Api Rest
Se cominza posterior a la intalzacion de las heramientas con la inizalizacion de npm

>npm init -y

esto crea el package.json

posteriormente se instala las dependencias nesesarias 

>npm i express mongoose

Se crea la carpeta donde que contendra los archivos de codigo para separlos de los archivos de configuracion, a esta carpeta la nombramos src y dentro de esta creamos una carpeta llamada routes 

./src/index.js:
    Contendra la configuracion nesesaria para correr el api

./src/database.js
    Contendra la configuracion neseasria para la conexion a la base de datos

./src/routes/index.routes.js
    Utilizara la dependencia express, contendra los metodos  de optencion de datos 


Posteriormente creamos los archivos para crear los contenedores en docker
- .dockerignore: 
    Este nos ayuda que que no se copie carpets como node_modules dentro del contenedor ya que seria inesesario dentro del contenedor
- Dockerfile:
    Este documento nos ayuda a la creacion de un contenedor con los archivos nesesarios para qeu corra el api
- docker-compose.yml:
    Este nos ayudara a la configuracion del contenedor y a  "orquestar" la base de datos.

Se corren los conteiners y se logra optener el mensage de conexion con la base de datos por medio del navegador.