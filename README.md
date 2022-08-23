# Projeto_Docker_2V-main


Existiram alguns passos para a criação deste container.

1. Criar o Dockerfile, chamando o banco de dados Mysql.
2. Criar o docker-compose, que irá subir como a imagem do docker que queremos.
    Dentro dele, existe:
        - As portas
        - O nome do container
        - O nome da imagem
        - A senha nula
        - O nome do administrador
        - Onde está localizado o mysql.

3. E os comandos utilizados??

a. para criar a imagem do docker -> docker build -t mysql-image .
b. para ver os containers ativos -> docker ps -a
            parar um container -> docker stop container-vic
            excluir um container -> docker rm container-vic
c. para subir o container com a imagem -> docker run -dit --name container-vic mysql-image /bin/bash
d. entrar no container ativo -> docker attach container-vic

e. docker run -dit --name container-vic --mount type=bind,source="/c/Users/VICTPGM/teste",target=/var/lib/mysql mysql-image /bin/bash

:) 
    

