# COMPLETAR  
Comparando sus conocimientos antes de hacer la práctica con sus conocimientos después de hacer la tarea, explicar los principales aprendizajes logrados para beneficio de su formación profesional.  
Si solucionó un problema presentado al realizar la práctica también se debe documentar.

## Mi Aprendizaje

* Aprendí que Docker Compose permite definir y levantar múltiples contenedores 
  con un solo comando `docker compose up -d`, usando un archivo `compose.yaml`.

* Aprendí que en el archivo `compose.yaml` la indentación debe ser con espacios, 
  no tabuladores, y que cada error de indentación impide que el archivo funcione.

* Aprendí que `depends_on` con `condition: service_healthy` garantiza que un 
  servicio espere a que otro esté saludable antes de iniciarse, lo que es 
  esencial cuando WordPress necesita que MySQL esté listo.

* Aprendí que los healthchecks en compose se configuran con `test`, `interval`, 
  `timeout`, `retries` y `start_period`, y que cada servicio puede tener 
  su propio comando de verificación.

* Aprendí que `docker compose ps` lista solo los contenedores creados por 
  compose, y `docker compose down` los elimina junto con la red.

* Aprendí que SonarQube requiere PostgreSQL como base de datos y se conecta 
  mediante la variable `SONAR_JDBC_URL` con la cadena de conexión JDBC.

* Aprendí que los volúmenes nombrados en compose persisten los datos aunque 
  se ejecute `docker compose down`, y solo se eliminan con `docker compose down -v`.

* Aprendí que el atributo `version` en compose.yaml está obsoleto y genera 
  una advertencia, por lo que se recomienda omitirlo en versiones recientes.
