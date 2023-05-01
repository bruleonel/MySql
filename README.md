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

````ruby
SELECT * FROM tabela_de_clientes;
````

![Captura de tela 2023-05-01 162303](https://user-images.githubusercontent.com/104650333/235515185-7a5357c1-4076-4bce-90e7-8cc0fbdd548b.png)

- Para selecionar campos específicos:
````ruby
SELECT CPF, NOME FROM tabela_de_clientes;
````

- Em consultas SQL, existe a opção do uso de alias, que funciona como um apelido que atribuímos a determinado campo. Isso é feito com o uso de as:
````ruby
SELECT CPF as IDENTIFICADOR, NOME as CLIENTE FROM tabela_de_clientes;
````
Nesse caso, "identificador" representa o CPF e "cliente" representa o NOME. Assim, quando o script for executado, notaremos que as colunas do resultado são os aliases e não os nomes originais dos campos (CPF e NOME).

![Captura de tela 2023-05-01 162933](https://user-images.githubusercontent.com/104650333/235516189-a1e6fb1e-0702-4ce4-aac0-3f41d151fade.png)

### A seguir, vamos consultar a "tabela_de_produtos":

````ruby
SELECT * FROM tabela_de_produtos;
````
![Captura de tela 2023-05-01 163135](https://user-images.githubusercontent.com/104650333/235516517-7e5c8f46-edb1-4902-94dc-7ed8696c2413.png)

````ruby
SELECT * FROM tabela_de_produtos WHERE CODIGO_DO_PRODUTO ="1000889";
````

![Captura de tela 2023-05-01 163349](https://user-images.githubusercontent.com/104650333/235516829-b9c23b03-f4b3-415d-8d36-fc047fcaf16f.png)

Essa consulta retorna apenas um produto, pois somente um suco tem sabor uva. Trocando o valor "uva" por "limão", nenhum produto será mostrado, pois não há sucos com esse sabor. Já ao escrever "laranja", são cinco os produtos que atendem a essa condição.

Mas qual é a grande diferença interna na execução da consulta com WHERE CODIGO_DO_PRODUTO = '1000889' e da consulta com WHERE SABOR = 'Uva'? A resposta está na performance!

Buscas com condições de filtro que possuem chaves primárias (como "CODIGO_DO_PRODUTO") são mais rápidas, pois chaves primárias têm índices que facilitam muito esse processo. "SABOR", por outro lado, não é uma chave primária nem estrangeira, logo não tem índice e consequentemente resulta numa busca um pouco mais lenta.

Como nosso banco de dados atual é relativamente pequeno, essa lentidão não é perceptível, porém essa diferença de performance pode ser problemática em bancos mais volumosos. Uma forma de solucionar esse problema é atribuindo um índice à coluna, algo que aprenderemos mais para frente, em outro curso de MySQL.

- Seguindo com as consultas, agora vamos fazer um filtro referente à embalagem:

````ruby
SELECT * FROM tabela_de_produtos WHERE EMBALAGEM = 'PET';
````

![Captura de tela 2023-05-01 163557](https://user-images.githubusercontent.com/104650333/235517168-c5c466df-a52e-4d7a-a194-54467885899c.png)

Ao executar esse script, note que na tabela o valor "PET" está escrito com letras maiúsculas. O que será que acontece se eu fizer a consulta usando letras minúsculas?

````ruby
SELECT * FROM tabela_de_produtos WHERE EMBALAGEM = 'pet';
````

O resultado é o mesmo! Como vimos anteriormente, o MySQL não distingue entre letras maiúsculas e minúsculas, ele fará a busca da mesma forma.

- Também podemos fazer seleções usando valores como critérios. Na nossa base, temos o produto "Videira do Campo - 1,5 Litros - Melancia" cujo "PRECO_DE_LISTA" é 19.51. Vamos criar um filtro usando esse valor como critério:

````ruby
SELECT * FROM tabela_de_produtos WHERE PRECO_DE_LISTA = 19.51
````

Ao rodar essa consulta, o MySQL retorna vazio. Mas por que isso acontece, se vimos que existe um produto que corresponde a esse filtro? Ao verificar mais detalhes sobre "PRECO_DE_LISTA", vê-se que é um dado do tipo float. Isso significa que é um ponto flutuante, ou seja, não é exatamente 19.51 mas, sim, um número com muitas casas decimais além das que estamos vendo. Em outras palavras, não corresponde completamente à condição que descrevemos.

- Para solucionar esse problema e filtrar um valor cravado, bem específico, podemos usar os operadores BETWEEN (entre) e AND (e):

````ruby
SELECT * FROM tabela_de_produtos WHERE PRECO_DE_LISTA BETWEEN 19.50 AND 19.52;
````

## Consultas Condicionais

````ruby
SELECT * FROM tabela_de_produtos WHERE SABOR = 'Manga';
````

Ao executar o script, você pode verificar na coluna "SABOR" que todos os registros encontrados têm valor "manga". Então, vamos incrementar nossa 
consulta, adicionando mais uma expressão à condição:

````ruby
SELECT * FROM tabela_de_produtos WHERE SABOR = 'Manga' OR TAMANHO = '470 ml';
````
![Captura de tela 2023-05-01 164358](https://user-images.githubusercontent.com/104650333/235518417-6cab08a1-c433-44c0-af43-eff9f357a715.png)

Com essa seleção, vamos filtrar apenas os registros que tenham sabor manga ou tamanho de 470 ml (ou até mesmo os dois). Executando o script, podemos 
reparar que o primeiro item do resultado atende às duas expressões; os quatro produtos seguintes têm sabor manga, porém tamanhos diferentes de 470 ml;
e o último registro tem 470 ml, no entanto, é sabor laranja.

- A seguir, criaremos uma consulta com AND:
````ruby
SELECT * FROM tabela_de_produtos WHERE SABOR = 'Manga' AND TAMANHO = '470 ml';
````
Nesse caso, como usamos o AND, o retorno terá apenas um registro - nessa tabela, é o único produto cujo sabor é manga E** o tamanho é igual a 470 ml **ao mesmo tempo.

- Agora, vamos inserir o NOT, para fazer a seleção inversa: uma consulta de todos os registros exceto os que têm sabor manga e** tamanho 470 ml **ao mesmo tempo:
````ruby
SELECT * FROM tabela_de_produtos WHERE NOT (SABOR = 'Manga' AND TAMANHO = '470 ml');
````

- Já se colocarmos o NOT em combinação com OR, o retorno não será tão abrangente:
````ruby
SELECT * FROM tabela_de_produtos WHERE NOT (SABOR = 'Manga' OR TAMANHO = '470 ml');
````
Desse script resulta uma seleção em que não veremos nenhum registro com sabor manga e nenhum registro com tamanho 470 ml.

- Há ainda outras formas de usar o NOT. Podemos, por exemplo, inseri-lo na frente de apenas uma das expressões:
````ruby
SELECT * FROM tabela_de_produtos WHERE SABOR = 'Manga' AND NOT (TAMANHO = '470 ml');
````
Nesse caso, procuraremos itens que tenham sabor manga E** que o tamanho **não seja 470 ml. Isso é, ao rodar o script, na tabela resultante você 
encontrará todos os produtos com sabor manga exceto os que tem tamanho 470 ml - qualquer outro tamanho será apresentado.

- Existem mais condições lógicas além das que expliquei no vídeo anterior. Uma delas é o IN, que pode ser interpretado como "contido":
````ruby
SELECT * FROM tabela_de_produtos WHERE SABOR IN ('Laranja', 'Manga');
````
![Captura de tela 2023-05-01 184926](https://user-images.githubusercontent.com/104650333/235537666-19671a2c-a178-4731-979f-491846061421.png)

Rodando esse script, teremos como resultado uma tabela com todos os clientes cuja cidade consta como Rio de Janeiro ou como São Paulo, e cuja idade 
seja maior ou igual a 20.

- Ademais, há sempre a possibilidade de criar consultas mais complexas:
````ruby
SELECT * FROM tabela_de_clientes WHERE CIDADE IN ('Rio de Janeiro', 'São Paulo') AND (IDADE >= 20 AND IDADE <= 22);
````
![Captura de tela 2023-05-01 185130](https://user-images.githubusercontent.com/104650333/235537922-1c234f64-7076-42df-b240-382574f28cfa.png)


## Like

Vamos aprender mais um comando que filtra informações de uma seleção: o operador LIKE. Normalmente, ele é usado assim:
````ruby
SELECT * FROM tab WHERE campo LIKE '<condição>';COPIAR CÓDIGO
````
Nesse exemplo, "tab" refere-se a uma tabela, e "campo" é a coluna que se está consultando. Após o LIKE, escrevemos o critério de busca entre aspas 
simples. Esse critério deve ser um texto e pode vir acompanhado do símbolo de porcentagem, também chamado de percent (%).

O % é usado para representar qualquer registro genérico que venha antes ou depois do texto que estamos procurando. Ele é como um caractere curinga em 
determinado trecho de uma string, equivalente ao * quando manipulamos arquivos.

Vamos ver na prática para ficar mais claro:
````ruby
SELECT * FROM tabela_de_produtos WHERE SABOR LIKE '%Maça%';
````
![Captura de tela 2023-05-01 185458](https://user-images.githubusercontent.com/104650333/235538404-64969301-50ad-4de1-88b4-f2ebad6be761.png)

Perceba que usamos um percent antes e outro depois do texto que vamos buscar. Ao executar o script, podemos verificar que a seleção retorna produtos com 
dois sabores diferentes: Maçã e Cereja/Maçã. Este último está presente no resultado por causa do primeiro % que colocamos na consulta: há outros 
caracteres antes, mas contém "Maça", que era o nosso critério de busca.

- Vale lembrar que o LIKE pode ser uma parcela de uma expressão mais complexa, é possível combiná-lo com outros operadores, por exemplo:
````ruby
SELECT * FROM tabela_de_produtos WHERE SABOR LIKE '%Maça%' AND
EMBALAGEM = 'PET';
````

![Captura de tela 2023-05-01 185631](https://user-images.githubusercontent.com/104650333/235538591-f7dabe81-b884-4a97-b128-a3367ed99d5b.png)

Ou seja, buscaremos todos os produtos que contêm "Maça" no campo "SABOR" E cuja embalagem é PET.

## Distinct

O comando que vamos aprender é o DISTINCT, que pode ser traduzido como "distinto, diferente". Ele retornará somente linhas com valores diferentes e 
vamos usá-lo depois do SELECT e antes da exibição dos campos.

- Vamos ao MySQL Workbench para testar esse comando na nossa tabela "sucos_vendas". Criaremos um novo script SQL e começaremos com uma seleção sem o DISTINCT:
````ruby
SELECT EMBALAGEM, TAMANHO FROM tabela_de_produtos;
````

![Captura de tela 2023-05-01 190255](https://user-images.githubusercontent.com/104650333/235539469-520e85f8-0ba1-4a5b-8682-47178663fbb2.png)

Essa consulta trata uma série de linhas e num instante é possível perceber que há registros que se repetem. Por exemplo, a 
combinação Garrafa com 700ml (linhas 1 e 3) ou a combinação PET com 2 Litros (linhas 6, 7 e 8).

- No entanto, temos a opção de incluir o DISTINCT para mudar essa situação:
````ruby
SELECT DISTINCT EMBALAGEM, TAMANHO FROM tabela_de_produtos;
````

![Captura de tela 2023-05-01 190606](https://user-images.githubusercontent.com/104650333/235539843-7445f562-23e3-4654-9248-0049fc75efbf.png)

Desse modo, o retorno será bem mais reduzido, porque mostrará apenas as combinações que não se repetem.

- Vale lembrar que podemos aplicar junto com DISTINCTtodas aquelas condições de filtro que aprendemos anteriormente, por exemplo:
````ruby
SELECT DISTINCT EMBALAGEM, TAMANHO FROM tabela_de_produtos WHERE SABOR = 'Laranja';
````

Essa consulta seria útil se, por exemplo, um cliente dessa empresa de sucos perguntasse: "Quais são as embalagens e os tamanhos 
disponíveis para o suco de frutas do sabor laranja?"

Examinando o resultado, poderíamos responder: "O suco de laranja é oferecido em PET de 2 litros, garrafa de 470 ml, PET de 1 
litro, lata de 350 ml e PET de 1,5 litro."

- Vamos ver um último exemplo, incluindo mais um campo à seleção:
````ruby
SELECT DISTINCT EMBALAGEM, TAMANHO, SABOR FROM tabela_de_produtos;
````
Nesse caso, obteremos mais registros do que na consulta anterior, pois com uma coluna a mais ("SABOR") o número de combinações 
aumenta. Observe que as cinco linhas que apareceram na penúltima seleção também estão presentes nessa última consulta, já que 
continuam a atender as condições.


## Limit

Às vezes, criamos seleções que retornam 1 milhão de registros, mas estamos na fase de desenvolvimento de um projeto e não 
queremos, de fato, ver 1 milhão de linhas, o objetivo era saber se a consulta funcionaria e se ela traria os dados esperados. 
Nesses casos, podemos limitar a saída de dados usando o comando LIMIT, que no caso do MySQL estará sempre no final da query, 
por exemplo:

````ruby
SELECT * FROM tabela_de_produtos LIMIT 5;
````
![Captura de tela 2023-05-01 193943](https://user-images.githubusercontent.com/104650333/235543809-86b0cefb-f995-4956-bf47-e9a0dfd2f616.png)

- Já se nosso objetivo for selecionar três linhas a partir do código 1002767, que é o terceiro registro da tabela, faremos:
````ruby
SELECT * FROM tabela_de_produtos LIMIT 2,3;
````
![Captura de tela 2023-05-01 194130](https://user-images.githubusercontent.com/104650333/235544021-289d527c-3de4-44e1-8795-ac02cf0a1f37.png)

- Vale lembrar que o MySQL considera a primeira linha como linha 0, portanto se vamos começar a seleção na linha 3, por isso, 
o primeiro número após o LIMIT será 2. Da mesma forma, se queremos que a seleção se inicie na primeira linha, podemos 
escrever o seguinte:
````ruby
SELECT * FROM tabela_de_produtos LIMIT 0, 2;
````
![Captura de tela 2023-05-01 194400](https://user-images.githubusercontent.com/104650333/235544278-e0493003-0398-4748-b316-8c249d0b233d.png)

## Ordenando a saída da consulta

Quando fazemos uma seleção de dados num banco, eles são exibidos na ordem natural que a informação está armazenada na tabela. 
Mas nós podemos, através do comando ORDER BY, fazer com que o resultado da consulta venha ordenado por determinados critérios. 
Basta especificar o campo pelo qual se deseja organizar os dados, por exemplo:

````ruby
SELECT * FROM tabela_de_produtos ORDER BY PRECO_DE_LISTA;
````
![Captura de tela 2023-05-01 194714](https://user-images.githubusercontent.com/104650333/235544681-8131230d-c5d8-4875-9534-3cbf2790e7a4.png)
Verificando o resultado, notaremos que os registros estão ordenados conforme a ordem crescente da coluna "PRECO_DE_LISTA", começando no valor R$2,808 e indo até R$38,012.

- Para mudar a direção da ordenação, vamos inserir o comando DESC na nossa consulta, depois do nome do campo:
````ruby
SELECT * FROM tabela_de_produtos ORDER BY PRECO_DE_LISTA DESC;
````
Dessa vez, os registros aparecerão de acordo com a ordem descendente da coluna "PRECO_DE_LISTA", do R$38,012 ao R$2,808.

- A seguir, faremos uma seleção nessa mesma tabela, porém ordenando pelo campo "NOME_DO_PRODUTO", que tem dados em formato de texto:
````ruby
SELECT * FROM tabela_de_produtos ORDER BY NOME_DO_PRODUTO;
````
![Captura de tela 2023-05-01 194924](https://user-images.githubusercontent.com/104650333/235544883-f2d3a5ca-7587-4eb1-97a7-a9eec9a5e6a4.png)

O resultado estará ordenado pela ordem alfabética dos nomes dos produtos. 

- Caso nosso objetivo seja ver na ordem contrária, precisaremos acrescentar o comando DESC:
````ruby
SELECT * FROM tabela_de_produtos ORDER BY NOME_DO_PRODUTO DESC;
````

- Por fim, vamos fazer um teste usando um critério composto:
````ruby
SELECT * FROM tabela_de_produtos ORDER BY EMBALAGEM, NOME_DO_PRODUTO;
````
![Captura de tela 2023-05-01 195118](https://user-images.githubusercontent.com/104650333/235545069-fcac50e2-3e1f-442d-b281-3bce0194318a.png)

Sabemos que existem três tipos de embalagem no nosso banco: garrafa, lata e PET. Executando a consulta, obteremos um resultado que 
primeiramente respeitará à ordem crescente (alfabética) do campo "EMBALAGEM", começando portanto por "GARRAFA". Dentre os registros 
cuja embalagem é garrafa, teremos a ordem crescente pelo campo "NOME_DO_PRODUTO" (nosso segundo critério). Só depois poderemos ver 
registros com embalagem "LATA" (também em ordem alfabética dos nomes dos produtos) e, em seguida, "PET".

- É possível deixar essa consulta ainda mais específica, acrescentando a direção da ordenação que queremos para cada um dos campos:
````ruby
SELECT * FROM tabela_de_produtos ORDER BY EMBALAGEM DESC, NOME_DO_PRODUTO ASC;
````
![Captura de tela 2023-05-01 195258](https://user-images.githubusercontent.com/104650333/235545216-d50d423a-cd36-4ddc-9f52-ac2c33005e6e.png)

Dessa vez, porque usamos DESC para o primeiro critério, a ordem das embalagens começará do maior para o menor (no caso, de "PET" 
a "GARRAFA") e, dentre os itens de cada tipo de embalagem, os nomes dos produtos estarão organizados em ordem alfabética, pois 
usamos o ASC para o segundo critério, "NOME_DO_PRODUTO".

## Agurpando os Resultados

No vídeo anterior, aprendemos como ordenar resultados. Agora, vamos estudar como agrupá-los. Agrupar é juntar campos que são repetidos 
e, nos casos de campos numéricos, em meio a essa junção temos a opção de aplicar fórmulas matemáticas, que podem ser de soma, de média, 
de máximo ou mínimo valor, entre outros.

- Então, vamos ao MySQL Workbench criar alguns exemplos na base "sucos_vendas". Criaremos um novo script e começaremos consultando toda 
a tabela de clientes:

````ruby
SELECT * FROM tabela_de_clientes;
````

- Em seguida, vamos restringir um pouco essa consulta, selecionando apenas o estado e o limite de crédito na tabela

````ruby
SELECT ESTADO, LIMITE_DE_CREDITO FROM tabela_de_clientes;
````
Ao fazer essa consulta, veremos uma lista em que cada linha mostra o estado e o limite de crédito de um cliente.

- Se nosso objetivo for saber o total de limite de crédito de cada estado, usaremos o GROUP BY:

````ruby
SELECT ESTADO, SUM(LIMITE_DE_CREDITO) as LIMITE_TOTAL FROM tabela_de_clientes GROUP BY ESTADO;
````
![Captura de tela 2023-05-01 200037](https://user-images.githubusercontent.com/104650333/235546052-58a2dca9-565b-4d75-aba9-43705c0daa9e.png)

Sempre que uma fórmula for usada, é necessário usar um alias ("apelido") para o campo. No nosso caso, definimos 
"LIMITE_TOTAL" como alias da soma dos limites de crédito.

O retorno mostrará os limites de crédito somados agrupados por estado: em São Paulo, o limite total é R$810.000,00 
e, no Rio de Janeiro, é R$995.000,00.

- Faremos, agora, uma consulta relativa às embalagens e aos preços de lista presentes na tabela de produtos:

````ruby
SELECT EMBALAGEM, PRECO_DE_LISTA FROM tabela_de_produtos;
````

- Vamos supor que precisamos descobrir qual é o preço mais caro de cada tipo de embalagem (PET, garrafa e lata):

````ruby
SELECT EMBALAGEM, MAX(PRECO_DE_LISTA) as MAIOR_PRECO FROM tabela_de_produtos GROUP BY EMBALAGEM;
````

![Captura de tela 2023-05-01 201805](https://user-images.githubusercontent.com/104650333/235547722-6013124f-302a-4a22-8139-8fa1c7cd6cd2.png)

Com essa consulta, constatamos que o produto mais caro que vem em garrafas tem o valor de R$13,312. O mais caro com embalagem PET é R$38,012. 
E o de lata custa R$4,56.

- Além disso, é possível criar seleções com o comando COUNT:

````ruby
SELECT EMBALAGEM, COUNT(*) as CONTADOR FROM tabela_de_produtos GROUP BY EMBALAGEM;
````

![Captura de tela 2023-05-01 201945](https://user-images.githubusercontent.com/104650333/235547880-9b2424b0-7996-4edc-865e-a0c051e7815b.png)

O retorno nos mostrará a quantidade de produtos que existem com cada tipo de embalagem: 11 tem embalagem garrafa, 15 vem em PET e 5 em lata.

- Vale lembrar que podemos aplicar critérios de filtro juntamente do ORDER BYe do GROUP BY. Como exemplo, primeiramente vamos selecionar 
os limites de crédito agrupados por bairro:

````ruby
SELECT BAIRRO, SUM(LIMITE_DE_CREDITO) as LIMITE FROM tabela_de_clientes GROUP BY BAIRRO;
````

![Captura de tela 2023-05-01 202131](https://user-images.githubusercontent.com/104650333/235548037-38e095bf-6a40-4600-8c8d-09d8bec49339.png)

- E, para filtrar a consulta, usaremos uma cláusula WHERE para ver apenas os limites de crédito dos bairros da cidade do Rio de Janeiro:

````ruby
SELECT BAIRRO, SUM(LIMITE_DE_CREDITO) as LIMITE FROM tabela_de_clientes WHERE CIDADE = 'Rio de Janeiro' GROUP BY BAIRRO;
````

![Captura de tela 2023-05-01 202318](https://user-images.githubusercontent.com/104650333/235548208-dbea2306-7901-47cd-b996-c1dca71a1b61.png)


- Ademais, é possível usar mais de um campo no GROUP BY:

````ruby
SELECT ESTADO, BAIRRO, SUM(LIMITE_DE_CREDITO) as LIMITE FROM tabela_de_clientes GROUP BY ESTADO, BAIRRO;
````

![image](https://user-images.githubusercontent.com/104650333/235548327-6179c710-2937-46cf-a6c0-a08a4668ed05.png)

Note que adicionamos o campo "ESTADO" no início da seleção (SELECT ESTADO) e também no fim, depois de GROUP BY. Na primeira ocorrência, 
estamos determinando como exibiremos os dados, já na segunda indicamos como queremos que sejam agrupados.

- Em seguida, aplicaremos um filtro que irá restringir a consulta somente à cidade do Rio de Janeiro:

````ruby
SELECT ESTADO, BAIRRO, SUM(LIMITE_DE_CREDITO) as LIMITE FROM tabela_de_clientes WHERE CIDADE = 'Rio de Janeiro' GROUP BY ESTADO, BAIRRO;
````

![image](https://user-images.githubusercontent.com/104650333/235548471-4c95d9e1-6b62-4468-bb1f-eb98d33e3f7b.png)

Ou seja, estamos selecionando estado, bairro e a soma dos limites de crédito somente da cidade do Rio de Janeiro, agrupando esses dados por estado e bairro.

- E, por fim, se nossa meta for visualizar esse resultado de forma ordenada, podemos ainda incluir o ORDER BY:

```ruby
SELECT ESTADO, BAIRRO, SUM(LIMITE_DE_CREDITO) as LIMITE FROM tabela_de_clientes 
WHERE CIDADE = 'Rio de Janeiro' 
GROUP BY ESTADO, BAIRRO 
ORDER BY BAIRRO;
````

![image](https://user-images.githubusercontent.com/104650333/235548647-893ffb09-f022-4b0c-8c7b-79a895630e93.png)

Dessa forma, veremos que o retorno respeitará a ordem alfabética dos bairros, começando por Água Santa, Barra da Tijuca, Cidade Nova e assim por 
diante. Essa última consulta é mais complexa, pois estamos agrupando, filtrando e ordenando dados em uma única seleção.

