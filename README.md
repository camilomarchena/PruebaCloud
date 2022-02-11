# PruebaCloud

## Pasos para crear un Dockerfile y realizar su respectivo Pull

#### Crear el Docker file con vim  Dockerfile
- from nginx:alpine  == Siendo alpine la distribución Linux de nginx

#### Copy es copiar un archivo de nuestra maquina al contenedor 
- index.nginx-debian.html /usr/share/nginx/html/index.html
#### El Dockerfile quedaría así: 
![Image text](https://github.com/CAMILOMARCHENA/PruebaCloud/blob/main/DockerFile%20image.PNG)
#### Creamos una imagen de Dockerfile
- docker build -t simple-nginx .
#### Le asignamos el Puerto y le cambiamos el nombre al server de gninx
- sudo docker run --name sever_nginx_2 -d -p 8889:80 nginx

#### Repetimos los pasos anteriores una vez 
- Para así tener 3 imágenes en un mismo contenedor Docker

#### Realizamos un pull a nuestro repositorio
- git add .
- git commit -m 'nombre de nuestro commit'
- git push origin main
- vamos a github y le damos a compare and create a pull request
- despues oprimimos el boton para crear el pull request 
- Listo, el pull request ha sido creado
