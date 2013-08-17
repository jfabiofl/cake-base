#Cake Base

Base de features comuns em diversos projetos


###Modo Multi Application ou Single Core
Com este branch o core do CakePHP deve estar instalado em seu computador 
ou servidor e adicionado o include_path do mesmo em seu projeto.


###Instalação

* git clone git@github.com:redsuns/cake-base.git


###Configuração

* Altere o include_path dos arquivos webroot/index.php  e webroot/test.php
de ` define('CAKE_CORE_INCLUDE_PATH',  DS . 'opt' . DS . 'cakephp' . DS . 'lib'); ` para
` define('CAKE_CORE_INCLUDE_PATH',  'seu_core_do_cakePHP'); `

webroot/index.php - linha: 66
webroot/test.php - linha: 64


* a partir do shell entre na pasta raiz de seu novo projeto e em seguida entre na pasta ` Console ` 
e rode o cake schema ` ./cake schema create ` para que seu banco de dados seja inicializado. 

* Caso o shell do cake não possa ser executado importe o arquivo schema.sql de ` Config/Schema ` através de 
seu gerenciador de banco de dados.



Para mais opções execute o init.php sem parâmetro que um menu de ajuda será exibido.

