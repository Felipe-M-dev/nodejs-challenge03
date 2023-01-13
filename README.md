# Desafío - Like Me (Parte II)

- Para realizar este desafío debes haber estudiado previamente todo el material disponible correspondiente a la unidad. </br>
- Desarrollo desafío:
  - El desafio se debe desarrollar de manera Individual.
  - Para la realización del desafío necesitarás apoyarte del archivo _Apoyo Desafío - Like Me_

## Descripción

La red social “Like Me” sigue desarrollando su plataforma y ahora necesita permitir la interacción de likes y la eliminación de posts.

En esta segunda parte del desafío deberás:

1. Agregar una ruta PUT en una API REST y utilizarla para modificar registros en una tabla alojada en PostgreSQL __(4 puntos)__

2. Agregar una ruta DELETE en una API REST y utilizarla para eliminar registros en una tabla alojada en PostgreSQL __(4 puntos)__

3. Capturar los posibles errores en una consulta SQL realizada con el paquete pg usando la sentencia try catch __(2 puntos)__

La siguiente imagen muestra la interacción de la aplicación cliente al registrar likes en un post.

<p align="center">
  <img src="https://github.com/Felipe-M-dev/nodejs-challenge03/blob/main/desafio03_06.png?raw=true?raw=true" alt="Imagen 06"><br>
</p>

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

2. Estado inicial en la base de datos:

<p align="center">
  <img src="https://github.com/Felipe-M-dev/nodejs-challenge03/blob/main/desafio03_07.png?raw=true?raw=true" alt="Imagen 07"><br>
</p>

3. Se dan 7 clicks en el like:

<p align="center">
  <img src="https://github.com/Felipe-M-dev/nodejs-challenge03/blob/main/desafio03_08.png?raw=true?raw=true" alt="Imagen 08"><br>
</p>

4. Estado en la base de datos:

<p align="center">
  <img src="https://github.com/Felipe-M-dev/nodejs-challenge03/blob/main/desafio03_09.png?raw=true?raw=true" alt="Imagen 09"><br>
</p>

5. Estado en el endpoint:

<p align="center">
  <img src="https://github.com/Felipe-M-dev/nodejs-challenge03/blob/main/desafio03_10.png?raw=true?raw=true" alt="Imagen 10"><br>
</p>

6. Se da click en la X para eliminar post:

<p align="center">
  <img src="https://github.com/Felipe-M-dev/nodejs-challenge03/blob/main/desafio03_11.png?raw=true?raw=true" alt="Imagen 11"><br>
</p>

<p align="center">
  <img src="https://github.com/Felipe-M-dev/nodejs-challenge03/blob/main/desafio03_12.png?raw=true?raw=true" alt="Imagen 12"><br>
</p>

7. Estado en base de datos:

<p align="center">
  <img src="https://github.com/Felipe-M-dev/nodejs-challenge03/blob/main/desafio03_13.png?raw=true?raw=true" alt="Imagen 13"><br>
</p>

8. Estado en endpoint:

<p align="center">
  <img src="https://github.com/Felipe-M-dev/nodejs-challenge03/blob/main/desafio03_14.png?raw=true?raw=true" alt="Imagen 14"><br>
</p>
