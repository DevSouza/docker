# 08 O que aprendemos?

Neste capítulo aprendemos:

- Que imagens criadas pelo Docker acessam a mesma rede, porém apenas através de IP.
- Ao criar uma rede é possível realizar a comunicação entre os containers através do seu nome.
- Que durante a criação de uma rede precisamos indicar qual driver utilizaremos, geralmente, o driver ```bridge```.

Segue também uma breve lista dos comandos utilizados:

- ```hostname -i``` - mostra o ip atribuído ao container pelo docker (funciona apenas dentro do container).
- ```docker network create --driver bridge NOME_DA_REDE``` - cria uma rede especificando o driver desejado.
- ```docker run -it --name NOME_CONTAINER --network NOME_DA_REDE NOME_IMAGEM``` - cria um container especificando seu nome e qual rede deverá ser usada.