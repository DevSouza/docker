# 02 Sobre volumes - Exercicio

Por que usamos volumes?

- [ ] A) Containers não guardam nenhum dado (são read-only) e por isso precisamos de volumes.
> Containers não são necessariamente read-only, como já vimos nesse curso. Você pode guardar dados dentro do container desde que não apague ele após o uso.

- [x] B) Muitas vezes removemos os containers após o uso. Volumes são usados para os dados que não devem ser removidos.
> Correto, é muito comum usar o container e apagá-lo após seu uso. Dessa forma também são removidos os dados desse container e aí entram os volumes que permitem salvar dados fora do container.

- [ ] C) O uso dos volumes simplifica a execução pois não precisamos mais de imagens.
> Errado, as imagens continuam sendo utilizadas e são necessárias.