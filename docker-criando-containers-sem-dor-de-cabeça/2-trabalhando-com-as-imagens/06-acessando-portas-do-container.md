# 06 Acessando portas do container - Exercicio

Luis resolveu acessar sua aplicação, chamada de **MinhaAplicacao** e que está dentro do container, utilizando a porta **8080** a partir de sua máquina. Porém, como é novo no ramo do Docker, ele está em dúvida sobre qual comando deve utilizar para saber quais são as portas mapeadas. Marque a opção que realiza o desejo de Luis:

- [ ] A) Luis deve usar o comando docker run MinhaAplicacao.
> Errado. Este comando é para executar um container com uma respectiva imagem.

- [x] B) Luis deve usar o comando ```docker port ID_DO_CONTAINER``` para que possa saber qual porta de sua máquina faz referência à porta 8080 de seu container.
> Certo!

- [ ] C) Luis deve usar o comando docker rmi MinhaAplicacao.
> Errado. Este comando é para remover uma imagem passada como parâmetro.