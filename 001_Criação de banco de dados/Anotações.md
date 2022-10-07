# MySQL



### Criação de banco de dados



#### Criação de um banco de dados

- **Comando: `CREATE DATABASE nome_do_banco;`**



#### Exibição dos bancos de dados

- **Comando: `SHOW DATABASES;`**
  - **Exibe todos os bancos existentes (todos os bancos que criados);**



#### Exclusão de um banco de dados

- **Comando: `DROP DATABASE nome_do_banco;`**
  - **Deleta/remove o banco especificado (essa ação é chamada/conhecida por "dropar");**
  - **Todos os dados são perdidos;**



#### Exportando um banco de dados

- **Comando: `mysqldump -u root nome_do_banco > nome_do_arquivo.sql`**
  - **Dessa forma, todas as tabelas e dados ficarão em um arquivo de extensão `.sql`;**



#### Utilizando um banco de dados

- **Comando: `USE nome_do_banco;`**
  - **Seleciona o banco especificado, para uso (a partir daí, todos os comandos utilizados serão direcionados a este banco);**





