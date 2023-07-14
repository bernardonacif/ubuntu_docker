# ubuntu_docker
scripts para subir e configurar um Container Docker com a Imagem do Ubuntu e configurando um ambiente virtual Python

Anotações: 

Todos os comandos estão duplicados, onde a primera linha você deve subistituir <nome_do_contêiner> pelo nome do seu container criado ou se quiser aproveitar o nome ja estou utilizando em todo o projeto, basta sempre utilizar o script da segunda linha.

1- Na pasta com o arquivo docker_compose.yml configurado para seu ambiente, execute via bash o seguinte comando para subir o container:

docker-compose up -d

Caso queira subir e já iniciar a linha de comando junto:

docker-compose exec <nome_do_contêiner> bash

docker-compose exec ubuntu-container bash

2- Para acessar via bash:

docker exec -it <nome_do_contêiner> bash

docker exec -it ubuntu_dev bash

3- Habilitar execução de scripts via bash:

chmod +x setup.sh

4- Executar o script update_and_install_python.sh

