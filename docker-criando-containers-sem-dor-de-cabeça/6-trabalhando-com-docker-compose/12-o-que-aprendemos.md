# 12 O que aprendemos?

Nessa aula aprendemos:

- A necessidade de usar o Docker Compose
- Configurar o build de vários containers através do ```docker-compose.yml```
- subir e parar os containers de maneira coordenada com Docker Compose

Segue também uma breve lista dos novos comandos utilizados:

- ```docker-compose up``` - sobe os serviços criados
- ```docker-compose down``` - para os serviços criados.
- ```docker-compose ps``` - lista os serviços que estão rodando.
- ```docker exec -it alura-books-1 ping node2-``` executa o comando ```ping node2``` dentro do container ```alura-books-1```