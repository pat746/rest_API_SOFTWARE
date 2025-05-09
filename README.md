1. clonar repositorio
```
git clone https://
```
2. reconstruir node_modules
```
npm install
```
3. construir el archivo .env 
```
DB_HOST=
DB_PORT=
DB_PASSWORD=
DB_USER=
DB_DATABASE=
```
4. RESTAURE LA db (db > database.sql)
```sql
CREATE DATABASE  appstore;

USE appstore;

CREATE TABLE softwares
(
  id          INT AUTO_INCREMENT PRIMARY KEY,
  nombre      VARCHAR(40)   NOT NULL,
  espaciomb   SMALLINT      NOT NULL,
  versionsoft VARCHAR(20)   NOT NULL,
  precio      DECIMAL(7,2)  NOT NULL
)ENGINE = INNODB;
```
5. ejecute el proyecto:
```
npm run dev 
```