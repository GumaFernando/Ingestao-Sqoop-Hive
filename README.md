# Ingestão de dados no hive utilizando o Scoop

Através dos conhecimentos adquiridos no Bootcamp de engenharia de dados da Semantix. Realizei uma prática de importação de uma tabela no banco de dados
do MYSQL diretamente para o Hive, realizando o armazenamento no HDFS no formato Parquet.

### Verificando quantidade total de registros na tabela do MYSQL -

Realizando uma contagem de total de registros no banco de dados relacional MySql. Total de 300024 registros no banco de dados relacional.

![alt text](https://github.com/GumaFernando/Projeto_Ingestao_Sqoop/blob/main/mysql_count_total.PNG?raw=true)

### Criação de um DataBase no Hive 

Criação de um banco de dados chamado "Guma" no Hive.

![alt text](https://github.com/GumaFernando/Projeto_Ingestao_Sqoop/blob/main/create_database_hive.PNG)

### Importando os dados do Mysql diretamente no HIVE

Fazendo a importação de uma tabela do banco de dados do Mysql, diretamente para o Hive.
- Salvando no formato Parquet
- usando Paralelismo para 2
- importando diretamente no banco de dados hive chamado "Guma"
- Criando uma tabela chamada Employees

![alt text](https://github.com/GumaFernando/Projeto_Ingestao_Sqoop/blob/main/sqoop_import.PNG)

### Validando registros no Hive ! 

Realizando a validação de importação no Hive, realizando a contagem geral dos registros. Sendo no total de 300024 registros importados com sucesso.

![alt text](https://github.com/GumaFernando/Projeto_Ingestao_Sqoop/blob/main/consulta_hive.PNG)

### Verificando arquivos no formato Parquet no hdfs 

Realizando a consulta diretamente no HDFS para verificação do formato do arquivo, neste caso foi validado armazenamento no formato Parquet.
dentro do caminho padrão /user/hive/warehouse

![alt text](https://github.com/GumaFernando/Projeto_Ingestao_Sqoop/blob/main/consulta_hdfs.PNG)
