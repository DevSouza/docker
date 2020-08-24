# 08 Reinicializando containers - Exercicio

Ana configurou o ```docker-compose.yml``` corretamente e subiu os containers. Depois de um tempo ela gostaria de reinicializá-los. Para tal, ela executa:

```
docker-compose down
docker-compose up
```

Estes comandos funcionam e não têm nada de errado, mas será que você consegue achar um atalho para isso?

Obs: Não vimos o comando na aula, mas basta executar o comando abaixo para descobrir a resposta:

```docker-compose --help```

- [ ] A) ```docker-compose rerun```
> Errado, ```rerun``` não existe.

- [ ] B) ```docker-compose restore```
> Errado, ```restore``` não existe.

- [ ] C) ```docker-compose resume```
> Errado, ```resume``` não existe.

- [x] D) ```docker-compose restart```
> Correto!