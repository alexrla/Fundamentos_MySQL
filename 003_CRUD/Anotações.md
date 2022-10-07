# MySQL



### CRUD



#### O que é CRUD

- **Ações mais utilizadas:**
  - **`CREATE`: criar/inserir dados (`INSERT`);**
  - **`READ`: ler dados (`SELECT`);**
  - **`UPDATE`: atualizar dados (`UPDATE`);**
  - **`DELETE`: deletar/remover dados (`DELETE`);**




#### Selecionando (exibindo) todos os dados de uma tabela

- **Comando: `SELECT * FROM nome_da_tabela;`**



#### Selecionando (exibindo) colunas específicas de uma tabela

- **Comando: `SELECT coluna1, coluna2,... FROM nome_da_tabela;`**
  - **Veja que aplicamos um filtro, selecionando apenas as colunas que queremos ver/exibir;**



#### Inserindo dados

- **Comando: `INSERT INTO nome_da_tabela (nomes_das_colunas...) VALUES (valores...)`**
  - **Colunas e valores (dados a serem inseridos), devem ser separados por vírgula;**

- **OBS.: se formos inserir dados, em todas as colunas, não é necessário informar as colunas:**

  ```sql
  INSERT INTO nome_da_tabela VALUES (valores...)
  ```

  

#### Cláusula WHERE

- **Cláusula utilizada em algumas queries, para podermos realizarmos uma filtragem/aplicar uma condição (seja para deletar/atualizar algum registro);**
- **Se não utilizarmos esta cláusula, as instruções de atualizações ou de remoções, serão aplicadas a todos os registros, ou seja, todos os registros poderão ser atualizados ou apagados;**



#### Atualizando dados

- **Comando: `UPDATE nome_da_tabela SET nome_da_coluna=novo_valor WHERE filtro;`**
  - **Podemos atualizar mais de uma coluna. Para isso, as separamos por vírgula;**



#### Deletando dados

- **Comando: `DELETE FROM nome_da_tabela WHERE filtro;`**





