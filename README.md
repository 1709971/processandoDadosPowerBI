# Neste desafio será criado uma instância para mySQL no AWS (Amazon Web Service) para integrar com Power BI

## 1. Criação de uma instância na AWS (Amazon Web Service) para MySQL

### 1.1 - Foi utilizada uma conta gratuita na AWS - recurso banco de dados - RDS, para criar a instância.

![aws-1](https://github.com/1709971/processandoDadosPowerBI/assets/80554521/26d85f3a-d87b-4817-a78e-7904de4830c0)

### 1.2 - Foi criado um Banco de Dados e instância conforme imagens abaixo

![aws-2](https://github.com/1709971/processandoDadosPowerBI/assets/80554521/bd6b177e-620b-476a-9831-df36904d0b67)

### 1.3 - Após a criação ficará disopnivel em Banco de Dados

![aws-5](https://github.com/1709971/processandoDadosPowerBI/assets/80554521/00f3654d-528a-4297-93aa-a2c738ce3215)


## 2. Criação de Banco de dados com base disponível no github

### 2.1 - Foi utilizado os materiais disponíveis no GitHub para criação do banco de Dados no WorkBench - MySQL

![mysql-1](https://github.com/1709971/processandoDadosPowerBI/assets/80554521/4fe2627e-4389-4744-bb1e-e0fff79a50e1)

## 3. Integração do Power BI com AWS (Amazon Web Service) 

### 3.1 - Com o Power BI desktop aberto clique em obter dados

![pb-1](https://github.com/1709971/processandoDadosPowerBI/assets/80554521/7c51e36e-f473-4ec4-b2f4-690205541db2)

### 3.2 - Escolha a opção Banco de dados / Banco de dados MySQL

![pb-2](https://github.com/1709971/processandoDadosPowerBI/assets/80554521/2bb818fa-06c8-44d2-ac28-5719bd2e3da6)

### 3.3 - Utilize as credenciais do AWS e banco de dados para se conectar

![pb-3](https://github.com/1709971/processandoDadosPowerBI/assets/80554521/cb9c551a-fe4f-4b6e-9447-b6612dd4e95c)

## 4. Verificar problemas na base a fim de realizar a transformação dos dados

### Foi realizado os passos abaixo para transformar os Dados

1. Verifique os cabeçalhos e tipos de dados
2. Modifique os valores monetários para o tipo double preciso
3. Verifique a existência dos nulos e analise a remoção
4. Os employees com nulos em Super_ssn podem ser os gerentes. Verifique se há algum colaborador sem gerente
5. Verifique se há algum departamento sem gerente
6. Se houver departamento sem gerente, suponha que você possui os dados e preencha as lacunas
7. Verifique o número de horas dos projetos
8. Separar colunas complexas
9. Mesclar consultas employee e departament para criar uma tabela employee com o nome dos departamentos associados aos colaboradores. A mescla terá como base a tabela employee. Fique atento, essa informação influencia no tipo de junção
10. Neste processo elimine as colunas desnecessárias. 
11. Realize a junção dos colaboradores e respectivos nomes dos gerentes. Isso pode ser feito com consulta SQL ou pela mescla de tabelas com Power BI. Caso utilize SQL, especifique no README a query utilizada no processo.
12. Mescle as colunas de Nome e Sobrenome para ter apenas uma coluna definindo os nomes dos colaboradores
13. Mescle os nomes de departamentos e localização. Isso fará que cada combinação departamento-local seja único. Isso irá auxiliar na criação do modelo estrela em um módulo futuro.
14. Explique por que, neste caso supracitado, podemos apenas utilizar o mesclar e não o atribuir. 
- No Power Query, "Mesclar" é usado para combinar tabelas com base em colunas comuns, enquanto "Atribuir" é utilizado para adicionar ou modificar colunas com base em expressões ou valores definidos. Mesclar é útil para agregar informações de diferentes fontes, como clientes e pedidos, enquanto Atribuir permite criar colunas calculadas ou atribuir valores constantes. 

15. Agrupe os dados a fim de saber quantos colaboradores existem por gerente
16. Elimine as colunas desnecessárias, que não serão usadas no relatório, de cada tabela
