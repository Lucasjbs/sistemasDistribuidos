************************************************************************
 PROJETO FEITO NO PRIMEIRO SEMESTRE DE 2021 NA LINGUAGEM JAVA
************************************************************************

O Projeto consiste na criação de um sistema simples de backup distribuído, com suporte a alta disponibilidade de dados. 
O projeto será construído usando a API sockets da linguagem Java. Desta forma, os conceitos teóricos relacionados com a 
comunicação entre processos serão tratados numa abordagem hands-on.

O aluno deverá criar um processo cliente que será responsável por sincronizar com um servidor de backup os dados armazenados 
no computador do usuário. O processo cliente deverá monitorar um determinado diretório e executar os seguintes procedimentos:
⦁	Se um usuário criar ou colar um arquivo/diretório novo dentro do diretório monitorado, esse arquivo/diretório deverá ser criado 
também no servidor de backup (isto é, enviado para o servidor).
⦁	Se um usuário editar um determinado arquivo/diretório dentro do diretório monitorado, a(s) alteração(ões) deverá(ão) ser replicada(s) 
no servidor de backup para manter a consistência dos dados armazenados no computador do usuário e nos servidores de backup.
⦁	Se um usuário deletar um arquivo/diretório dentro do diretório monitorado, o arquivo/diretório deverá ser removido também no servidor 
de backup.
⦁	A definição do diretório a ser monitorado pelo processo cliente pode ser realizada  pelo próprio desenvolvedor, via hard coding, ou 
pelo usuário, via prompt (no terminal).
⦁	Não será exigido o desenvolvimento de interface gráfica para o processo cliente. Fica a critério do aluno implementar essa 
característica adicional no seu projeto.  
⦁	O aluno deverá criar três processos servidores que serão responsáveis por manterem cópias consistentes dos dados de um determinado 
computador do usuário que está sendo monitorado.
⦁	Um processo servidor será o principal, responsável por manter contato direto com o processo cliente, para fins de obtenção dos 
arquivos/diretórios a serem persistidos.
⦁	Dois processos servidores serão secundários, responsáveis por manterem cópias replicadas dos dados obtidos a partir do processo 
servidor principal.
⦁	Todas as ações (adição, alteração e exclusão de arquivos/diretórios) realizadas pelo usuário sobre o diretório monitorado no seu 
equipamento deverão ser reproduzidas também nos servidores secundários de backup.
⦁	Como os três servidores executarão na mesma máquina, para fins de controle, cada um poderá criar uma pasta específica para manter os 
dados do backup sob sua tutela.

************************************************************************
 EXECUÇÃO
************************************************************************

O projeto foi criado na IDE NetBeans.
Antes de executar o arquivo "Main.java" é necessário executar os servidores de backup: "Server2.java", "Server3.java" e "MainServer.java"
Após isso, execute o arquivo "Main.java" e utilize a interface do NetBeans para navegar pelos diretórios dentro do projeto.
