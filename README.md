# 📦 How to Migrations
First, clone this repository: 

https://github.com/federus1105/koda-b4-db.git
```bash
cd migrations
```
### Install Go migrate
```bash
go install -tags 'postgres' github.com/golang-migrate/migrate/v4/cmd/migrate@latest;
```
### Create database
```bash
CREATE DATABASE <database_name>;
```
#### ⚠️ Attention: This ENUM only applies to PostgreSQL.
### Migrations Up
```bash
migrate -path . -database "postgres://user:password@localhost:5432/database?sslmode=disable" up 
```
### Migrations Down
```bash
migrate -path . -database "postgres://user:password@localhost:5432/database?sslmode=disable" down
```

 ## 👨‍💻 Author
**Federus Rudi**  
📧 federusrudi@gmail.com