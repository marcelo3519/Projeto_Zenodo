## **Integração do Banco de Dados MySQL e linguagem Python.** ##
>Introdução

Este trabalho oferece uma visão abrangente sobre o MySQL, um sistema de gerenciamento de banco de dados relacional de código aberto amplamente utilizado em aplicações web. Desde sua criação em 1995, o MySQL tem sido uma escolha popular entre os desenvolvedores devido à sua confiabilidade, desempenho e flexibilidade. Capaz de lidar com grandes volumes de dados e oferecer acesso rápido, o MySQL tornou-se fundamental para muitos sistemas dinâmicos na web. Além disso, o texto aborda a linguagem de programação Python, escolhida por sua simplicidade, vasta biblioteca padrão e comunidade ativa, Python é amplamente adotada em diferentes setores da indústria.
Por fim, o texto destaca a integração entre MySQL e Python usando o MySQL Connector/Python. Este conector proporciona uma integração direta e eficiente entre as duas tecnologias, garantindo desempenho otimizado e segurança nos dados. Com uma API amigável, facilita a execução de consultas e atualizações no banco de dados. Mantido ativamente pela comunidade, o MySQL Connector/Python é compatível com várias versões do MySQL, tornando-se uma escolha confiável para o desenvolvimento de aplicativos robustos.

>Pesquisa

<div style="text-align: justify; font-size: 18px; margin: 10px;">
<p> 
  Um banco de dados é uma coleção organizada de dados estruturados que são armazenados eletronicamente em um sistema de computador. Ele é projetado para permitir o armazenamento, recuperação, manipulação e gerenciamento eficiente desses dados, permitindo que usuários e aplicativos acessem e trabalhem com as informações de forma fácil e rápida.
<p></p>

 
<div style="text-align: justify; font-size: 18px; margin: 10px;">
<p> 
	
1. Armazenamento de Dados: Capacidade de armazenar grandes volumes de dados de forma estruturada, seguindo um modelo de dados específico.<p></p>
2. Recuperação de Dados: Capacidade de recuperar dados de forma eficiente por meio de consultas, permitindo que os usuários obtenham informações específicas conforme necessário.<p></p>
3. Gerenciamento de Transações**: Suporte para transações que garantem a integridade e consistência dos dados, permitindo operações como inserção, atualização e exclusão de registros.<p></p>
4. Concorrência: Habilidade de lidar com múltiplos usuários acessando e manipulando os dados simultaneamente de forma segura e eficiente.<p></p>
5. Controle de Acesso: Implementação de mecanismos de segurança para controlar o acesso aos dados, garantindo que apenas usuários autorizados possam visualizar e modificar informações sensíveis.<p></p>
6. Backup e Recuperação: Capacidade de realizar backups regulares dos dados armazenados e restaurá-los em caso de falhas no sistema ou perda de dados.<p></p>
7. Integridade Referencial: Suporte para garantir a integridade referencial entre diferentes conjuntos de dados por meio de chaves estrangeiras e restrições de integridade.<p></p>
8. Indexação e Otimização: Uso de índices para acelerar a recuperação de dados e otimizar o desempenho das consultas, especialmente em grandes conjuntos de dados.<p></p>
9. Suporte a Transações ACID: Implementação dos princípios ACID (Atomicidade, Consistência, Isolamento e Durabilidade) para garantir que as transações sejam executadas de forma confiável e segura.<p></p>
10. Escalabilidade: Capacidade de expandir o banco de dados conforme necessário para lidar com um aumento na quantidade de dados ou na carga de trabalho, sem comprometer o desempenho ou a disponibilidade. <p></p>

Os principais recursos de um banco de dados incluem:

Os bancos de dados servem vários propósitos e desempenham um papel central em muitos sistemas de informação. Aqui estão alguns dos principais objetivos de um banco de dados:
• Armazenamento de dados;<p></p>
• Recuperação de dados e ciente;<p></p>
• Integridade de dados; <p></p>
• Controle de concorrência (acesso);<p></p>
• Segurança de dados;<p></p>
• Redundância e backup;<p></p>
• Entre outros.<p></p>

Esses são os principais recursos essenciais de um banco de dados moderno, que garantem eficiência, segurança e confiabilidade no armazenamento e gerenciamento de dados.
<p></p>


## **MYSQL** ##
>História 	


<div style="text-align: justify; font-size: 18px; margin: 10px;">
<p> 
 O MySQL é um sistema de gerenciamento de banco de dados relacional (SGBDR) que teve sua origem em meados da década de 1990. Sua história remonta a uma empresa sueca chamada MySQL AB, fundada em 1995 por David Axmark, Allan Larsson e Michael "Monty" Widenius. O nome "MySQL" é derivado do nome de Monty, filho de Michael Widenius.

O desenvolvimento inicial do MySQL foi impulsionado pela necessidade de um banco de dados leve, rápido e acessível para uso em aplicativos web. Inicialmente, o MySQL foi desenvolvido como um projeto de código aberto, tornando-se uma escolha popular entre desenvolvedores e empresas devido à sua simplicidade, desempenho e custo zero.

Ao longo dos anos, o MySQL ganhou destaque como um dos SGBDR mais populares e amplamente utilizados do mundo. Ele foi adotado por uma vasta gama de organizações, desde pequenas empresas até grandes corporações e provedores de serviços de internet.

Em 2008, a MySQL AB foi adquirida pela Sun Microsystems por cerca de US$ 1 bilhão, aumentando ainda mais a visibilidade e o suporte ao MySQL. No entanto, em 2010, a Sun Microsystems foi adquirida pela Oracle Corporation, levantando preocupações sobre o futuro do MySQL devido à concorrência direta com o banco de dados Oracle.

Apesar das preocupações iniciais, o MySQL continuou sendo desenvolvido ativamente como um projeto de código aberto. A Oracle Corporation oferece várias edições comerciais do MySQL, juntamente com suporte e serviços adicionais. Além disso, a comunidade de código aberto em torno do MySQL permanece vibrante, contribuindo para o seu desenvolvimento contínuo.

Ao longo dos anos, o MySQL passou por várias versões e atualizações, introduzindo novos recursos, melhorias de desempenho e suporte a padrões emergentes. Em 2021, a versão mais recente do MySQL é a MySQL 8.0, que continua a ser uma escolha popular para muitos desenvolvedores e organizações em todo o mundo.
<p></p>


## **Instalação MySQL** ##
>MySQL

<div style="text-align: justify; font-size: 18px; margin: 10px;">
  A Linguagem de Consulta Estruturada (Structured Query Language), ou SQL, conhecida no mercado como linguagem de consulta, é usada para manipular bancos de dados relacionais, como MySQL, SQL Server, Oracle, entre outros. O SQL não se limita apenas a consultas; também inclui recursos para definir a estrutura de dados, modificar dados e especificar restrições de segurança.
	
Os recursos do SQL são divididos em cinco partes:

• DDL (Linguagem de Definição de Dados): Para definir a estrutura do banco de dados.<p></p>
• DML (Linguagem de Manipulação de Dados): Para modificar dados no banco de dados.<p></p>
• DQL (Linguagem de Consulta de Dados): Para consultar dados.<p></p>

Além disso, há o DCL (Linguagem de Controle de Dados) para especificar restrições de segurança e o DTL (Linguagem de Transação de Dados) para operações de transação.
 <p></p>

**Instalação**

Para instalar o banco de dados **MySQL**, acesse o site oficial do **MySQL** e baixe o software adequado para sua arquitetura (**32** ou **64** bits). Durante a instalação, escolha a opção "**Developer Default**"

<p align="center">
  <img width="500" height="400" src="https://github.com/roneycsilva/zenodo/assets/61150519/6c15fa7c-50d2-4d1d-9611-f4d30eaa49ee" alt="Descrição da imagem">
</p>

<p align="center" style="font-size: 18px; margin: 10px;">Figura 1. Opção selecionada "Developer Default" e botão "Next".</p>


<div style="text-align: justify; font-size: 18px; margin: 10px;">
  Após a instalação dos componentes, ao configurar o MySQL, certifique-se de marcar a opção <strong><em>"Enable TCP/IP Networking"</em></strong>  e definir a porta como 3306.
 <p></p>
<p align="center">
  <img width="500" height="400" src="https://github.com/roneycsilva/zenodo/assets/61150519/ea8d9959-350e-46d6-92df-c757408321d7" alt="Descrição da imagem">
</p>
<p align="center" style="font-size: 18px; margin: 10px;">Figura 2. Escolha das opções demarcadas e botão “Next”.</p>
<div style="text-align: justify; font-size: 18px; margin: 10px;">
Em seguida aparecerá a tela de inserção dos dados de login do usuário root, como mostra a Figura 3.
 <p></p>
<p align="center">
  <img width="500" height="400" src="https://github.com/roneycsilva/zenodo/assets/61150519/e443b0a1-5b28-4063-82cd-d2fe16171267" alt="Descrição da imagem">
</p>
<p align="center" style="font-size: 18px; margin: 10px;">Figura 3. Definição de senha e botão “Next”.</p>

<div style="text-align: justify; font-size: 18px; margin: 10px;">
Na etapa seguinte, é solicitado que você defina o nome do seu servidor. Ao prosseguir com mais alguns cliques em <strong><em>next</em></strong>, a instalação do <strong><em>MySQL</em></strong> é concluída. <p></p>
Existem duas maneiras de utilizá-lo: através do <strong><em>MySql 5.6 Command Line Client</em></strong>, que se assemelha ao terminal do MS-DOS, ou pela ferramenta <strong><em>MySQL Workbench</em></strong>, que oferece uma interface gráfica e visual para gerenciar o <strong><em>MySQL</em></strong>. <p></p>
</div>

<p align="center">
  <img width="550" height="400" src="https://github.com/roneycsilva/zenodo/assets/61150519/7ebdb902-3f43-4f89-88f9-65311c44cf4b" alt="Descrição da imagem">
</p>
<p align="center" style="font-size: 18px; margin: 10px;">Figura 4. Aparência do MySQL 5.6 Command Line Client..</p>
<p align="center">
  <img width="600" height="400" src="https://github.com/roneycsilva/zenodo/assets/61150519/9b85fbe3-8527-412d-b354-61eae23b5f95" alt="Descrição da imagem">
</p>
<p align="center" style="font-size: 18px; margin: 10px;">Figura 5. Aparência do MySQL 5.6 Workbench.</p>

## **Utilizando o MySQL Workbench**<p></p> ##
>MySQL Workbench

<div style="text-align: justify; font-size: 18px; margin: 10px;">
Para começarmos a trabalhar, vamos nos conectar a nossa DataBase usando a ferramenta gráfica. Para isso, acesse o menu “DataBase” e clique na opção “Connect to Database...”. Use as configurações padrão vistas na <strong><em>Figura 7</em></strong>.
	<p></p>

<p align="center">
  <img width="550" height="400" src="https://github.com/roneycsilva/zenodo/assets/61150519/d9921289-670c-41bc-84b6-ce4959cdd6bd" alt="Descrição da imagem">
</p>
<p align="center" style="font-size: 18px; margin: 10px;">Figura 6. Acessando o menu “Database”.</p>
<p align="center">
  <img width="600" height="400" src="https://github.com/roneycsilva/zenodo/assets/61150519/f41c4c7e-7555-4772-87a8-31fe0bfff7da" alt="Descrição da imagem">
</p>
<p align="center" style="font-size: 18px; margin: 10px;">Figura 7. Configurações. </p>


**Linguagem de Definição de Dados (DDL)**<p></p>
 
<div style="text-align: justify; font-size: 18px; margin: 10px;">
Ao criarmos banco de dados com as tabelas explicitando seus tipos de dados a cada campo, sua(s) <strong><em>chave</em></strong> (s) <strong><em>primária</em></strong> (s) e <strong><em>estrangeiras</em></strong>, <strong><em>índices</em></strong>, <strong><em>regras</em></strong> e etc.
Para isso, a criação e alteração de estruturas definem como os dados serão armazenados. Logo, quando falamos de comando do tipo DDL estamos nos referindo a comandos do tipo <strong><em>CREATE</em></strong>, <strong><em>ALTER</em></strong> e <strong><em>DROP</em></strong> (criar, alterar e excluir, respectivamente). <p></p>
</div>

Para criar o banco de dados **DBDevMedia** utilizaremos a sintaxe **CREATE**, conforme o código a seguir:
```c
1| CREATE DATABASE DBDevMedia;
```
> Ao executá-lo teremos o mesmo resultado da Figura 8.

<p align="center">
  <img width="550" height="400" src="https://github.com/roneycsilva/zenodo/assets/61150519/b2429f78-7a3b-471c-a665-2817c513827f" alt="Descrição da imagem">
</p>
<p align="center" style="font-size: 18px; margin: 10px;">Figura 8. Criando o banco de dados.</p>
<p align="center">

 <div style="text-align: justify; font-size: 18px; margin: 10px;">
Podemos complementar o nosso código com a sintaxe opcional <strong><em>IF NOT EXISTS</em></strong>, que permite ao  <strong><em>MySQL</em></strong>verificar <strong><em>se o nome escolhido esteja sendo utilizando no servidor</em></strong>, evitando que retorne um erro com a possível existência de dois bancos com o mesmo nome em um mesmo <strong><em>servidor MySQL:</em></strong> <p></p>
</div>

```C
1| CREATE DATABASE IF NOT EXISTS DBDevMedia;
```
Para visualizar uma lista com todos os bancos de dados existentes no servidor, use o comando:
```C
SHOW DATABASES;
```

 <div style="text-align: justify; font-size: 18px; margin: 10px;">
Observe que todos os <strong><em>comandos em MySQL</em></strong> sempre termina com “;” no final. Essa sintaxe é obrigatória para que o MySQL possa entender o termino do comando.
Para remover os bancos de dados existentes no servidor, utilize o comando a seguir, mas atenção, pois uma vez executado, a ação é irreversível (Figura 9): <p></p>
</div>

```c
DROP DATABASE DBDevMedia;
```

<p align="center">
  <img width="550" height="400" src="https://github.com/roneycsilva/zenodo/assets/61150519/072236f4-5ca8-4d3b-9b55-f3033f7ffa1c" alt="Descrição da imagem">
</p>
<p align="center" style="font-size: 18px; margin: 10px;">Figura 9. Removendo o banco de dados.</p>

**Criando tabelas no MySQL**

 <div style="text-align: justify; font-size: 18px; margin: 10px;">
Dada a grande quantidade de parâmetros aceitos, a declaração <strong><em>CREATE TABLE</em></strong> é uma das mais complexas no <strong><em>MySQL</em></strong>.
Selecione o banco de dados que ganhará a nova tabela usando a sintaxe: <p></p>
</div>

```C
USE DBDevMedia;
```
De acordo com a documentação disponível pela **Oracle**, a sintaxe simplificada seria:
```C
CREATE [TEMPORARY] TABLE [IF NOT EXISTS] tbl_name
(create_definition, ...)
```
A parte de declaração que se encontra entre colchetes é opcional:
• **TEMPORARY**: Indica que a tabela criada será temporária, ou seja, ela expira assim que sua sessão no MySQL terminar. Use-a sempre que estiver fazendo testes.
• **IF NOT EXISTS**: Verifica a prévia existência da tabela e evita uma interrupção do script causada por erro. Como o **MySQL** é case sensitive, tabelas com nomes iguais, mas usando letras em caixa alta, como em **tbl_name** e **Tbl_name**, são consideradas tabelas totalmente diferentes.

>Uma tabela é composta por uma ou mais colunas, cada qual com suas definições.

Criando uma agenda telefônica. A tabela contatos terá a seguinte estrutura da Listagem 1.

```C
Listagem 1. Tabela Contatos
CREATE TABLE contatos (
        nome VARCHAR(50) NOT NULL,
        telefone VARCHAR(25) NOT NULL
        );
```
Para verificar se a tabela foi criada use o comando:
```C
SHOW TABLES;
```
<p align="center">
  <img width="550" height="400" src="https://github.com/roneycsilva/zenodo/assets/61150519/874be11f-70f4-4c46-9cc1-f3f90fdb3455" alt="Descrição da imagem">
</p>
<p align="center" style="font-size: 18px; margin: 10px;">Figura 10. Listando tabelas existentes.</p>

<div style="text-align: justify; font-size: 18px; margin: 10px;">
Podemos melhorar um pouco mais a tabela contatos, ao acrescentar mais alguns campos, como sobrenome dos contatos, DDD, data de nascimento e e-mail. Antes de criar uma nova tabela, com o mesmo nome, vamos remover a anterior usando o comando: <p></p>
</div>

```C
DROP TABLE contatos;
```
Agora, vamos criar a nova tabela, conforme a **Listagem 2**.

```C
CREATE TABLE IF NOT EXISTS contatos (
nome VARCHAR(20) NOT NULL,
sobrenome VARCHAR(30) NOT NULL,
ddd INT(2) NOT NULL,
telefone VARCHAR(9) NOT NULL,
data_nasc DATE NULL,
email VARCHAR(30) NULL);
```
<p align="center" style="font-size: 18px; margin: 10px;">Listagem 2. Tabela contatos</p>


 <div style="text-align: justify; font-size: 18px; margin: 10px;">
A chave primária é o que torna a linha ou o registro de uma tabela único. Geralmente, é utilizada uma sequência automática para a geração dessa chave para que ela não venha a se repetir. Nosso caso, o <strong><em>nro_contato</em></strong> será único, com uma sequência numérica que identificará o registro. <p></p>
A cláusula <strong><em>>auto_increment</em></strong é utilizada para incrementar automaticamente o valor da chave primária. Por padrão, essa cláusula inicia com 1. Porém, se houver a necessidade de iniciar por outro valor, podemos fazer como no exemplo a seguir: <p></p>
</div>

```C
CREATE TABLE contatos AUTO_INCREMENT=100;
```

**ALTER TABLE**

 <div style="text-align: justify; font-size: 18px; margin: 10px;">
Imagine que sua tabela já contenha dados armazenados e você precisa acrescentar mais um campo <strong><em>(chamado Ativo)</em></strong> na tabela de contatos.
Conhecidamente pensaríamos em usar o <strong><em>drop table</em></strong> para excluir a tabela e recriá-la com o novo campo, mas perder os dados é algo inviável.
A solução é utilizar a sintaxe <strong><em>ALTER TABLE</em></strong>, que permite alterar a estrutura da tabela existente. Por exemplo, você pode adicionar ou deletar colunas, criar ou remover índices, alterar o tipo de coluna existentes, ou renomear coluna ou tabelas. Você também pode alterar o comentário para a tabela e tipo de tabela.
Para adicionar colunas use o comando <strong><em>ADD</em></strong>, seguido do nome e dos atributos da coluna que será adicionada e, da sua posição dentro da tabela com o auxílio do parâmetro <strong><em>AFTER</em></strong>. Assim, para adicionarmos a coluna ativo, usaremos o código a seguir: <p></p>
</div>

```C
ALTER TABLE contatos
ADD ativo SMALLINT NOT NULL AFTER email;
```

Para ver o resultado das alterações, dê o comando:

```C
DESCRIBE contatos;
```

 <div style="text-align: justify; font-size: 18px; margin: 10px;">
Para alterar os atributos e nome de colunas usamos o parâmetro <strong><em>CHANGE</em></strong>, seguido da denominação da coluna a ser alterada e dos novos atributos. Para mudar os atributos da coluna nome, utilizaremos a seguinte sintaxe: <p></p>
</div>

```C
ALTER TABLE contatos
CHANGE telefone telefone CHAR(9) NOT NULL;
```

 <div style="text-align: justify; font-size: 18px; margin: 10px;">
Percebe-se que a palavra <strong><em>"telefone"</em></strong>

Vocês devem ter percebido que a palavra “telefone” foi utilizada duas vezes. Isso ocorre porque se indica primeiro a coluna e depois seus novos atributos, e o nome da coluna é um de seus atributos. Para mudar o nome da coluna e manter seus demais atributos usamos a sintaxe a seguir: <p></p>
</div>

```C
ALTER TABLE contatos
CHANGE telefone fone VARCHAR(9) NOT NULL;
```

**Linguagem de Manipulação de Dados (DML) e Linguagem de Transação de Dados (DTL)**
>Inserindo registros

Com as tabela pronta precisamos agora de registros em nosso banco de dados, neste caso diretamente <strong><em>SGBD</em></strong> através de comando SQL.
Vamos fazer o primeiro <strong><em>INSERT</em></strong> na tabela contatos com o comando <strong><em>INSERT INTO</em></strong> contatos. Entre parênteses informaremos em quais colunas queremos inserir os registros e depois devemos informar qual o valor para cada coluna.


```C
INSERT INTO contatos (nome
,sobrenome
,ddd
,telefone
,data_nasc
,email
,ativo)
VALUES(‘Bruno’
,‘Santos’
,11
,999999999
,‘2015-08-22’
,‘contato@dominio.com.br’
,1);
```

Pode inserir em todos os campos da tabela, não é necessário descrever quais serão populados, apenas não se esquecer de conferir se os valores estão na sequência correta, como podemos ver na <strong><em>"Listagem 04"</em></strong> onde omitimos estes campos. O <strong><em>SGBD</em></strong> subentende que todos os campos serão populados.

```C
INSERT INTO contatos VALUES(‘Bruno’
,‘Santos’
,11
,999999999
,‘2015-08-22’
,‘contato@dominio.com.br’
,1);
```
<p align="center" style="font-size: 18px; margin: 10px;">Listagem 4. Inserindo dados sem descrever</p>

Podemos obserrvar que em nenhum momento foi mencionado o campo <strong><em>"nro_contato 04"</em></strong> ou acrescentado um valor diretamente, isso por que este campo foi definido como <strong><em>auto_increment</em></strong>, desta forma, o campo recebe o valor automaticamente.

**Alterando registros** 

 <div style="text-align: justify; font-size: 18px; margin: 10px;">
Para alterar os registros usamos o comando <strong><em>UPDATE</em></strong>.
No exemplo anterior inserimos um sobrenome errado. Para corrigir usamos a sintaxe da Listagem 5. <p></p>
</div>

```C
UPDATE contatos SET
sobrenome= ‘Nascimento’ WHERE nro_contato= 100;
commit;
```
<p align="center" style="font-size: 18px; margin: 10px;">Listagem 5. Alterando dados </p>

Podemos atualizar mais de um campo de uma vez só, separando com “,”, como mostra a Listagem 6.

```C
UPDATE contatos SET
sobrenome= ‘Nascimento’
, ddd= 015
, telefone= ‘0123456789’
WHERE nro_contato = 100
commit;
```
<p align="center" style="font-size: 18px; margin: 10px;">Listagem 6. Alterando mais de um dado</p>

 <div style="text-align: justify; font-size: 18px; margin: 10px;">
Note que, além do UPDATE utilizamos o <strong><em>SET</em></strong> para informar qual campo que queremos alterar. O <strong><em>WHERE</em></strong> indica a condição para fazer a alteração e, em seguida, o commit diz ao SGBD que ele pode realmente salvar a alteração do registro. Se, por engano, fizermos o <strong><em>UPDATE</em></strong> incorreto, antes do <strong><em>commit</em></strong> podemos reverter a situação usando a instrução <strong><em>SQL rollback</em></strong>, da seguinte e maneira: <p></p>
</div>

```C
UPDATE contatos SET
sobrenome= ‘Nascimento’ WHERE nro_contato= 100;
rollback;
```
 <div style="text-align: justify; font-size: 18px; margin: 10px;">
Note que, além do UPDATE utilizamos o <strong><em>SET</em></strong> para informar qual campo que queremos alterar. O <strong><em>WHERE</em></strong> indica a condição para fazer a alteração e, em seguida, o commit diz ao SGBD que ele pode realmente salvar a alteração do registro. Se, por engano, fizermos o <strong><em>UPDATE</em></strong> incorreto, antes do <strong><em>commit</em></strong> podemos reverter a situação usando a instrução <strong><em>SQL rollback</em></strong>, da seguinte e maneira: <p></p>

 <div style="text-align: justify; font-size: 18px; margin: 10px;">
O <strong><em>SGBD</em></strong> vai reverter a última instrução. Porém, se tiver a intenção de utilizar o <strong><em>rollback</em></strong>, faça-o antes de aplicar o <strong><em>commit</em></strong>, pois se você aplicar o <strong><em>UPDATE</em></strong> ou qualquer outro comando que necessite do <strong><em>commit</em></strong>, não será possível reverter.
As instruções commit e <strong><em>rollback</em></strong> são tratadas pela <strong><em>Linguagem de Transação de Dados (DTL)</em></strong>. <p></p>
	 
**Excluindo registros**

<div style="text-align: justify; font-size: 18px; margin: 10px;">
Para deletar algum registo usamos a Instrução <strong><em>DELETE</em></strong> e <strong><em>DROP</em></strong>
Explicação de cada uma:<p></p>

. O DROP é usado para excluir objetos do banco, como tabelas, colunas, views e procedures <p></p>
. O delete deletará os registros das tabelas, podendo excluir apenas uma linha ou todos os registros.<p></p>

```C
DELETE FROM contatos WHERE nro_contato= 100;
commit;
```

Para deletar todos os registros da tabela de clientes usamos o comando:

```C
DELETE FROM contatos;
commit;
```
<div style="text-align: justify; font-size: 18px; margin: 10px;">
Observe que, ao empregar o <strong><em>DELETE</em></strong> você também deve usar o <strong><em>commit</em></strong> logo após a instrução. Da mesma maneira, podemos também utilizar o <strong><em>rollback</em></strong> para não efetivar uma exclusão de dados incorretos.
Além do <strong><em>DELETE</em></strong>, podemos eliminar os dados usando a instrução <strong><em>SQL TRUNCATE</em></strong>, que não necessita de <strong><em>commit</em></strong>. Nem o <strong><em>rollback</em></strong> pode reverter à operação.
Isso ocorre porque, quando você utiliza o <strong><em>DELETE</em></strong>, o <strong><em>SGBD</em></strong> salva os seus dados em uma tabela temporária e, quando aplicamos o <strong><em>rollback</em></strong>, ele a consulta e restaura os dados. Já o <strong><em>TRUNCATE</em></strong> não a utiliza, o <strong><em>SGBD</em></strong> faz a eliminação direta. Para usar esse comando utilizar a sintaxe a seguir: <p></p>

```C
TRUNCATE TABLE contatos;
```

>Essa instrução não pode ser usada dentro da cláusula **WHERE**.

**Linguagem de Consulta de Dados (DQL)**

<div style="text-align: justify; font-size: 18px; margin: 10px;">
O objetivo de armazenar registros em um banco de dados é a possibilidade de recuperar e utilizá-los em relatórios para análises mais profundas. Essa recuperação é feita através de consultas. O comando <strong><em>SQL</em></strong>  utilizado para fazer consultas é o <strong><em>SELECT</em></strong>. Selecionando os dados, devemos dizer ao <strong><em>SGBD</em></strong> de onde queremos selecionar, através do comando <strong><em>FROM</em></strong>.
Como exemplo, vamos selecionar os registros da tabela de contato. Quando não queremos selecionar um ou vários campos específicos, utilizamos o asterisco <strong><em>(*)</em></strong>: <p></p>

```C
SELECT * FROM contatos;
```

<p align="center">
  <img width="550" height="400" src="https://github.com/roneycsilva/zenodo/assets/61150519/4ee2492e-e0d1-46e6-8421-7cd82e0c5bc4" alt="Descrição da imagem">
</p>
<p align="center" style="font-size: 18px; margin: 10px;">Figura 11. Consultando contatos.</p>

 
Se quisermos selecionar os registros dos campos nome e sobrenome, usamos a sintaxe:

```C
SELECT nome, sobrenome FROM contatos;
```

<p align="center">
  <img width="550" height="400" src="https://github.com/roneycsilva/zenodo/assets/61150519/0de05b21-ca32-4129-8324-eb00b40ad17d" alt="Descrição da imagem">
</p>
<p align="center" style="font-size: 18px; margin: 10px;"> Figura 12. Consultando o nome e o sobrenome da tabela contatos.</p>

Ainda podem surgir situações que necessitem selecionar apenas um registro. Neste caso, utilizamos o **WHERE**
Vamos selecionar o cliente com uma cláusula que deve ter **nro_contato= 101**:

```C
SELECT nome, sobrenome
FROM contatos
WHERE nro_contato= 100;
```

Para colunas do tipo texto será necessário colocar o valor entre aspas simples, assim dizemos ao SGBD que estamos querendo comparar o valor com uma coluna do tipo texto:

```C
SELECT nome, sobrenome
FROM contatos
WHERE nome= ‘Bruno’;
```

E se quiséssemos todos os clientes que sejam diferentes de **‘100’**? Faríamos uma consulta utilizando o operador do **MySQL** diferente **<>**:

```C
SELECT nome, sobrenome
FROM contatos
WHERE nro_contato<> 100;
```

<p align="center">
  <img width="550" height="320" src="https://github.com/roneycsilva/zenodo/assets/61150519/42b28660-607e-4856-8e58-bee78df808f4" alt="Descrição da imagem">
</p>
<p align="center" style="font-size: 18px; margin: 10px;">Figura 13. Utilizando a clausula “WHERE nro_contato <> 100”.</p>

 
Além dos operadores de comparação = e <>, temos os seguintes operadores:
• >: maior;
• <: menor;
• >=: maior e igual;
• <=: menor e igual.

A clausula **DISTINCT** retorna apenas uma linha de dados para todo o grupo de linhas que tenha o mesmo valor. Por exemplo, executando a consulta a seguir:

```C
SELECT DISTINCT sobrenome FROM contatos;
```
Os valores retornados são apenas três, pois Santos se repete duas vezes:

```C
Santos
Carvalho
Silva
```

Já a clausula **ALL** é o oposto de **DISTINCT**, pois retorna todos os dados. Observe a consulta a seguir:

```C
SELECT ALL sobrenome FROM contatos;
```

Repare que o resultado a seguir apresenta o sobrenome Santos duas vezes:

```C
Santos
Carvalho
Santos
Silva
```

A clausula **ORDER BY** retorna os comandos em ordem **ascendente (ASC)** ou **descendente (DESC)**, sendo o padrão _ascendente_. 

Vejamos um exemplo:

```C
SELECT nome FROM contatos ORDER BY nome DESC;
```
Repare que os nomes são retornados em ordem descrescente

```C
Isabelle
Elaine
Cauã
Bruno
```
A clausula **LIMIT [inicio,]** linhas retorna o número de linhas especificado. Se o valor inicio for fornecido, aquelas linhas são puladas antes do dado ser retornado. **Lembre-se que a primeira linha é 0**.

```C
SELECT * FROM contatos LIMIT 3,1;
```
O resultado da consulta será:

```C
103 Isabelle Silva 11 999999999 2013-11-20 contato@rh.com.br
```
Para incrementar as consultas podemos usar algumas funções. A seguir apresentaremos as mais comuns:

• A função ABS retorna o valor absoluto do número, ou seja, só considera a parte numérica, não se importando com o sinal de positivo ou negativo do mesmo. Por exemplo: **ABS(-145) retorna 145**;<p></p>
• A função **BIN** considera o binário de número decimal. Por exemplo: **BIN(8) retorna 1000;**<p></p>
• A função **CURDATE() / CURRENTDATE()** retorna a data atual na forma **YYYY/MM/DD**. Por exemplo: **CURDATE() retorna 2002/04/04**;<p></p>
• A função **CURTIME() / CURRENTTIME()** retorna a hora atual na forma **HH:MM:SS**. Por exemplo: **CURTIME() retorna 13:02:43**;<p></p>
• A função **DATABASE** retorna o ome do **banco de dados atual**: Por exemplo: **DATABASE() retorna DBDevMedia**;<p></p>
• A função **DAYOFMONTH** retorna o **dia do mês para a data dada**, na **faixa de 1 a 31**. Por exemplo: **DAYOFMONTH("2004-04-04") retorna 04**;<p></p>
• A função **DAYNAME** retorna o **dia da semana para a data dada**. Por exemplo: **DAYNAME("2004-04-04") retorna Sunday**;<p></p>
• A função **DAYOFWEEK** retorna o **dia da semana em número para a data dada**, na **faixa de 1 a 7**, onde o **1 é domingo**. Por exemplo: **DAYOFWEEK("2004-04-04") retorna 1;**<p></p>
• A função **DAYOFYEAR** retorna o **dia do ano para a data dada**, na faixa de **1 até 366**. Por exemplo: **DAYOFYEAR("2004-04-04") retorna 95**;<p></p>
• A função **FORMAT(NÚMERO, DECIMAIS)** formata o número nitidamente com o número de decimais dado. Por exemplo: **FORMAT(5543.00245,2) retorna 5.543.002,45**<p></p>

A função **LIKE** merece um destaque especial, pois faz uma busca **sofisticada** por uma **substring** dentro de uma **string informada**. Temos, dentro da função **LIKE**, os seguintes caracteres especiais utilizados em substrings:

• %: busca zero ou mais caracteres;<p></p>
•_: busca somente um caractere.<p></p>

Vamos a alguns exemplos:<p></p>
```C
SELECT nome From contatos Where nome like ‘B%’;
```
O caractere ‘%’ nessa consulta indica que estamos procurando nomes que possuem a inicial B, ou seja, com base na nossa tabela contatos, o retorno será apenasBruno.
```C
SELECT nome From contato Where nome like ‘_a%’;
```

O caractere ‘_’ na consulta indica que estamos procurando nomes nos quais a letra A é a segunda letra do nome, ou seja, o retorno será apenas Cauã.
```C
SELECT nome From contato Where nome like ‘%o’;
```

A consulta buscou nomes em que a última letra é o caractere ‘O’, ou seja, teremos como retorno apenas Bruno.
Outra função importante para retorno de consultas é Left, que retorna os primeiros caracteres à esquerda de uma string. Sua sintaxe é apresentada a seguir:
```C
LEFT(string,tamanho)
```
A consulta a seguir retornará os três primeiros caracteres à esquerda dos registros da coluna nome:
```C
SELECT LEFT(nome,3) from contatos
```
O resultado será:
```C
Bru
Ela
Cau
Isa
```

A função **Right** é semelhante a função **Left**, mas esta retorna os **últimos caracteres à direita de uma string**. Sua sintaxe também é semelhante:
O resultado será:
```C
RIGHT(string1,tamanho)
```

Repare que na consulta a seguir **são retornados os quatro últimos caracteres à direita dos nomes da tabela contatos**:
```C
SELECT RIGHT(nome,4) From contatos;
```
O resultado será:
```C
runo
aine
Cauã
ele
```
## **Python**##
>História

<div style="text-align: justify; font-size: 18px; margin: 10px;">
Python é uma linguagem de programação de alto nível, interpretada e de propósito geral, criada por Guido van Rossum e lançada pela primeira vez em 1991. Desde então, Python experimentou um crescimento fenomenal e se tornou uma das linguagens mais populares e influentes no mundo da computação.
Nos primeiros anos, Python ganhou destaque principalmente por sua sintaxe simples e legibilidade, tornando-o acessível para programadores iniciantes e experientes. Sua filosofia de design, enfatizada pelo "Zen do Python", promove a legibilidade do código e a simplicidade.
Ao longo dos anos, Python evoluiu constantemente, com o lançamento de novas versões que introduziram recursos poderosos e melhorias de desempenho. O lançamento da versão 2.0 em 2000 foi um marco significativo, mas eventualmente, em 2008, o desenvolvimento se concentrou na versão 3.x, que trouxe uma série de melhorias substanciais e correções de design.
Python é amplamente utilizado em uma variedade de domínios, desde desenvolvimento web e automação de sistemas até ciência de dados e inteligência artificial. Sua flexibilidade e extensa biblioteca padrão tornam-no uma escolha popular para uma variedade de tarefas de programação.
Nos dias de hoje, Python continua a crescer em popularidade. Grandes empresas como Google, Facebook, Amazon e Microsoft utilizam Python em suas infraestruturas e desenvolvimento de software. Além disso, comunidades de desenvolvedores em todo o mundo contribuem ativamente para o ecossistema Python, criando bibliotecas, frameworks e ferramentas que estendem ainda mais sua funcionalidade e usabilidade.
 <p></p>

## **Instalação do ambiente Python** ##
<div style="text-align: justify; font-size: 18px; margin: 10px;">
O ambiente Python (linguagem, interpretador, módulos e ferramentas) é super simples de se instalar, em caso de sistema operacional (SO) Linux, a maioria das distribuições já vem com Python instalado, porque 17vários scripts do SO já são executados em Python. 
Para verificar se já está instalado no Linux ou Windows, abra a console de comandos do sistema operacional e digite o comando python --version. que apresenta o resultado do comando.
 <p></p>

<p align="center">
  <img width="500" height="190" src="https://github.com/roneycsilva/zenodo/assets/61150519/0623cae1-d545-448f-af16-9648a0867883">
</p>
<p align="center" style="font-size: 18px; margin: 10px;">Figura 9 Verifica instalação da linguagem Python.</p>

<div style="text-align: justify; font-size: 18px; margin: 10px;">
No Linux, caso seja detectado que não há Python instalado, utilize o seu gerenciador de pacote preferido conforme comandos na Tabela 1 abaixo:
 <p></p>

| Gerenciado de Pacote Linux | Comando                            | Oque esta Intalado									 |
| :---                       |     :---:                          |          :---     									 |
| Apt-get                    | sudo apt-get install python3.8     | Python            									 |
|                            | sudo apt-get install python-pip    | Gerenciador de módulos do Python. Serve para instalar extensões do Python.           |
|   Yum                      | sudo yum install python38          | Python         									 |
|                            | yum -y install python-pip          | Gerenciador de módulos do Python.    					         |

<div style="text-align: justify; font-size: 18px; margin: 10px;">
No Windows, por padrão, não vem instalado, então você deve baixar o instalador e realizar a instalação no seu computador. O site oficial é  www.python.org.
 <p></p>

<p align="center">
  <img width="600" height="300" src="https://github.com/roneycsilva/zenodo/assets/61150519/5ac282e7-1039-48aa-addb-1446dd3c009f">
</p>
<p align="center" style="font-size: 18px; margin: 10px;">Figura 10 Site oficial da linguagem Python.</p>

<div style="text-align: justify; font-size: 18px; margin: 10px;">
No website, acesse a aba “downloads” e baixe o instalador Python. Na ocasião de escrita deste material, a versão do momento é a Python 3.8.0. Se na época em que estiver lendo este livro, existir uma versão mais nova, não tem problema, todos os passos aqui ensinados se aplicarão. <p></p>
	
<p align="center">
  <img width="600" height="300" src="https://github.com/roneycsilva/zenodo/assets/61150519/6dd7f7d2-4330-468b-adc4-4af9c5e8c3cd">
</p>
<p align="center" style="font-size: 18px; margin: 10px;">Figura 11 Local para baixar o instalador Python para Windows.</p>
 
<div style="text-align: justify; font-size: 18px; margin: 10px;">
Para instalar o Python 3.8 na sua máquina, basta executar o arquivo de instalação com dois cliques ou pressionar ENTER após selecioná-lo. Durante a instalação, siga o processo padrão do Windows, clicando em "Next" algumas vezes e depois em "Finish". Na primeira tela, certifique-se de marcar a opção "Add Python 3.8 to PATH" e clique em "Install Now" para concluir a instalação.<p></p>
	
<p align="center">
  <img width="600" height="300" src="https://github.com/roneycsilva/zenodo/assets/61150519/caf6aca3-e42e-4492-8735-40b8e91e5abb">
</p>
<p align="center" style="font-size: 18px; margin: 10px;">Figura 12 Primeira janela do instalador Python no Windows.</p>

<div style="text-align: justify; font-size: 18px; margin: 10px;">
Após clicar em "Install Now", o processo de instalação será iniciado. Esteja atento, pois como a instalação envolve a modificação de arquivos do sistema, o Windows pode solicitar sua confirmação para prosseguir. Certifique-se de responder "Sim" quando essa pergunta surgir.
<p></p>
	
<p align="center">
  <img width="600" height="300" src="https://github.com/roneycsilva/zenodo/assets/61150519/08200100-1c89-4b83-8016-4824cb567b76">
</p>
<p align="center" style="font-size: 18px; margin: 10px;">Figura 13 Janela de progresso de instalação da linguagem Python.</p>

<div style="text-align: justify; font-size: 18px; margin: 10px;">
Ao fim do processo, aparece uma janela informando que a instalação foi concluída com sucesso. Clique agora em close para fechar a janela.<p></p>
	
<p align="center">
  <img width="600" height="300" src="https://github.com/roneycsilva/zenodo/assets/61150519/66dc2e66-1f96-4900-9826-367fe7688266">
</p>
<p align="center" style="font-size: 18px; margin: 10px;">Figura 14 Janela que informa o sucesso da instalação no Windows.</p>
 

<div style="text-align: justify; font-size: 18px; margin: 10px;">
Depois da instalação, executar teste para verificar se tudo foi instalado correto. No Windows ir em programas instalados e localizar a pasta Python 3.8. Execute o aplicativo IDLE conforme a imagem abaixo.<p></p>
	
<p align="center">
  <img width="600" height="330" src="https://github.com/roneycsilva/zenodo/assets/61150519/30564a7f-ca3e-46bf-bf2f-fc8a9d5b2671">
</p>
<p align="center" style="font-size: 18px; margin: 10px;">Figura 15 Como iniciar a interface de programação IDLE.</p>
 
 
 <div style="text-align: justify; font-size: 18px; margin: 10px;">
O IDLE é um ambiente de desenvolvimento integrado para Python, que é lançado em cada liberação da ferramenta desde a versão 2.3. Na nossa opinião, não é a melhor ferramenta para se programar, mas para aprender programação é excelente.<p></p>
	
<p align="center">
  <img width="600" height="330" src="https://github.com/roneycsilva/zenodo/assets/61150519/6f685ef6-2b52-401e-86d0-39648a3e3333">
</p>
<p align="center" style="font-size: 18px; margin: 10px;">Figura 16 O ambiente IDLE.</p>

  <div style="text-align: justify; font-size: 18px; margin: 10px;">
Para desenvolvedores que estejam em um estágio avançado de conhecimento da linguagem em Python, pode ser utilizado o ambiente Pycharm da JetBrains. Um ambiente mais produtivo contendo excelentes facilidade de depuração de código.<p></p>
	
<p align="center">
  <img width="600" height="330" src="https://github.com/roneycsilva/zenodo/assets/61150519/942e9d84-dfad-4272-be35-6057025566f1">
</p>
<p align="center" style="font-size: 18px; margin: 10px;">Figura 17 Tela inicial do Pycharm.</p>

   <div style="text-align: justify; font-size: 18px; margin: 10px;">
Depois de instalar o Python, é hora de vermos o primeiro programa funcionando, neste caso usaremos o tradicional "Hello World. <p></p>
	
<p align="center">
  <img width="600" height="330" src="https://github.com/roneycsilva/zenodo/assets/61150519/ce2f0df7-c183-4e18-9907-78fbc9bd2388">
</p>
<p align="center" style="font-size: 18px; margin: 10px;">Figura 18 Exemplo de programa “Hello World” no Python.</p>

 <div style="text-align: justify; font-size: 18px; margin: 10px;">
Quando executado o programa, foi utilizado o console da linguagem Python. asicamente, é um espaço onde digita comandos, pressiona ENTER e eles são executados imediatamente. 
Para criar um módulo Python, “uma sequência de comandos em um arquivo”, basta clicar em "File", depois em "New File" iniciar a programação. Ao terminar de escrever o programa, basta pressionar a tecla F5, nomear o arquivo e observar o resultado do seu programa. É uma forma prática e simples de desenvolver seus próprios scripts em Python.<p></p>
 

## **Introdução ao MySQL Connector/Python** ##
>MySQL Connector/Python

 <div style="text-align: justify; font-size: 18px; margin: 10px;">
O MySQL Connector/Python é uma ferramenta que permite que programas escritos em Python acessem bancos de dados MySQL, seguindo a especificação de API de banco de dados Python v2.0 (PEP 249). 

Ele oferece suporte a uma ampla gama de recursos incluindo:
• Quase todos os recursos do MySQL Server 5.7 e superior, com suporte ao X DevAPI, <p></p>
• Conversão de valores entre tipos de dados Python e MySQL, <p></p>
• Extensões MySQL para sintaxe SQL padrão, <p></p>
• Compactação de protocolo, <p></p>
• Conexões seguras TCP/IP e Unix, <p></p>
• Um driver independente. <p></p>

É importante observar que o Connector/Python não suporta os antigos métodos de autenticação do MySQL Server, exigindo versões 4.1 ou superiores do MySQL para funcionar.<p></p>


**Diretrizes para desenvolvedores Python**

 <div style="text-align: justify; font-size: 18px; margin: 10px;">

Para criar aplicativos MySQL com Python, é essencial seguir algumas diretrizes importantes. Em primeiro lugar, evite codificar informações de login diretamente no script principal em vez disso, utilize um arquivo de configuração separado. Além disso, considere otimizar o armazenamento e a recuperação de dados usando IDs numéricos em tabelas MySQL, o que pode reduzir o tamanho dos valores das chaves e minimizar a duplicação de dados.

Ao lidar com entrada de dados, certifique-se de validar e tratar possíveis dados incorretos, tanto no lado do servidor quanto no cliente, usando técnicas como restrições exclusivas, tratamento de exceções e validação de entrada. Importante proteger contra ataques de "injeção de SQL" escapando caracteres especiais e validando os dados de entrada para evitar comportamentos inesperados nas consultas SQL.

Por fim, ao lidar com grandes conjuntos de resultados de consultas SQL, utilize métodos eficientes para recuperar e processar os itens do conjunto de resultados conforme necessário. Essas práticas ajudarão a garantir a segurança e o desempenho dos seus aplicativos MySQL em Python. 

Aqui estão os métodos disponíveis para isso:

• fetchone(): Recupera um único item do conjunto de resultados. Este método é adequado quando você sabe que o conjunto de resultados contém apenas uma linha.<p></p>
• fetchall(): Recupera todos os itens do conjunto de resultados e os retorna como uma lista. É recomendado usar este método quando você sabe que o conjunto de resultados tem um número limitado de linhas que cabem confortavelmente na memória.<p></p>
• fetchmany(size): Recupera vários itens do conjunto de resultados, especificados pelo parâmetro `size`, e os retorna como uma lista. Este método é mais adequado quando você não pode prever o tamanho total do conjunto de resultados. Você pode continuar chamando `fetchmany()` e percorrendo os itens retornados até que não haja mais resultados para processar.<p></p>

Python oferece módulos convenientes como pickle e cPickle para gravar estruturas de dados em disco, no entanto ao armazenar dados no MySQL, é importante considerar caracteres especiais que podem estar presentes.

• Quando lidamos com conjuntos de dados muito grande, é necessário otimizar as consultas usando instruções SELECT para recuperar apenas os itens necessários. Configurar a opção innodb_buffer_pool_size no servidor MySQL é crucial para dedicar uma quantidade específica de RAM ao cache de dados de tabela e índice.<p></p>

• Para lidar com dados complexos, é recomendado dividir os dados entre diferentes tabelas SQL e reuni-los usando consultas de junção. Configurar relacionamentos de chave primária é fundamental para garantir a consistência dos dados relacionados.<p></p>

• Quando os dados são frequentemente atualizados por vários usuários simultaneamente, é essencial utilizar instruções SQL como INSERT, UPDATE e DELETE para atualizar itens de forma eficiente, gravando apenas os valores alterados no disco. O uso de tabelas InnoDB e transações ajuda a evitar conflitos entre operações de gravação e garante resultados consistentes durante atualizações concorrentes.<p></p>

Seguir as melhores práticas do MySQL pode melhorar significativamente o desempenho do seu aplicativo, permitindo escalabilidade sem grandes reescritas ou mudanças de arquitetura. Utilizar instruções SQL de forma clara e objetiva, juntamente com extensões e cláusulas específicas do MySQL, pode garantir resultados eficientes. 
Recomenda-se consultar as seções relevantes da documentação do MySQL para entender melhor as principais instruções e cláusulas disponíveis. 
Ao emitir instruções SQL em Python, é comum lidar com literais de string longos que podem abranger várias linhas. Para simplificar esse processo, o Python oferece o mecanismo de aspas triplas, permitindo incluir a instrução inteira de forma mais conveniente.
Aqui está um exemplo simples:	 
  <p></p>
  
```C
'''It doesn't matter if this string contains 'single'
or "double" quotes, as long as there aren't 3 in a
row.'''
```
 <div style="text-align: justify; font-size: 18px; margin: 10px;">
Pode usar tanto para aspas simples (') quanto aspas duplas (") para criar literais de string multilinhas usando o mecanismo de aspas triplas no Python.

Para garantir uma aplicação MySQL rápida e escalável, é crucial usar a sintaxe correta, especialmente ao criar tabelas com instruções CREATE TABLE. Recomenda-se o uso da cláusula ENGINE=INNODB para a maioria das tabelas, devido aos benefícios transacionais e de escalabilidade oferecidos pelo mecanismo de armazenamento InnoDB. 
É importante também declarar uma chave primária numérica para cada tabela, facilitando a busca de valores e sua utilização como chave estrangeira em outras tabelas. Além disso, ao definir os tipos de dados das colunas, deve-se optar por aqueles mais compactos para melhorar o desempenho e a escalabilidade do sistema, reduzindo a movimentação de dados entre memória e disco.
<p></p>

**Conectando Python ao banco de dados MySQL**

 <div style="text-align: justify; font-size: 18px; margin: 10px;">
O Python não possui um acesso nativo a banco de dados SQL em sua biblioteca padrão, somente ao Berkley database engine (BDB), neste trabalho vamos utilizar mysql.connecto utilizando o sistema de gerenciamento de pacotes pip. 

Com o terminal do seu sistema operacional aberto digite o comando pip install mysql-connector-python
pip install mysql-connector-python
Caso esteja enfrentando algum problema durante a instalação, verifique a versão e módulo tentando instalá-lo novamente. Dúvida verifique a tabela abaixo para instalar versão correta. 
<p></p>

| Conector MySQL Python | Versões do MySQL     		 | Versões Python       	   |
| 	:---            |     	:---             	 |        :--- 			   |
|8,0  		        | 8,0, 5,7, 5,6, 5,5    	 | 3,6, 3,5, 3,4, 2,7  		   |
|2.2 		        | 5,7, 5,6, 5,5        		 | 3,5, 3,4, 2,7        	   |
|2.1 		        | 5,7, 5,6, 5,5        		 | 3,5, 3,4, 2,7, 2,6   	   |
|2.0 		        | 5,7, 5,6, 5,5        		 | 3,5, 3,4, 2,7, 2,6   	   |
|1.2		        | 5,7, 5,6, 5,5 (5,1, 5,0, 4,1)  | 3,4, 3,3, 3,2, 3,1, 2,7, 2,6    |



<p align="center" style="font-size: 18px; margin: 10px;">Versões do conector Python MySQL</p>

 <div style="text-align: justify; font-size: 18px; margin: 10px;">
• Para evitar possíveis erros, insira no final a versão do mysql, instalado em usa máquina usando o comando pip install:
	 
```C
mysql-connector-python==8.0.13
``` 	 
<p></p>

• Se você estiver enfrentando um erro de falha na instalação do pip com connection:  
  
```C
error: [SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed (_ssl.c:598)
```  
 Este erro pode ser resolvido ignorando o erro de SSL definindo pypi.org e files.pythonhosted.org como hosts confiáveis. <p></p>

```C
python -m pip install --trusted-host pypi.org --trusted-host files.pythonhosted.org --trusted-host pypi.python.org mysql-connector-python
```
Após a instalação do MySQL Connector Python é executar o comando:

```C
pip: -
```
 Apresenta os seguintes mensagens:
 
• Coletando ``` mysql-connector-python<p></p>```<p></p>
• Baixando pacotes.<p></p>
• Requisito já atendido: ferramentas de configuração em```D:python\python37-32\lib\site-packages```p></p>
• Instalando pacotes coletados: ```mysql-connector-python```p></p>
•  ```C MySQL-connector-python-8.0.13``` instalado com sucesso p></p>

Com o **MySQL Connector Python** instalado é necessário fazer o import da biblioteca para comunicação entre MySQL e Python

```C
from mysql.connector import connect
```

A função connect() fornecida pelo módulo mysql.connector é essencial para estabelecer a comunicação entre o seu código e o banco de dados. Necessário fornecer alguns parâmetros importantes, como o nome do host onde o banco de dados está localizado, o nome de usuário e a senha para autenticação, além do nome do banco de dados que deseja acessar. 
Aqui está um exemplo simples: 
<p></p>
	
```C
def mysql_connection(host, user, passwd, database=None):
    connection = connect(
        host = host,
        user = user,
        passwd = passwd,
        database = database
    )
    return connection
```

Em seguida, é feita a chamada da função **mysql_connection**, que foi criada anteriormente, passando os parâmetros necessários.

```C
connection = mysql_connection('localhost', 'root', 'mysql123')

```


**Estrutura de Dados MySQL e Python**

 <div style="text-align: justify; font-size: 18px; margin: 10px;">
A estrutura de dados MySQL com Python envolve a utilização da linguagem de programação Python para interagir com bancos de dados MySQL. Isso inclui a criação, manipulação e consulta de tabelas, além da execução de operações como inserção, atualização, exclusão e seleção de dados. 
Para essa integração, podemos contar com bibliotecas como o MySQL Connector/Python, facilitando o desenvolvimento de aplicativos eficientes e robustos que fazem uso de bancos de dados relacionais.
No processo de criação da estrutura de dados no MySQL com Python, o primeiro passo é criar uma nova base de dados. Isso é realizado através da execução de um comando SQL (CREATE DATABASE), armazenado em uma variável chamada query. 
Em seguida, estabelecemos a conexão com o banco de dados e executamos o comando SQL utilizando um cursor. Essa abordagem nos permite automatizar o processo de criação da base de dados de forma eficaz e direta.
O processo completo envolvendo a interação com um banco de dados MySQL pode ser dividido em várias etapas. Desde a criação da base de dados até o encerramento da conexão, cada passo desempenha um papel crucial no gerenciamento dos dados. 
Abaixo está uma descrição detalhada de cada etapa:. 
<p></p>

 <div style="text-align: justify; font-size: 18px; margin: 10px;">
	 
1. Criar a Base de Dados: antes de qualquer interação com o banco de dados, é necessário criar a base de dados. Isso pode ser feito através do MySQL Shell ou de uma interface de gerenciamento, como o phpMyAdmin. Durante este processo, é importante definir o nome da base de dados e, opcionalmente, especificar configurações adicionais, como o conjunto de caracteres e a codificação.<p></p>

2. Conectar à Biblioteca MySQL: para interagir com o banco de dados MySQL em um ambiente Python, é necessário utilizar uma biblioteca compatível, como `mysql-connector-python`. Essa biblioteca fornece métodos e classes para estabelecer conexões com o banco de dados, executar consultas e manipular resultados.<p></p>

3. Criar um Objeto Cursor: após estabelecer uma conexão com o banco de dados, um objeto cursor é criado. O cursor é essencial para executar comandos SQL e recuperar resultados de consultas. Ele atua como um ponto de controle para enviar comandos SQL para o banco de dados e receber os resultados de volta.<p></p>

4. Criar tabela: com a função query podemos criar a tabela de dados a variável query, vai receber um comando SQL (CREATE TABLE, para criação da tabela). Em seguida criamos uma variável chamada cursor, que vai estabelecer a conexão através da variável connection. Finalizamos com a variável cursor executando o comando SQL da variável query.<p></p>

5. Alimentar Dados: inserir novos registros na base de dados é uma tarefa comum. Isso pode ser feito através de comandos SQL de inserção, como `INSERT INTO`. Durante esse processo, os dados são adicionados às tabelas, seguindo a estrutura definida anteriormente.<p></p>

6. Atualizar Dados: às vezes, é necessário modificar registros existentes na base de dados. Isso pode ser feito usando comandos SQL de atualização, como `UPDATE`. Os dados existentes são alterados de acordo com as condições especificadas na consulta.<p></p>

7. Consultar Dados: recuperar informações específicas da base de dados é uma operação comum. Isso é feito através de consultas SQL, como `SELECT`, que retornam conjuntos de resultados que atendem aos critérios especificados.<p></p>

8. Deletar Dados: para remover registros da base de dados, são utilizados comandos SQL de exclusão, como `DELETE FROM`. Isso elimina os registros que correspondem às condições especificadas na consulta.<p></p>

9. Fechar a Conexão: após concluir todas as operações necessárias no banco de dados, é importante fechar a conexão para liberar recursos do sistema. Isso é feito chamando o método `close()` na conexão estabelecida.<p></p>
 
<p></p>

 <div style="text-align: justify; font-size: 18px; margin: 10px;">

Cada uma dessas etapas desempenha um papel fundamental na gestão eficaz dos dados em um ambiente MySQL, garantindo a integridade e a consistência das informações armazenadas.
<strong><em>1. Criar a Base de Dados </em></strong><p></p>
Para criar um banco de dados MySQL usando mysql.connector.connect(), primeiro você precisa ter o MySQL Server instalado e em execução. Em seguida, você pode usar essa função para se conectar ao servidor MySQL e executar uma instrução SQL para criar o banco de dados.
Aqui está um exemplo simples:
 <p></p>

```C
import mysql.connector

conexao = mysql.connector.connect(
    host="localhost",
    user="seu_usuario",
    password="sua_senha"
)
cursor = conexao.cursor()
query = "CREATE DATABASE minha_base_de_dados"

cursor.execute(query)
cursor.close()
conexao.close()
```
 <div style="text-align: justify; font-size: 18px; margin: 10px;">
<strong><em>2. Conectar à Biblioteca MySQL </em></strong><p></p>
Para conectar-se à biblioteca MySQL em Python, instale o pacote mysql-connector-python e utilize a função connect(), fornecida por ela, passando os parâmetros necessários, como host, usuário, senha e nome do banco de dados. Assim, você estabelece a conexão para executar operações no banco de dados.
Aqui está um exemplo simples:
 <p></p>
 
```C
conexao = mysql.connector.connect(
    host="localhost",
    user="seu_usuario",
    password="sua_senha",
    database="minha_base_de_dados"  # Adicionando o nome da base de dados
)
```

 <div style="text-align: justify; font-size: 18px; margin: 10px;">
<strong><em>3. Criar um Objeto Cursor</em></strong><p></p>
Para criar um objeto Cursor em Python ao trabalhar com banco de dados, utilize o método cursor() na conexão estabelecida com o banco de dados. Este objeto Cursor permite executar consultas SQL e manipular os resultados retornados pelo banco de dados.
Aqui está um exemplo simples:
 <p></p>
 
```C
cursor = conexao.cursor()

```

 <div style="text-align: justify; font-size: 18px; margin: 10px;">
<strong><em>4. Criar tabela</em></strong><p></p>
Para criar uma tabela em um banco de dados MySQL usando o conector MySQL em Python, você pode usar o objeto Cursor para executar uma instrução SQL CREATE TABLE. 
Aqui está um exemplo simples:
 <p></p>
 
```C
query = """
    CREATE TABLE minha_tabela (
        id INT AUTO_INCREMENT PRIMARY KEY,
        nome VARCHAR(255),
        idade INT
    )
"""
```

 <div style="text-align: justify; font-size: 18px; margin: 10px;">
<strong><em>5. Alimentar Dados</em></strong><p></p>
Para alimentar dados em uma tabela do banco de dados MySQL usando o conector MySQL em Python, você pode utilizar o objeto Cursor para executar instruções SQL de inserção (INSERT INTO). 
Aqui está um exemplo simples:
 <p></p>
 
```C
query = '''
    INSERT INTO minha_tabela VALUES
        (1001, 'Novo Nome 1', '1199999-9999', user1@email.com', São Paulo),
        (1002, 'Novo Nome 2', '2199999-9999', 'user2@email.com', 'Rio de Janeiro'),
        (1003, 'Novo Nome 3', '1199999-9999', 'user3@email.com', São Paulo),
        (1004, 'Novo Nome 4', '4199999-9999', 'user4@email.com', 'Curitiba'),
        (1005, 'Novo Nome 5', '2199999-9999', 'user5@email.com', Rio de Janeiro),
        (1006, 'Novo Nome 6', '2199999-9999', 'user6@email.com', 'Rio de Janeiro'),
        (1007, 'Novo Nome 7', '1199999-9999', 'user@email.com', 'Santos')
'''

cursor = connection.cursor()
cursor.execute(query)
connection.commit()
```

 <div style="text-align: justify; font-size: 18px; margin: 10px;">
<strong><em>6. Atualizar Dados: </em></strong><p></p>
Para atualizar dados em uma tabela do banco de dados MySQL usando o conector MySQL em Python, você pode utilizar o método execute(). Isso pode ser feito usando comandos SQL de atualização, como `UPDATE`. Os dados existentes são alterados de acordo com as condições especificadas na consulta.
Aqui está um exemplo simples:
 <p></p>
 
```C
import mysql.connector

hostname = 'localhost'  # ou o endereço IP do seu servidor MySQL
username = 'seu_usuario_mysql'  # seu nome de usuário MySQL
password = 'sua_senha_mysql'  # sua senha MySQL
database = 'seu_banco_de_dados_mysql'  # nome do seu banco de dados MySQL

try:
    conn = mysql.connector.connect(
        host=hostname,
        user=username,
        password=password,
        database=database
    )
    print("Conexão ao Banco de Dados estabelecida com sucesso!")

    cursor = conn.cursor()

    update_query = "UPDATE clientes SET email = 'novo_email@example.com' WHERE nome = 'Alice'"

    cursor.execute(update_query)
    conn.commit()
    print("Dados atualizados na tabela 'clientes' com sucesso!")

except mysql.connector.Error as err:
    print("Erro ao conectar ao Banco de Dados:", err)
    conn.rollback()

finally:
    if 'conn' in locals() and conn.is_connected():
        cursor.close()
        conn.close()
        print("Conexão ao Banco de Dados fechada.")
```


 <div style="text-align: justify; font-size: 18px; margin: 10px;">
<strong><em>7. Consultar Dados: </em></strong><p></p>
Recuperar informações específicas da base de dados é uma operação comum. Isso é feito através de consultas SQL, como `SELECT`, que retornam conjuntos de resultados que atendem aos critérios especificados.
Aqui está um exemplo simples:
 <p></p>
 
```C
import mysql.connector

hostname = 'localhost'  # ou o endereço IP do seu servidor MySQL
username = 'seu_usuario_mysql'  # seu nome de usuário MySQL
password = 'sua_senha_mysql'  # sua senha MySQL
database = 'seu_banco_de_dados_mysql'  # nome do seu banco de dados MySQL

try:
    conn = mysql.connector.connect(
        host=hostname,
        user=username,
        password=password,
        database=database
    )
    print("Conexão ao Banco de Dados estabelecida com sucesso!")

    cursor = conn.cursor()

    select_query = "SELECT * FROM clientes"

    cursor.execute(select_query)

    resultados = cursor.fetchall()

    print("Resultados da consulta:")
    for resultado in resultados:
        print(resultado)

except mysql.connector.Error as err:
    print("Erro ao conectar ao Banco de Dados:", err)

finally:
    # Fecha a conexão após o uso
    if 'conn' in locals() and conn.is_connected():
        cursor.close()
        conn.close()
        print("Conexão ao Banco de Dados fechada.")
```

 <div style="text-align: justify; font-size: 18px; margin: 10px;">
<strong><em>8. Deletar Dados: </em></strong><p></p>
Para remover registros da base de dados, são utilizados comandos SQL de exclusão, como `DELETE FROM`. Isso elimina os registros que correspondem às condições especificadas na consulta.
Aqui está um exemplo simples:
 <p></p>
 
```C
import mysql.connector

hostname = 'localhost'  # ou o endereço IP do seu servidor MySQL
username = 'seu_usuario_mysql'  # seu nome de usuário MySQL
password = 'sua_senha_mysql'  # sua senha MySQL
database = 'seu_banco_de_dados_mysql'  # nome do seu banco de dados MySQL

try:
    conn = mysql.connector.connect(
        host=hostname,
        user=username,
        password=password,
        database=database
    )
    print("Conexão ao Banco de Dados estabelecida com sucesso!")

    cursor = conn.cursor()

    delete_query = "DELETE FROM clientes WHERE nome = 'Alice'"

    cursor.execute(delete_query)
    conn.commit()
    print("Dados excluídos da tabela 'clientes' com sucesso!")

except mysql.connector.Error as err:
    print("Erro ao conectar ao Banco de Dados:", err)
    conn.rollback()

finally:
    if 'conn' in locals() and conn.is_connected():
        cursor.close()
        conn.close()
        print("Conexão ao Banco de Dados fechada.")
```

 <div style="text-align: justify; font-size: 18px; margin: 10px;">
<strong><em>9. Fechar a Conexão: </em></strong><p></p>
Após concluir todas as operações necessárias no banco de dados, é importante fechar a conexão para liberar recursos do sistema. Isso é feito chamando o método `close()` na conexão estabelecida.
Aqui está um exemplo simples:
 <p></p>
 
```C
import mysql.connector

# Substitua os valores das variáveis abaixo com as informações do seu banco de dados
hostname = 'localhost'  # ou o endereço IP do seu servidor MySQL
username = 'seu_usuario_mysql'  # seu nome de usuário MySQL
password = 'sua_senha_mysql'  # sua senha MySQL
database = 'seu_banco_de_dados_mysql'  # nome do seu banco de dados MySQL

try:
    conn = mysql.connector.connect(
        host=hostname,
        user=username,
        password=password,
        database=database
    )
    print("Conexão ao Banco de Dados estabelecida com sucesso!")

    cursor = conn.cursor()

finally:
    # Fecha o cursor e a conexão após o uso
    try:
        if cursor:
            cursor.close()
            print("Cursor fechado com sucesso!")
    except Exception as e:
        print("Erro ao fechar o cursor:", e)

    try:
        if conn:
            conn.close()
            print("Conexão ao Banco de Dados fechada com sucesso!")
    except Exception as e:
        print("Erro ao fechar a conexão:", e)
```


 <div style="text-align: justify; font-size: 18px; margin: 10px;">
As considerações finais deste trabalho destacam a importância do MySQL como um sistema de gerenciamento de banco de dados relacional de código aberto amplamente utilizado em aplicações web. Desde sua criação em 1995, o MySQL tem sido valorizado por sua confiabilidade, desempenho e flexibilidade, tornando-se uma escolha fundamental para muitos sistemas dinâmicos na web. Sua capacidade de lidar com grandes volumes de dados e oferecer acesso rápido o tornou indispensável para diversos projetos.

Além disso, o texto ressalta a linguagem de programação Python, escolhida por sua simplicidade, vasta biblioteca padrão e comunidade ativa. Python é amplamente adotada em diferentes setores da indústria devido a essas características.

Por fim, destaca-se a integração entre MySQL e Python através do MySQL Connector/Python. Este conector proporciona uma integração direta e eficiente entre as duas tecnologias, garantindo desempenho otimizado e segurança nos dados. Com uma API amigável, facilita a execução de consultas e atualizações no banco de dados. Sua manutenção ativa pela comunidade e compatibilidade com várias versões do MySQL o tornam uma escolha confiável para o desenvolvimento de aplicativos robustos.

Em suma, o trabalho oferece uma visão abrangente sobre a combinação poderosa do MySQL e Python, destacando não apenas suas características individuais, mas também a forma como se complementam para criar soluções eficientes e seguras para diversas aplicações web.
 <p></p>


 <div style="text-align: justify; font-size: 18px; margin: 10px;">
<strong><em>Referencias: </em></strong><p></p>
	 
MySQL [MySQL](https://dev.mysql.com/doc/refman/8.0/en/).<p></p> 	 
Dowload MySQL [Dowload MySQL](https://dev.mysql.com/downloads/mysql/).<p></p> 
DevMedia [DevMedia](https://www.devmedia.com.br/mysql-tutorial/33309).<p></p> 
MySQL [Documento](https:dev.mysql.com/doc/connector-python/en/preface.htm).<p></p> 
Dado ao Cubo [DadoaoCubo](https://dadosaocubo.com/conectar-banco-de-dados-mysql-com-python/).<p></p> 
