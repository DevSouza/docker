# Comandos Basicos na ordem de aprendizado da alura

### Aula 1 Hello world
- Comando para buscar/rodar um determinado container ``` docker run hello-world ```
  com esse comando caso o docker não encontre nenhuma imagem localmente ele busca no dockerhub a imagem com o nome de 'hello-world'
  e cria e inicia um container com essa imagem
  
### Comandos basicos com container

- Buscando e cria uma imagem do ubuntu ``` docker run ubuntu ``` (Obs: A imagem do ubunto ela não executa nada por padrão, com isso ele cria o container mas não exibe nada).

- Listar todos os containers que estão ativos no momento ``` docker ps ```
- Listar todos os containers que foram criados (Ativos e inativos) ``` docker ps -a ```
- Rodando o container do ubuntu e mandando ele executar um determinado comando ``` docker run ubuntu echo "Olá mundo" ```

- Criando um container Ubuntu com terminal interativo(terminal interativo serve para atrelar o terminal do computador com o do container) ``` docker run -it ubuntu ```
- Atalho para fechar um terminal interativo ``` Ctrl + d ``` ou digitar ``` exit``` no terminal

- Comando para iniciar um container ja criado ``` docker start CONTAINTER_ID ``` o container id pode ser encontrado com o seguinte comando ``` docker ps -a ```
- Comando para matar um container ``` docker stop CONTAINER_ID ```
- Comando para iniciar um container ja criado com o terminal Attach e interativo ``` docker start -a -i CONTAINER_ID ```

- Comando para remover um container do computador ```docker rm CONTAINER_ID ```
- Comando para limpar todos os containers inativos/stopped ``` docker container prune ```

- Comando para listar todas as imagens que foram baixadas ``` docker images ```
- Comando para remover uma imagem ``` docker rmi NOME_DA_IMAGEM ``` (obs o nome da imagem pode se encontrado com o comando ``` docker images ```  na coluna 'REPOSITORY')

### Layered File System

Toda imagem pode ser composta por uma ou mais camada. com isso se for criado 3 containers com a imagem do ubuntu, todos eles compartilham a mesma base(Read only),   
e é criada uma camada fina (Read write) para que cada container manipule seus proprios arquivos.

### Praticando com o docker run

