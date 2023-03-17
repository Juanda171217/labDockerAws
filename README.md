# TALLER DE DE MODULARIZACIÓN CON VIRTUALIZACIÓN E INTRODUCCIÓN A DOCKER Y A AWS

## Juan David Martinez


### Descripción

Este taller consiste en la creación de una aplicación web que por medio de LogService que es un servicio REST recibe una cadena, la almacena en la base de datos y responde con las 10 ultimas cadenas almacenadas y la fecha en la que se almacenaron. Utilizando el framework Spark y desplegada en un contenedor Docker. La aplicación web se desplegará en una instancia EC2 de AWS.


### Pre-requisitos

* Java
* Maven
* Docker
* En caso de desplegarlo en AWS se necesita una cuenta de AWS y crear una instancia EC2.
  
### Compilación y ejecución

Primero debe acceder a las carpetas logService y roundRobin y ejecutar el comando 

```
mvn package
```
en cada una.


Luego para compilar el proyecto se debe ejecutar el siguiente comando:

```
docker-compose up -d --build
```

luego desde su navegador ingrese a la siguiente ruta http://localhost:35000

### Prueba

[![lr.png](https://i.postimg.cc/wxrnQtkm/lr.png)](https://postimg.cc/qg8mkvSJ)


### Estructura de archivos

[![awsE.png](https://i.postimg.cc/GmbjQsnW/awsE.png)](https://postimg.cc/PPFZfJxy)

[![awse2.png](https://i.postimg.cc/5NDVQbcQ/awse2.png)](https://postimg.cc/xcG7Wr19)





