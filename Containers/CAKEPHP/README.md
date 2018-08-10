Containers docker APACHE, PHP e MYSQL. 
 - Pré-requisitos: docker e docker-compose instalado na maquina. 
  
1 - Baixe o arquivo docker-compose.yml na sua pasta de escolha.

2 - Edite informacoes como porta da sua preferencia, nome do container, nome do banco e senha usuario banco.  

3 - Rode docker-compose up -d (Verificar antes se a porta já está sendo usada por outro container).

4 - O docker irá criar um diretorio chamado www/ ( local que estará online suas aplicacoes ). 

5 - Faça um clone do projeto dentro da pasta www gerada pelo docker-compose.yml.  

6 - Verifique se houve sucesso na montagem rode  docker ps (listagem dos container ativos)

8 - configuracao workbench ou ferramenta de visao de banco dados: 

   - use o endereco listado com o comando docker ps. 
     monte a conexao lembrando que a porta do mysql será usada a que foi cadastrada no docker-compose.yml 


9 - configuracao aplicaçao para enxergar o banco

  -  O servidor web visualiza o banco usando o nome db. nao configurar a aplicacao usando localhost. \n
     'depends_on: - db' essa linha no docker-compose e um link para a imagem do mysql.
     O endereco db representa localhost para nosso container web.    
 
      
   
 
