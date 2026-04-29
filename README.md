# Academia Full Revisado

Projeto didático completo de Desenvolvimento Web Back-End com Spring Boot, JPA, Validation, arquitetura em camadas, SQL Server/MySQL/H2 e frontend funcional.

## Rodar rápido com H2
```bash
mvnw.cmd spring-boot:run
```
Acesse: `http://localhost:8081`

## LAB A27 - SQL Server
No `application.properties`:
```properties
spring.profiles.active=sqlserver
```
No SSMS, conectar em `A2702\SQLEXPRESS` com Autenticação do Windows. Ajuste usuário/senha JDBC se necessário.

## Máquina pessoal - MySQL
No `application.properties`:
```properties
spring.profiles.active=mysql
```
Crie o banco:
```sql
CREATE DATABASE academia CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
```
Ajuste `spring.datasource.username` e `spring.datasource.password` em `application-mysql.properties`.

## Rotas principais
- `POST /api/planos`
- `GET /api/planos`
- `PUT /api/planos/{id}`
- `DELETE /api/planos/{id}`
- `POST /api/alunos`
- `GET /api/alunos`
- `PUT /api/alunos/{id}`
- `DELETE /api/alunos/{id}`
