# flywayDemo

This project is a demo spring-boot project showing how we can configure flyway, a database migration tool, for database migration as well as version control for our database.


## Steps to set up flyway:

 - Add Flyway dependency to pom file.
 - Create a database user with full DDL permissions.
 - Add configuration for `datasource.url`, `datasource.username` and `datasource.password`.
 - Create `src/main/resources/db/migration` folder in project.
 - For each changes in database, create a new file in format: `V[VersionID]__NameOfChanges.sql`.
 - Note: To add database migration on existing database, add `flyway.baselineOnMigrate = true` in properties file.
 
 
