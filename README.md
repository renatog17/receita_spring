# receita_spring_mysql

## Spring Initializr
Acesse https://start.spring.io/


Dependências: 
* Spring Boot DevTools
* Spring Web
* Validation
* Spring Security
* MySQL Driver
* Flyway Migration
* Flyway Migration MySQL


## application.properties
```
spring.datasource.url=jdbc:mysql://localhost:3306/aluraflix  
spring.datasource.username = root 
spring.datasource.password = admin 
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver 
spring.jpa.show-sql=true 
spring.jpa.properties.hibernate.format_sql=true 
spring.data.web.pageable.page-parameter=pagina 
spring.data.web.pageable.size-parameter=tamanho 
spring.data.web.sort.sort-parameter=ordem 
server.error.include-stacktrace=never 
api.security.token.secret=${JWT_SECRET:12345678} 
```
