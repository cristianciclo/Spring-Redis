# Spring-Redis
En este proyecto, trataremos datos obtenidos de Redis mediante Spring, y como usar las notaciones @RequestMapping(), @PathVariable() y @RequestParam().

## Instalacion:
Para poner en funcinamiento nuestro proyecto, necesitaremos la base de datos redis, la debemos de iniciar colocandonos en la carpeta src de Redis y ejecutando <code>./redis-server ../redis.conf</code>

  Una vez iniciado redis, ejecutaremos el archivo python que nos introducira los datos en la base de datos 12 de redis, para ejecutarlo, nos moveremos donde tenemos el archivo y ejecutamos <code>phyton datos_redis.py</code>
  
  También necesitaremos tener maven instalado, con todo esto estaremos listo para ejecutarlo.
  
  ## Ejecución:
  Para ejecutar nuestro programa, nos iremos a la carpeta donde encontramos el pom.xml y ejecutaremos
  <code>mvn clean install jetty:run</code>
  
  Ya lo tenemos funcionando ahora nos iremos a nuestro navegador y pondremos <code>http://localhost:9999/employee</code>
  
  ## Funcionamiento:
  
  1. En la página principal encontraremos una selección de profesores, escojeremos uno y nos mandara a la siguiente vista.
  2. En esta vista, nos muestra los grupos que posee dicho profesor, seleccionaremos un grupo y nos llevara a la siguiente vista.
  3. Aquí, nos muestra los alumnos que tiene el grupo, seleccionaremos uno y nos llevara a la siguiente vista.
  4. Ahora, nos permitira añadir una nota al alumno que hemos seleccionado, esta nota aparecera en la consola, una vez introducida, nos mandara a la ultima vista en la cual nos muestra el mensaje de introducido y un boton para volver, el cual nos manda de nuevo al principio, es decir, a /employee.
  
  Resumen:
  Lista_Profesores --> Lista_Grupos --> Lista_Alumnos --> Añadir_Nota --> Volver
  
