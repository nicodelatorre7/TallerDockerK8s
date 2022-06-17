## Ejercicio 04

Descargo `java:8`

```
docker pull java:8
```

Armo el Dockerfile: 
```Dockerfile
FROM java:8
ADD passwordapi.jar /passwordapi.jar
EXPOSE 8080
ENTRYPOINT ["java", "-jar", "passwordapi.jar"]
```

Buildeo:
```
docker build -t pwdapi . 
```

Ejecuto:
```
docker run -p 8080:8080 pwdapi
```

Subo la imagen a DockerHub:
```
docker tag pwdapi ndelatorre/pwdapi
docker push ndelatorre/pwdapi
```

Imagen:
```
https://hub.docker.com/r/ndelatorre/pwdapi
```