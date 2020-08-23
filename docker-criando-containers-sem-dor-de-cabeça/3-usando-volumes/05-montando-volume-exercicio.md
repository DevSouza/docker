# 05 Montando volume - Exercicio

Qual dos comandos abaixo configura o volume do diretório ```/var/www``` do container para ```C:\logs``` do Host?


- [ ] A) ```docker run -v "/var/www" ubuntu```
> Errado, mas o comando não vai dar erro, mas para usar a pasta ```C"\logs``` devemos usar:   ```docker run -v "C:\logs:/var/www" ubuntu```

- [] B) ```docker run -v "C:\logs" ubuntu```
> Errado, devemos usar a flag ```-v``` seguindo pelo ```CAMINHO_HOST:CAMINHO_CONTAINER```:

- [x] C) ```docker run -v "C:\logs:/var/www" ubuntu```
> Correto, usando a flag ```-v``` seguindo pelo ```CAMINHO_HOST:CAMINHO_CONTAINER```.

- [ ] D) ```docker run "C:\logs:/var/www" ubuntu```
> Errado, faltou a flag ```-v```.