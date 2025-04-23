# MYSQL-aulapratica-

show databases; 
-- mostrar os bancos de dados 
create database tads049; 
-- se atentar ao colocar qual DB usar 
use tads049;
-- criar banco de dados 
/* e la vamos nos: quando eu quero um banco de dados com um nome que tenha espaço entre si, tem que colocar underline
"create table (nome la), dai coluna 1 com tipo de dados e restições" tipo:
*/ 
-- para saber o erro do seu codigo pegar e colocar (; tipo um sorriso com piscada
/*para criar uma chave primaria para o seu banco de dados */
CREATE TABLE departamento (
id INT PRIMARY KEY AUTO_INCREMENT,
nome VARCHAR (100) 
);
/* varchar (esse var ai é significaruma variavel visse)*/
show tables; 

/*id (nome) INT AUTO_INCREMENT PRIMARY KEY: Isso cria uma coluna de numeros inteiros que é incrementada automaticamnte e serve como chave primaria*/

show tables;
/* exemplo de uso dos tipos de dados numericos. o tipo de dado double tem mais precisão que o decimal */
create table produto(
	ID int auto_increment primary key,
    preco_prateliera decimal(10,2) default 1.99999,
    -- truncagem (arredondamento)
    -- esse 10 é relacionado ao numero de caracteres antes da virgula
    preco_precisao double default 1.99999
    );
    /* inserindo 
    */
    insert into produto () values(); 
    -- para mostrar a tabela 
    select * from produto; 
-- para mostrar a tabela 
    describe produto; 
-- para saber a versão do sistema do mysql
select version();

create table usuarios ( 
	nickname varchar(20) not null, 
    senha varchar(15) not null, 
    descricao text 
);
desc usuarios;
