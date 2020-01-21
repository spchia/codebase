# codebase
Starter code for java web project using spring boot

## To use this code
Download the source code using 'Download Zip' instead of git clone.
### Things to change
- In pom.xml:
    - artifactId
    - version
    - prj.displayname
    - start-class (if package path is change)
- In application.properties:
    - spring.application.name
    - logging.level.pengster.codebase (if package path is changed) 

## Requirement
- Maven - to manage dependencies and build
- JDK 1.8
- MySQL
- Environment Variables
    - DB_HOST - database hostname, e.g. localhost
    - DB_PORT - database port number, e.g. 3306
    - DB_USERNAME - database username for login
    - DB_PASSWORD - database password for login
  
 ## Build and Run
To build the project, on command prompt:
 ```shell script
$ cd <project folder>
$ mvn clean install
```
Jar will appear in `target` folder, this jar will contain all the dependencies, to run the jar:
```shell script
$ cd <project folder>/target
$ java -jar <jar file name>.jar 
```
> Remember to export the required environment variables before running the jar.

## Additional Information
### Database versioning
Database versioning is done using [flyway](https://flywaydb.org/).
SQL scripts is keep in src/main/resources/db/migration.  
