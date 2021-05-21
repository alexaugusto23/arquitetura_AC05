# arquitetura_AC05
Criação de APP Flask com banco de dados no Docker e Doker Compose.

Comandos - DOCKER

docker logs --help -> Mostra os Comandos.
docker images -a -> Listas todas as imagens.
docker ps ->
docker info -> Exibe informações do docker.
docker login -u login e -p senha -> Faz login no servidor de registo docker.
docker logout -> Faz logout no servidor de registo docker.
docker search -> Pesquisa imagnes no repositório "regis" ou "--limit" ex: "--limit l redis" 
docker pull php: latest -> Baixa imagens do docker hub.
docker build -> Constroi o container
docker run -> Roda o Container. 
    -e -> var de ambiente.
    --env-file -> local de um arquivo com var de ambiente.
    --link -> add link ao container.
    -m -> limite de memória.
    --memory-swap -> limite de memória swap.
    --name -> nome do container.
    -p -> mapeia porta
    --restart -> tipo de renicilização.
    --rm -> mata o processo quando o container é terminado.
    -v -> vincula volume.
    --storage-opt -> opções de starage container.
    -d -> roda o container em background.

docker search mysql
docker pull mysql:5.7
mysql -> docker2309

docker run --name  mysql8 -e MYSQL_ROOT_PASSWORD=docker2309 -p 3308:3308 -d mysql:5.7

docke ps -> exibe containes em andamento.
docker exec -it mysql8 /bin/bash

mysql -uroot -p

docker network inspect bridge

mysql -uroot -p --host=172.17.0.2

docker image build -t python-web-primos .
docker run -p 5001:5000 -d python-web-primos
docker ps
docker logs -f "id container pega pelo comando docker ps"