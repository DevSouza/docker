# 03 Análise de um DockerFile

Vejamos um exemplo de um dockerfile que utiliza a última imagem disponível do nginx:

```
FROM nginx:latest
MAINTAINER Douglas Quintanilha
COPY /public /var/www/public
COPY /docker/config/nginx.conf /etc/nginx/nginx.conf
EXPOSE 80 443
ENTRYPOINT ["nginx"]
CMD ["-g", "daemon off;"]
```

Marque as alternativas verdadeiras sobre o arquivo:

- [x] A) Utilizamos a última versão disponível da imagem do nginx como base

- [ ] B) Apenas a porta 80 é aberta.
> O comando EXPOSE abre as portas 80 e 443.

- [x] C) Copiamos o conteúdo da pasta public, que contém os arquivos estáticos, e um arquivo de configuração do NGINX para dentro do container.

- [x] D) É executado o comando nginx, passando os parâmetros extras -g e daemon off.