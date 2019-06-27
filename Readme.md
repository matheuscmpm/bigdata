#BigData
Projeto montado para ser utilizado no curso de BigData realizado pelo Porto Digital

###Pré-requisitos necessários para utilizar esse repositório
* docker
* docker-compose

###### É possível executar o projeto sem o docker-compose, mas torna um pouco mais complicado, o que foi documentado no docker-compose.yml precisaria ser portado para um comando docker run

### Passos para levantar o ambiente
* Clonar esse repositório dentro da sua pasta de usuário
    * Linux: dentro de /home/<usuario>
    * Windows: dentro de C:/Users/<usuario>
    * Mac: dentro de /Users/<usuario>
    * (pode ficar dentro de qualquer subdiretório, mas precisa estar dentro da pasta do usuário do computador)
* Entrar no diretório clonado via terminal (bash, cmd)
    * É importante que o terminal usado tenha acesso aos comandos: docker e docker-compose
* Executar o comando: docker-compose up -d
    * Esse comando construirá o ambiente de acordo com o docker-compose.yml
    * A primeira vez que executar, vai demorar bastante, depois é tudo bem rápido
* Executar o comando: docker-compose logs -f
    * Comando usado para visualizar os logs do container
    * Necessário para pegar o token do jupyter que será impresso direto no console
    * O terminal ficará em follow nos logs, pra cancelar, basta teclar CTRL+C

Para desativar o ambiente:
* Executar o comando: docker-compose down

###### É importante que todo comando docker-compose seja executado dentro do diretório do projeto
###### Um volume será criado dentro da pasta src pra dentro do container. Recomendo criar todos os notebooks do jupyter dentro da pasta volume que será apresentada, dessa forma, você pode editar direto do seu computador. 
