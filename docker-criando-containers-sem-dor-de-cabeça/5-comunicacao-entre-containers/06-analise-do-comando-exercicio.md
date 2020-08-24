# 06 Análise do comando - Exercicio

Eric, para testar sua amiga Paula, executou o seguinte comando:

```docker run -d --name meu-mongo --network minha-rede mongo```

Em seguida, pediu para que Paula detalhasse o comando executado.

Nesse contexto, marque as afirmativas verdadeiras a respeito do comando executado:

- [x] A) Sobe um container na rede minha-rede.
> Correto.

- [ ] B) Executa o container na rede ```mongo```.
> A rede é ```minha-rede```.

- [x] C) Executa o container em modo ```detached```.
> Correto.

- [ ] D) É um comando inválido, pois o parâmetro ```-d``` não é suportado.
> Falso, o comando ```-d``` é suportado sim, ele realiza uma execução ```detached``` do container. Dessa maneira, podemos continuar a usar o terminal.