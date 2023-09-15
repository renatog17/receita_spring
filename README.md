# receita_spring_mysql

## spring Initializr
acesse https://start.spring.io/


inclu as seguintes dependências: 
* Spring Boot DevTools
* Spring Web
* Spring Data
* Validation
* Spring Security
* JWT Token
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

## spring security

após adicionar a dependência do spring security, é necessário configurar a autenticação e autorização do projeto.

## flyway migration

por último, é necessário criar o script de criação da tablea 'usuarios' e adicionar um usuario.
```
create table usuarios(
    id bigint not null auto_increment,
    login varchar(100) not null,
    senha varchar(255) not null,
    primary key(id)
);
```
concluídos os passos acima, o projeto estará pronto para desenvolvimento.
