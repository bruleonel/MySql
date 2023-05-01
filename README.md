# MySql

A linguagem SQL foi desenvolvida no começo dos anos 70, na cidade de São José, Califórnia, em um projeto chamado System R da IBM, do inglês International Business Machines, cujo objetivo era comprovar a viabilidade da implementação de um modelo relacional, que um estudioso chamado Codd estava propondo.

<img src="https://4b7b3223-a-62cb3a1a-s-sites.googlegroups.com/site/pioneiroscomputacao/p-1970-89/p61/ed_codd3.jpg?attachauth=ANoY7cpxdnWfPgAuzubQA6siXO-vIfB4Q59ee9ltPtvniqM7aRdvHVdyx05flOY3vekoZMllqU_qgc4CxtKqrqLp84Dbyyz66t_c66IWqsd1i2e9IYNQC7sO2kvN-w8KJLsOcbmgiaj0SozbFDY2QGpLWiDVyrI14Ve73FOtL20vBXX1wLeq4JyZosISUIRKcQlFMrGxmYk3d6JMvYqRl-C7JBmwoom-wwZCqtXsNpADaDtWRhRQ9_9wmH86OH2zu_BrxDEzkZYU&attredirects=0"  
width="200px" height="300px" alt="Minha Figura">
<a href="https://4b7b3223-a-62cb3a1a-s-sites.googlegroups.com/site/pioneiroscomputacao/p-1970-89/p61/ed_codd3.jpg?attachauth=ANoY7cpxdnWfPgAuzubQA6siXO-vIfB4Q59ee9ltPtvniqM7aRdvHVdyx05flOY3vekoZMllqU_qgc4CxtKqrqLp84Dbyyz66t_c66IWqsd1i2e9IYNQC7sO2kvN-w8KJLsOcbmgiaj0SozbFDY2QGpLWiDVyrI14Ve73FOtL20vBXX1wLeq4JyZosISUIRKcQlFMrGxmYk3d6JMvYqRl-C7JBmwoom-wwZCqtXsNpADaDtWRhRQ9_9wmH86OH2zu_BrxDEzkZYU&attredirects=0">Veja mais aqui</a>

Esse estudioso elaborou uma forma estruturada de realizar consultas nos bancos de dados que estavam surgindo, chamados “bancos de dados relacionais”.

Naquela época, os bancos de dados ainda não possuíam relacionamento entre as tabelas nas quais os dados eram armazenados. Era a categoria de banco de dados mais antigo, a sequencial, que efetuava a consulta dos registros de maneira sequencial, ou seja, um após o outro.

Com o surgimento dos bancos de dados relacionais (ou DBMS, do inglês, Data Base Management System, “Sistema de Gerenciamento de Banco de Dados), Codd considerou criar uma linguagem que facilitasse a extração e manipulação de dados, além da manipulação das estruturas desse banco aproveitando a característica de relacionamento entre eles.

Então, foi criada a linguagem SQL, do inglês Structured English Query Language, que traduzindo seria algo como “linguagem de consulta estruturada em inglês”. No inglês, geralmente, é pronunciado SEQUEL e não SQL, soletrando as letras - diferentemente do português, em que normalmente lemos como “ésse quê éle”.

## Objetivo

O principal objetivo da linguagem SQL é padronizar a maneira como os registros são consultados nos bancos de dados relacionais. Atualmente, os bancos relacionais aderem ao padrão SQL, que vai além das consultas: é usado também, na criação, alteração, estruturação e manipulação do banco de dados, além da maneira como banco de dados interage com a segurança, entre outros usos.

## Vantagens: 
- Essa padronização utilizando a linguagem SQL tem um custo reduzido do aprendizado. 
Por exemplo, o profissional com conhecimento sobre o SQL da Oracle conseguirá manipular facilmente o MySQL ou SQL Server da Microsoft. Por mais que existam diferenças (principalmente na parte de funções), a adaptação do profissional não é uma questão complicada.

- A portabilidade. 
Por exemplo, é mais simples migrar sistemas que usam Oracle para SQL Server ou para MySQL, ou vice-versa. Lembrando que quanto mais for utilizado o SQL Standard definido pelo ANSI, mais fácil será essa portabilidade no futuro. Então, é útil evitar as funções específicas do banco de dados e permitir que o programa realize essa tarefa.

- A longevidade é a garantia de que os seus relatórios ou processos utilizando o SQL irão funcionar por um longo período, já que estarão sempre adaptados ao padrão ANSI. Ou seja, ao efetuar um upgrade de banco de dados o seu sistema não ficará fora de serviço.

- A comunicação. O fato da maioria utilizar SQL permite a facilidade de comunicação entre os sistemas. Como, por exemplo, processos de ETL, (extract, transform and load), ou de integração entre sistemas que ficam mais simples de serem desenvolvidos, já que ambos utilizam o SQL padrão.

- Liberdade de escolha. Por existir um padrão de linguagem, se a empresa for optar pelo uso de um banco de dados relacional não ficará presa à linguagem de comunicação, por exemplo, já que são bem semelhantes. Ao tomar essa decisão, a corporação irá utilizar outros critérios de escolha, como performance, hardware, custo, entre outros.

## Desvantagens: 
- A privação da criatividade. O SQL possui limitações que podem não atender às novas demandas no mercado na linguagem SQL, principalmente com o surgimento das redes sociais e dos enormes volumes de dados, o chamado big data. Ou seja, há uma carência nas coletas de dados que estão trafegando na internet.

Para tal, estão surgindo outros bancos que usam padrões diferentes dos bancos de dados relacionais, o chamado NoSQL. Estes atendem de forma mais eficiente as demandas de tabelas de big data , como no caso das redes sociais. Lembrando que estamos nos referindo a estruturas que escapam do padrão ANSI e que, por isso, exigem um aprendizado mais específico.

- A escassez de estruturação da linguagem SQL, já que ela não possui if, for e when, isto é, comandos condicionais como as demais linguagens de programação.

Para conseguir suprir essa carência da estruturação, os bancos de dados relacionais da Oracle, SQL e MySQL criaram suas linguagens próprias internas que realizam esse conjunto de estruturação usando a linguagem SQL, mas que acaba se afastando um pouco do padrão ANSI.

Falando um pouco sobre o padrão ANSI, este possui três grupos de comandos. O primeiro, é o DDLs, ou Data Definition Language (linguagem de definição de dados). Os DDLs são a parte da linguagem SQL que permite a manipulação das estruturas do banco de dados. Como, por exemplo, criar um banco, tabelas, índices, apagar as tabelas e alterar a política de crescimento de índice. Ou seja, os comandos que envolvem a estrutura do banco de dados relacionais são os comandos do tipo DDL.

O segundo grupo de comandos são os chamados DML, ou Data Manipulation Language (linguagem de manipulação de dados). Esse grupo visa gerenciar os dados: incluindo, alterando e excluindo informações nas estruturas do banco, como as tabelas. Além disso, realizam as consultas, buscam as informações das estruturas e exibiremos para o usuário.

Finalmente, chegamos nos comandos DCL, ou Data Control Language ("linguagem de controle de dados"). Este grupo nos permite administrar o banco de dados como, por exemplo, o controle de acesso, o gerenciamento do usuário, gerenciar o que cada usuário(a) pode ou não visualizar, gerenciar o banco ao nível de estrutura (como a política de crescimento, como e onde será armazenado no disco), administrar os processos, saber quantos processos estão sendo executados, controle de log e assim por diante.

<img src="https://lh6.googleusercontent.com/N3nCjYeLaw030Jy9key4fOaAu_LKnzp8RCOmLlumwp0tc-hymIycnbzuhQXlisl-uo0hbTCzo7_QU3gTxBpqbaU5op08D_7ib4MHQJPhqbHAyjFsE8tVZLoZrYZ69P2Ick_LU6Mc" width="500px" height="300px">
<a href="https://blog.betrybe.com/sql/">Veja mais aqui</a>

# Trabalhando

## Select

### Considere o seguinte diagrama das tabelas e suas relações preenchidas:

![diagrama_workbench](https://user-images.githubusercontent.com/104650333/235514315-41b5ed63-d8cf-4afb-9e2e-65d4d4f9c62b.png)

- Para selecionar tudo de qualquer tabela use:

````
SELECT * FROM tabela_de_clientes;
````

![Captura de tela 2023-05-01 162303](https://user-images.githubusercontent.com/104650333/235515185-7a5357c1-4076-4bce-90e7-8cc0fbdd548b.png)

- Para selecionar campos específicos:
````JS
SELECT CPF, NOME FROM tabela_de_clientes;
````

- Em consultas SQL, existe a opção do uso de alias, que funciona como um apelido que atribuímos a determinado campo. Isso é feito com o uso de as:
````
SELECT CPF as IDENTIFICADOR, NOME as CLIENTE FROM tabela_de_clientes;
````
Nesse caso, "identificador" representa o CPF e "cliente" representa o NOME. Assim, quando o script for executado, notaremos que as colunas do resultado são os aliases e não os nomes originais dos campos (CPF e NOME).

![Captura de tela 2023-05-01 162933](https://user-images.githubusercontent.com/104650333/235516189-a1e6fb1e-0702-4ce4-aac0-3f41d151fade.png)

### A seguir, vamos consultar a "tabela_de_produtos":

````
SELECT * FROM tabela_de_produtos;
````
![Captura de tela 2023-05-01 163135](https://user-images.githubusercontent.com/104650333/235516517-7e5c8f46-edb1-4902-94dc-7ed8696c2413.png)

````
SELECT * FROM tabela_de_produtos WHERE CODIGO_DO_PRODUTO ="1000889";
````

![Captura de tela 2023-05-01 163349](https://user-images.githubusercontent.com/104650333/235516829-b9c23b03-f4b3-415d-8d36-fc047fcaf16f.png)

Essa consulta retorna apenas um produto, pois somente um suco tem sabor uva. Trocando o valor "uva" por "limão", nenhum produto será mostrado, pois não há sucos com esse sabor. Já ao escrever "laranja", são cinco os produtos que atendem a essa condição.

Mas qual é a grande diferença interna na execução da consulta com WHERE CODIGO_DO_PRODUTO = '1000889' e da consulta com WHERE SABOR = 'Uva'? A resposta está na performance!

Buscas com condições de filtro que possuem chaves primárias (como "CODIGO_DO_PRODUTO") são mais rápidas, pois chaves primárias têm índices que facilitam muito esse processo. "SABOR", por outro lado, não é uma chave primária nem estrangeira, logo não tem índice e consequentemente resulta numa busca um pouco mais lenta.

Como nosso banco de dados atual é relativamente pequeno, essa lentidão não é perceptível, porém essa diferença de performance pode ser problemática em bancos mais volumosos. Uma forma de solucionar esse problema é atribuindo um índice à coluna, algo que aprenderemos mais para frente, em outro curso de MySQL.

- Seguindo com as consultas, agora vamos fazer um filtro referente à embalagem:

````
SELECT * FROM tabela_de_produtos WHERE EMBALAGEM = 'PET';
````

![Captura de tela 2023-05-01 163557](https://user-images.githubusercontent.com/104650333/235517168-c5c466df-a52e-4d7a-a194-54467885899c.png)

Ao executar esse script, note que na tabela o valor "PET" está escrito com letras maiúsculas. O que será que acontece se eu fizer a consulta usando letras minúsculas?

````
SELECT * FROM tabela_de_produtos WHERE EMBALAGEM = 'pet';
````

O resultado é o mesmo! Como vimos anteriormente, o MySQL não distingue entre letras maiúsculas e minúsculas, ele fará a busca da mesma forma.

- Também podemos fazer seleções usando valores como critérios. Na nossa base, temos o produto "Videira do Campo - 1,5 Litros - Melancia" cujo "PRECO_DE_LISTA" é 19.51. Vamos criar um filtro usando esse valor como critério:

````
SELECT * FROM tabela_de_produtos WHERE PRECO_DE_LISTA = 19.51
````

Ao rodar essa consulta, o MySQL retorna vazio. Mas por que isso acontece, se vimos que existe um produto que corresponde a esse filtro? Ao verificar mais detalhes sobre "PRECO_DE_LISTA", vê-se que é um dado do tipo float. Isso significa que é um ponto flutuante, ou seja, não é exatamente 19.51 mas, sim, um número com muitas casas decimais além das que estamos vendo. Em outras palavras, não corresponde completamente à condição que descrevemos.

- Para solucionar esse problema e filtrar um valor cravado, bem específico, podemos usar os operadores BETWEEN (entre) e AND (e):

````
SELECT * FROM tabela_de_produtos WHERE PRECO_DE_LISTA BETWEEN 19.50 AND 19.52;
````

## Consultas Condicionais

````
SELECT * FROM tabela_de_produtos WHERE SABOR = 'Manga';
````

Ao executar o script, você pode verificar na coluna "SABOR" que todos os registros encontrados têm valor "manga". Então, vamos incrementar nossa consulta, adicionando mais uma expressão à condição:

````
SELECT * FROM tabela_de_produtos WHERE SABOR = 'Manga' OR TAMANHO = '470 ml';
````
![Captura de tela 2023-05-01 164358](https://user-images.githubusercontent.com/104650333/235518417-6cab08a1-c433-44c0-af43-eff9f357a715.png)








