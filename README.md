# practica-docker-nginx

### PARTE A
Para realizar la práctica con Nginx, solo necesitaremos el siguiente comando para descargar la imagen de Nginx:
```js
docker pull nginx
```

<img width="800" alt="image" src="https://user-images.githubusercontent.com/91556453/157730396-a9ba7d25-8960-4c91-ac67-fcad0f387703.png">

Una vez descargada la imagen, tendremos que ejecutarla mediante el comando:
```
docker run --rm -d -p 8080:80 --name web nginx
```
Con el comando anterior, comienza la ejecución del contenedor y publica el puerto 8080 en la red del host. Al ejecutar el comando, vemos la página por defecto de Nginx:

<img width="568" alt="image" src="https://user-images.githubusercontent.com/91556453/158657607-3fd06dea-e4e6-4789-9006-aa2671feed14.png">

Si deseamos detener el contenedor, utilizamos:

<img width="284" alt="image" src="https://user-images.githubusercontent.com/91556453/158658225-a4f5d910-d970-4c9d-918f-f2fd9058cb05.png">

Si queremos modiciar el contenedor, deberemos crear un archivo **html**, escribiendo en él todo lo que queremos mostrar en el contenedor:

<img width="329" alt="image" src="https://user-images.githubusercontent.com/91556453/158658725-1c475987-f210-4b41-a358-448a8b7b12f2.png">

Ahora, debemos poner la ubicación del archivo **html** en el comando anterior, y así, nos abrirá el contenedor modificado a nuestro gusto:

<img width="980" alt="image" src="https://user-images.githubusercontent.com/91556453/158658958-85b9c459-4035-408b-acd8-6aef1427fb88.png">

Y, esta sería la visualización del contenedor:

<img width="980" alt="image" src="https://user-images.githubusercontent.com/91556453/158660074-067acba9-44c0-4e7e-b62a-fb428982d1b0.png">

### PARTE B

Sí que es posible subir la imagen creada en Docker Hub a Microsoft Azure, solo tendremos que instalar Docker en la máquina, para que sea capaz de descaragar la imágen y que cree un contenedor sobre ella.

