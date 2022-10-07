# MySQL



### Criação de tabelas



#### O que é uma tabela

- **Entidade responsável por guardar os dados;**
  - **Ela possui colunas;**
  - **Essas colunas são utilizadas para categorizar os dados (reuní-los em grupos);**
  - **As colunas ainda possuem tipos de dados determinados (textos, números, datas, etc.) e atributos (não nulos, chave primária, auto incremento, etc.);**
    - **Os atributos (constraints - restrições) correspondem as características de cada coluna, que determinam como os dados serão inseridos nela;**



#### Criando uma tabela

- **Comando: `CREATE TABLE nome_da_tabela (nome_da_coluna tipo_de_dado, ...);`**
  - **Diversas colunas, com diferentes tipos de dados, podem ser inseridas na tabela;**



#### Removendo uma tabela

- **Comando: `DROP TABLE nome_da_tabela;`**
  - **Todos os dados serão perdidos;**



#### Alterando uma tabela

- **Tipos de alteração no SQL:**
  - **Adição de colunas;**
  - **Remoção de colunas;**
  - **Modificação de tipo da coluna;**



##### Adicionando nova coluna a uma tabela

- **Comando: `ALTER TABLE nome_da_tabela ADD COLUMN nome_da_nova_coluna tipo_da_nova_coluna;`**



##### Removendo coluna de uma tabela

- **Comando: `ALTER TABLE nome_da_tabela DROP COLUMN nome_da_coluna;`**



##### Modificando o tipo de uma coluna

- **Comando: `ALTER TABLE nome_da_tabela MODIFY COLUMN nome_da_coluna novo_tipo_da_coluna;`**



#### Tipos de dados

- **Classificam um dado;**

- **Cada coluna deve ter um tipo de dado específico;**
- **Tipos de dados:**
  - **`texto`**
  - **`numérico`**
  - **`data`**
  - **`etc...`**
- **OBS.: alguns dados permitem a aplicação de limites (podemos determinar a quantidade máxima de caracteres, por exemplo);**



#####  Tipos de texto

- **`CHAR(x)`**
  - **Aceita textos contendo de 0 a 255 caracteres;**
- **`VARCHAR(x)`**
  - **Aceita textos de 0 a 65535 caracteres;**
- **`TINYTEXT`**
  - **Apenas textos com até 255 caracteres;**
- **`MEDIUMTEXT`**
  - **Apenas textos com até 16777215 caracteres;**
- **OBS_1.: `x` é a quantidade máxima;**
- **OBS_2.: `CHAR` e `VARCHAR` aceitam números e caracteres especiais;**



##### Tipos numéricos

- **`BIT(x)`**
  - **1 a 64 caracteres;**
- **`TINYINT(x)`**
  - **1 a 255 caracteres;**
- **`BOOL`**
  - **0 é falso e qualquer outro valor é verdadeiro;**
- **`INT(x)`**
  - **Valores entre -2147483648 a 2147483647;**
- **OBS.: não é necessário a utilização de aspas, ao realizar a inserção de dados de algum tipo numérico;**



##### Tipos de data

- **`DATE`**
  - **Aceita uma data no formato: `YYYY-MM-DD`;**
- **`DATETIME`**
  - **Aceita uma data com horário, no formato: `YYYY-MM-DD hh:mm:ss`;**
- **`TIMESTAMP`**
  - **Aceita uma data no formato `DATETIME`, porém apenas entre os anos de 1970 a 2038;**
- **OBS.: as datas são inseridas entre aspas;**



#### Inserindo dados no banco

- **Comando: **

  ```sql
  INSERT INTO nome_da_tabela (coluna1, coluna2,...) VALUES (valor1, valor2,...);
  ```

  - **Nomes das colunas e os dados a serem inseridos, devem ser separados por vírgula;**
  - **Os valores precisam ser inseridos de acordo com a ordem das colunas;**
  - **OBS.: valores de texto, devem ser inseridos entre aspas;**
