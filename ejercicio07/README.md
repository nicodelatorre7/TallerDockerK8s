## Ejercicio 07

- Se estan ejecutando 2 contenedores 
- Las imagenes son: `nicopaez/jobvacancy-ruby:1.3.0` y `postgres` 

- Ambas lineas de `image` especifican que imagen utilizara cada contenedor
- La linea de `links` le dice al contenedor `web` como "comunicarse" con el otro contenedor
- La linea `ports` especifica en que puerto correra la app web
- Dentro de `environment` setea variables de entorno, y en la linea de `DATABASE_URL` especifica como conectarse a la base de datos, tomando como contraseña la setteada en la variable de entorno dentro de `db` 

- Pueden verse entre si por el linkeo que hay en: 
```
    links:
      - db
```