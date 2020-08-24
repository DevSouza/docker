# 03 Criando uma rede - Exercicio

Emanuelle decidiu criar uma nova rede para que pudesse realizar a comunicação entre containers através dela. Então, ela executou o seguinte comando:

```docker network create --driver bridge local```

Marque as alternativas verdadeiras a respeito do comando executado por Emanuelle.

- [x] A) A instrução ```create``` não é opcional.
> Correto, sem ela não será possível criar a rede.

- [ ] B) Cria uma rede local chamada ```bridge```.
> Falsa. ```bridge``` é o driver utilizado, a rede criada se chama de ```local```.

- [ ] C) Utiliza o driver ```local```.
> Falsa. O driver utilizado é o ```bridge```, a rede criada se chama de ```local```.

- [x] D) O parâmetro ```--driver``` indica qual driver será utilizado durante a criação da rede local.
> Correto.