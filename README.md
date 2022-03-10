# practica-docker-nginx

Para realizar la práctica con Nginx, solo necesitaremos el siguiente comando para descargar la imagen de Nginx:
```js
docker pull nginx
```

<img width="800" alt="image" src="https://user-images.githubusercontent.com/91556453/157730396-a9ba7d25-8960-4c91-ac67-fcad0f387703.png">

Una vez descargada la imagen, tendremos que ejecutarla mediante el comando:
```
docker run --rm -d -p 8080:80 --name web nginx
```
Con el comando anterior, comienza la ejecución del contenedor y publica el puerto 8080 en la red del host. Al ejecutar el comando, vemos la página por defecto de Nginx, pero ahora vamos a servir una hecha por nosotros, poniendo en la 
