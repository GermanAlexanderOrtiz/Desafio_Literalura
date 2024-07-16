# Desafío literalura
Este proyecto, llamado "Desafío Literalura", fue realizado como parte de la formación en el programa Oracle Next Education (Oracle ONE). Es una aplicación de consola en Java que permite a los usuarios buscar libros por título, listar libros y autores registrados, listar autores vivos en un determinado año, listar libros por idioma, ver los 10 libros más descargados y obtener estadísticas.

## Descripción del proyecto
El proyecto utiliza Java como lenguaje de programación, Spring Boot como framework y Maven para la gestión de dependencias. La estructura del proyecto sigue la estructura estándar de Maven y está organizado en varios paquetes, incluyendo modelos, repositorios y servicios.

La aplicación consume la API de Gutendex para obtener datos de libros y autores, y luego convierte estos datos en objetos de modelo que se pueden manipular dentro de la aplicación. Los datos de los libros y autores se almacenan en una base de datos, lo que permite a los usuarios realizar búsquedas y obtener estadísticas.

La comunicación con la aplicación se realiza a través de la consola, con el siguiente menú: 

                    1 - Buscar libros por título
                    2 - Listar libros registrados
                    3 - Listar autores registrados
                    4 - Listar autores vivos en un determinado año
                    5 - Listar libros por idioma
                    6 - Top 10 libros más descargados
                    7 - Obtener estadísiticas
                    0 - Salir

## Como usar la aplicación
**Clonar el repositorio**

Para empezar, necesitas clonar el repositorio en tu máquina local. Puedes hacerlo utilizando el siguiente comando en tu terminal:
   `git clone https://github.com/GermanAlexanderOrtiz/Desafio_Literalura.git`
   
O si lo prefieres, puedes presionar el botón verde `code<>` del repositorio y descargar los archivos como ZIP

1. Configurar la base de datos

La aplicación utiliza una base de datos PostgreSQL. Deberás crear una base de datos local y configurar las credenciales de la base de datos en el archivo src/main/resources/application.properties. Reemplaza ${DB_HOST}, ${DB_NAME_LITERALURA} ${DB_USER} y ${DB_PASSWORD} con tus propios valores (Puede ser en el mismo archivo properties, o creando tus propias variables de entorno).
- DB_HOST: el nombre de tu host (si la base de datos está en tu computadora, pon localhost).
- DB_NAME_LITERALURA: el nombre de tu base de datos.
- DB_USER: el nombre del usuario de la base datos (por default, postgres pondrá el nombre de "postgre").
- DB_PASSWORD: la contraseña que pusiste para postgreSQL

2. Compilar y ejecutar la aplicación

La aplicación utiliza Maven para la gestión de dependencias. Puedes compilar y ejecutar la aplicación utilizando los siguientes comandos en tu terminal:  <pre>cd desafio-literalura mvn clean install mvn spring-boot:run </pre> Esto compilará la aplicación y la iniciará.
Asimismo, si prefieres ejecutarla desde un IDE como IntelliJ por ejemplo, solo tienes que abrir el proyecto y correr la clase DesafioLiteraluraApplication.

3. Interactuar con la aplicación

Una vez que la aplicación esté en ejecución, puedes interactuar con ella a través de la consola. Se te presentará un menú con varias opciones para buscar libros, listar libros y autores registrados, listar autores vivos en un determinado año, listar libros por idioma, ver los 10 libros más descargados y obtener estadísticas.  Simplemente sigue las instrucciones en pantalla para interactuar con la aplicación.

## Tecnologías utilizadas
- Java SE22
- Maven
- Spring Boot V3.3.1
- Para el desarrollo del código, se usó el IDE IntelliJ
- Para la base de datos, se usó PostgreSQL

## Estado del proyecto

Finalizado.















