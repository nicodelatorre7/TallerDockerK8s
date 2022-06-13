## Ejercicio 01

Descargo `nginx`
```
docker pull nginx
```
Creo un `Dockerfile` con el siguiente contenido: 
```
FROM nginx:alpine
COPY . /usr/share/nginx/html
```

Ejecuto el siguiente comando: 
```
docker build -t html-server .
docker run -d -p 80:80 html-server
```

Verifico que quedo funcionando:
```
curl localhost:80
```