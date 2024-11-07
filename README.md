# LiteraturaChallengeOne
# Instalacion
Clonar el repositorio:

1) git clone https://github.com/andres-dev2111/LiteraturaChallengeOne.git

2) cd LiterAlura-ChallengeONEcd LiterAlura-ChallengeONE
   
 Configurar la base de datos:Configurar la base de datos: Ejecutar PostgreSQL y crear la base de datos literalura.
Configurar las credenciales de la base de datos en:

3) src/main/resources/application.properties:
# Nombre de la aplicación
spring.application.name=literalura

# Configuración de la conexión a la base de datos PostgreSQL
spring.datasource.url=jdbc:postgresql://${DB_HOST}/desafio_literalura
spring.datasource.username=${DB_USER}
spring.datasource.password=${DB_PASSWORD}
spring.datasource.driver-class-name=org.postgresql.Driver

# Configuración específica de Hibernate para PostgreSQL
hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect

# Propiedades opcionales de JPA para mostrar y formatear las consultas SQL
 spring.jpa.show-sql=true
 spring.jpa.format-sql=true
 
# Compilar y ejecutar la aplicación:

Compilar el proyecto usando Maven:
mvn clean install
Ejecutar la aplicación:
mvn spring-boot:run
Interactuar con la aplicación:

# Menu de inicio
BIBLIOTECA DIGITAL
----------------- MENÚ PRINCIPAL -----------------
1. Buscar libro por título
2. Listar libros registrados
3. Listar autores registrados
4. Listar autores vivos en un determinado año
5. Listar libros por idioma
6. Visualizar datos estadísticos
7. Mostrar top 10 libros descargados
8. Buscar autor por nombre
9. Listar autores que nacieron y murieron en un determinado rango de años
0. Salir de la aplicación

Selecciona una opción (1-9):
