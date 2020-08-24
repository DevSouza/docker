# 04 Novo Dockerfile - Exercicio

Guilherme Nicolau recebeu as seguintes instruções para criação de um docker container:

- Deve instalar o mysql da última imagem disponível
- Os dados iniciais devem ser copiados para a pasta ```/etc/sinc```
- O diretório de trabalho deve ser ```/etc/sinc/plen```
- A porta de comunicação deve ser ```1711```
- O comando de entrada ```chmod 755 /etc/sinc```

Marque a opção que possui a configuração de um Dockerfile condizente com a especificação passada para Guilherme:

- [ ] A) 
```
FROM mysql:latest
MAINTAINER Guilherme Nicolau
COPY . /etc/sinc/plen
WORKDIR /etc/sinc
EXPOSE 1711
```
> Faltou o ENTRYPOINT para definir o comando de entrada

- [x] B)
```
FROM mysql:latest
MAINTAINER Guilherme Nicolau
COPY . /etc/sinc
WORKDIR /etc/sinc/plen
ENTRYPOINT chmod 755 /etc/sinc
EXPOSE 1711
```
> Correto!

- [ ] C)
```
FROM mysql:latest
MAINTAINER Guilherme Nicolau
COPY /etc/sinc/plen
WORKDIR . /etc/sinc
ENTRYPOINT chmod 755 /etc/sinc
EXPOSE 1711
```
> Valores invertidos para COPY e WORKDIR

- [ ] D)
```
FROM mysql:latest
MAINTAINER Guilherme Nicolau
WORKDIR /etc/sinc/plen
ENTRYPOINT chmod 755 /etc/sinc
EXPOSE 1711
```
> Faltou o COPY