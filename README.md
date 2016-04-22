# docker_mysql

Projeto para criar container mysql usando docker

Comando para criar imagem mysql:

$ docker build -t mysql .

Comando para iniciar container:

$ docker run -d -p 3306:3306 -e MYSQL_ROOT_PASSWORD=xpto1234 mysql

Comando para acessar banco de dados mysql no host mac os:

$ mysql -h $(docker-machine ip default) -P 3306 -u root -p