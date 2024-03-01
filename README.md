# TALLER DE DE MODULARIZACIÓN CON VIRTUALIZACIÓN E INTRODUCCIÓN A DOCKER

En este  taller se creó una aplicación web usando el micro-framework de Spark java, la aplicación web ofrece las siguientes funciones: Seno, Coseno, Palíndromo, Vector. Una vez implementada esta aplicación se procede a construir un container docker, desplegarlo y configurarlo en nuestra máquina local. Luego, creamos un repositorio en DockerHub y subiremos la imagen al repositorio.

## Diseño de la aplicación

## Guía de Inicio

Las siguientes instrucciones le permitirán descargar una copia y ejecutar la aplicación en su máquina local.

### Prerrequisitos

- Java versión 8 OpenJDK
- Docker
- Maven
- Git

## Instalación 

### Docker

1. Abra la aplicación de escritorio de Docker.

   ![image](https://github.com/AndresOnate/AREP_TALLER5/assets/63562181/f1051197-c00b-4603-9dfd-d427a26d0eab)

2. Ejecute el siguiente comando para descargar la imagen del repositorio de docker:
   
     ``` docker run -d -p 34000:46000 --name dockercontainer aonatecamilo/arep_taller5```

   Debería ver algo así en consola:

   ![image](https://github.com/AndresOnate/AREP_TALLER5/assets/63562181/828a8d77-43ac-4a8f-8d48-cf1025df14c1)

   Verifique en la aplicación de escritorio de Docker que el contenedor se esté ejecutando
   
   ![image](https://github.com/AndresOnate/AREP_TALLER5/assets/63562181/8ca8bc5c-0b3a-4623-999f-2ccaa638424c)

### Respositorio en GitHub

1. Ubíquese sobre el directorio donde desea realizar la descarga y ejecute el siguiente comando:
   
     ``` git clone https://github.com/AndresOnate/AREP_TALLER5.git ```

2. Navegue al directorio del proyecto:
   
      ``` cd  AREP_TALLER5 ```

3. Ejecute el siguiente comando para compilar el código:

      ``` mvn compile ```

5.  Ejecute el siguiente comando para empaquetar el proyecto:
   
      ``` mvn package ``` 

6. Para iniciar el servidor, ejecute el siguiente comando:

    ``` ava -cp "target/classes:target/dependency/*" org.eci.arep.app.SparkWebServer ```

7. Verifique en la linea de comanos que se imprimió el mensaje **Listo para recibir ...**
   


## Probando la Aplicación.  

Ingrese a la siguiente URL para ingresar a el cliente: `http://localhost:34000/index.html`

Ingrese en los campos del formulario los valores, de clic en el botón `Search`:

![image](https://github.com/AndresOnate/AREP_TALLER5/assets/63562181/c5247754-f588-45cc-a17c-d3c1d6ec1523)

Función Seno:



## Construido Con. 

- Maven - Administrador de dependencias

## Versión
1.0.0
