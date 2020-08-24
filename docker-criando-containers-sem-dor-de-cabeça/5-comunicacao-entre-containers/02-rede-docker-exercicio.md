# 02 Rede Docker - Exercicio

Marque as alternativas verdadeiras a respeito de uma Rede Docker:

- [x] A) Por padrão, os containers ficam na mesma rede com o nome ```bridge```.
> Correto. Porém, a comunicação deve ser feita através de IP.

- [x] B) Na rede padrão do Docker, só podemos realizar a comunicação utilizando IPs.
> Exatamente. Se criarmos nossa própria rede podemos usar seu nome no lugar do IP.

- [x] C) Com ```docker inspect ID_DO_CONTAINER``` podemos verificar a qual rede ele pertence.
> Exatamente, o comando ```inspect``` mostra vários detalhes sobre o container, entre eles o ```network```. Nesse item, aparece o nome da nossa rede, IP do container, o gateway e entre outras informações.

- [ ] D) A rede padrão deve ser habilitado explicitamente para funcionar.
> Errado, pois já está habilitado por padrão.