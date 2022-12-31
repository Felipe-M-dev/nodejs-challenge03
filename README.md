# Desafío - Like Me (Parte I)

- Para realizar este desafío debes haber estudiado previamente todo el material disponible correspondiente a la unidad. </br>
- Desarrollo desafío:
  - El desafio se debe desarrollar de manera Individual.
  - Para la realización del desafío necesitarás apoyarte del archivo _Apoyo Desafío - Like Me_

## Descripción

La red social "Like Me" está apenas iniciando el proceso de desarrollo, se encuentra estudiando el mercado y analizando la competencia y ha descubierto que el éxito de esta industria se enfoca en los likes de los posts emitidos por los usuarios, por lo que decidió iniciar con el desarrollo de la lógica correspondiente a la creación de posts y a la interacción de likes que este puede tener.

En este desafío serás un desarrollador full stack developer de la empresa "Like Me" y deberás crear un servidor que disponibilice las rutas __GET__ y __POST__ para consultas y guardar los post en una base de datos PostgresSQL con el paquete pg.

Para el desarrollo de este desafío dispondrás de un Apoyo Desafío - Like Me, que contiene una aplicación React con la interfaz que te mostramos en la siguiente imagen.

<p align="center">
  <img src="https://github.com/Felipe-M-dev/nodejs-challenge03/blob/main/desafio03_01.png?raw=true?raw=true" alt="Imagen 01"><br>
</p>

La siguiente imagen muestra la interacción de la aplicación cliente al registrar un nuevo post.

<p align="center">
  <img src="https://github.com/Felipe-M-dev/nodejs-challenge03/blob/main/desafio03_02.png?raw=true?raw=true" alt="Imagen 02"><br>
</p>

Esta aplicación React de apoyo incluyte las consultas HTTP a un servidor local en el puerto 3000 con las rutas correspondientes al desafío en sus diferentes interacciones.

Para iniciar con el desarrollo de este desafío, ocupa las siguientes instrucciones SQL para crear una base de datos __likeme__ y una tabla __post__.

```sql
CREATE DATABASE likeme;
```

```sql
CREATE TABLE posts (id SERIAL, titulo VARCHAR(25), img VARCHAR(1000), descripcion VARCHAR(255), likes INT);
```

## Requerimientos

1. Habilitar los __cors__ en el servidor utilizando el paquete de npm. __(2 puntos)__

2. Usar el paquete __pg__ para conectarse e interactuar con la base de datos. __(2 puntos)__

3. Crear una ruta GET con Express para devolver los registros de una tabla alojada en PostgreSQL. __(3 puntos)__

4. Crear una ruta POST con Express que reciba y almacene en PostgreSQL un nuevo registro. __(3 puntos)__

  😊 ¡Mucho éxito!
  
## Solución

1. Descargar el proyecto.

2. Desde una terminal, posicionarse sobre la carpeta del proyecto y lanzar el siguiente comando:

```npm install```

3. Setear los valores del archivo `.env` a los correspondientes de la base de datos PostrgreSQL que utilizará.

4. Levantar servidor con el siguiente comando:

```npm start```

5. Cuando el server ya se encuentre arriba, ingresar al navegador y validar sitio en la siguiente URL:

```http://localhost:3000/```

6. Conectarse a PostgreSQL y lanzar el contenido del archivo script.sql ubicado en la ruta `script/script.sql` para crear la base de datos y la tabla solicitada.

## Validaciones

1. Se agrega un post de test para verificar funcionamiento:

<p align="center">
  <img src="https://github.com/Felipe-M-dev/nodejs-challenge03/blob/main/desafio03_03.png?raw=true?raw=true" alt="Imagen 03"><br>
</p>

2. Se valida registro correcto en base de datos PostgreSQL y en consola:

<p align="center">
  <img src="https://github.com/Felipe-M-dev/nodejs-challenge03/blob/main/desafio03_04.png?raw=true?raw=true" alt="Imagen 04"><br>
</p>

3. Revisión de registro en endpoint `/posts`:

<p align="center">
  <img src="https://github.com/Felipe-M-dev/nodejs-challenge03/blob/main/desafio03_05.png?raw=true?raw=true" alt="Imagen 05"><br>
</p>
