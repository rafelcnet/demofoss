## Introducción 

Ejemplo basico para crear una aplicacion .net core, crear una imagen en docker, y despues hacer un deployment con Kubernetes a un cluster de Raspberry PI:

http://myapps.rafaelc.net/post/2019/06/07/Contenedores-y-cluster-con-Raspberry-parte-1.aspx 

## Uso 

El archivo Dockerfile es para crear la imagen, la sintaxis para hacerlo y para subirlo al jub de Docker es:

* docker build -t [usuarioDocker]/[aplicacion] -f Dockerfile .

* docker push [usuarioDocker]/[aplicacion]

Los archivos yaml se usan para hacer el deployment en el master del cluster de Raspberry con Kubernetes, de esta forma:

* kubectl apply -f mydeploy.yaml
* kubectl apply -f myservice.yaml
