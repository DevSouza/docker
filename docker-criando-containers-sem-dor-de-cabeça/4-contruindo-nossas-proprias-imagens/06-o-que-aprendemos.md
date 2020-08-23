# O que aprendemos?

Aprendemos neste capítulo:

- A entender o papel do arquivo DockerFile para criar imagens.
  - O Dockerfile define os comandos para executar instalações complexas e com características específicas.
- Vimos os principais comandos como ```FROM```, ```MAINTAINER```, ```COPY```, ```WORKDIR```, ```RUN```, ```EXPOSE``` e ```ENTRYPOINT```
- A subir uma imagem criada através de um Dockerfile para o Docker Hub e disponibilizar para os desenvolvedores

Lembrando também:

- as imagens são read-only sempre
- um container é uma instância de uma imagem
- para guardar as alterações a docker engine cria uma nova layer em cima da última layer da imagem

Segue também uma breve lista dos comandos utilizados:

- ```docker build -f Dockerfile``` - cria uma imagem a partir de um Dockerfile.
- ```docker build -f CAMINHO_DOCKERFILE/Dockerfile -t NOME_USUARIO/NOME_IMAGEM``` - constrói e nomeia uma imagem não-oficial informando o caminho para o Dockerfile.
- ```docker login``` - inicia o processo de login no Docker Hub.
- ```docker push NOME_USUARIO/NOME_IMAGEM``` - envia a imagem criada para o Docker Hub.
- ```docker pull NOME_USUARIO/NOME_IMAGEM``` - baixa a imagem desejada do Docker Hub.