# Analisando o Dockerfile

No primeiro dia de trabalho de Fernando, ele encontrou um Dockerfile chamado ```ns.dockerfile```:

```
FROM node:latest
MAINTAINER Ubuntu
COPY . /var/www
WORKDIR /var/www
RUN npm install
ENTRYPOINT npm start
EXPOSE 3000
```

Marque as alternativas verdadeiras sobre o Dockerfile encontrado por Fernando:

- [x] A) A imagem se baseia na imagem node. Inclusive o container se baseará sempre na última versão da imagem.
> Correto.

- [x] B) Todo o conteúdo que será copiado para a imagem ficará dentro da pasta ```/var/www```.
> Correto.

- [ ] C) Em MAINTAINER indicamos a versão do sistema operacional que utilizaremos.
> Completamente errado! Nela indicamos nome do responsável em manter o container. Nesse sentido, o nome ```Ubuntu``` foi utilizado mais para confundir do que para explicar, ao menos que o nome do responsável seja ```Ubuntu```.

- [ ] D) EXPOSE indica quanto tempo o container ficara no ar.
> Errado. Ela indica a porta de acesso do container.