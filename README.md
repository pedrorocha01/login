# Sistema de login com Node.js e MySQL
Aplicação de login desenvolvida com Node.js em conjunto com o banco de dados MySQL

<h2> Banco de Dados </h2>

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

ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY '';

flush privileges;

<h2> Comandos</h2>

--Dependências:
npm init
npm install nodemon -g 
npm install -- save express
npm install express-session
npm install --save body-parser
npm install --save mysql
npm install ejs -save

--Para subir o servidor:
node app.js