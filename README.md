# Sistema de login com Node.js e MySQL
Aplicação de login desenvolvida com Node.js em conjunto com o banco de dados MySQL

<h2> Banco de Dados </h2>

```
--Criar um banco de dados no MySQL.

CREATE DATABASE dblogin;

use dblogin;

CREATE TABLE users(
	id INTEGER PRIMARY KEY AUTO_INCREMENT,
    username VARCHAR (100) NOT NULL,
    email VARCHAR (100) NOT NULL,
    idade INTEGER NOT NULL,
    pass INTEGER NOT NULL

);

--Caso aconteça problema de conexão com o banco, rodar no Workbench:

em casa
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY '';
flush privileges;

ou no laboratorio
ALTER USER 'user2020108000'@'localhost:8081' IDENTIFIED WITH mysql_native_password BY '2015108000';
flush privileges;

```

<h2> Comandos</h2>

```
--Dependências:
npm init
npm install nodemon
npm install -- save express
npm install express-session
npm install --save body-parser
npm install --save mysql
npm install ejs -save

-- Altere os dados de conexão com banco mysql em app.js

function conectiondb()
    var con = mysql.createConnection
        host: '', // O host do banco. Ex: turing, nome da conexão do banco
        user: '', // Um usuário do banco. user2020108000 
        password: '', // A senha do usuário. Ex: 2020108000
        database: '' // A base de dados a qual a aplicação irá se conectar. Ex: db2020108000


--Para subir o servidor:
node app.js
localhost:8081

```