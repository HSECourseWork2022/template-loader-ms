# Template Application

Ready to kick-start Spring Boot application template with Dockerfile and docker-compose.yml
* Java: 17
* Spring Boot: 2.7.5
# What do you need to update?
1. Rename `TemplateApplication` in `dev.hse.template` package
2. Under `src/main/java` rename `dev.hse.template` package to your preferred one
3. Change `artifactId` in pom from `template-spring-project` to your project's
4. (If needed) Update `docker-compose.yml`
   1. Change application service name `template_app`
   2. Change container name `template_container`

```bash
./mvnw clean
./mvnw package -Dmaven.test.skip
docker compose up
```