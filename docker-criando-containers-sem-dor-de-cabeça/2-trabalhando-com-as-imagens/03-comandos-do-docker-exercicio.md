# 03 Comandos do Docker Exercicio

Temos os seguintes comandos do Docker e suas respectivas funcionalidades:

1) O comando ```docker ps``` nos permite ver todos os container já criados

2) O comando ```docker rm ID_DO_CONTAINER``` remove um container

3) O comando ```docker container prune``` permite remover todos os containers inativos de uma só vez.

Quais funcionalidades, e seus respectivos comandos, estão corretas?

> A) Funcionalidade 1
    > Alternativa errada! A funcionalidade 1 está errada, pois o comando ```docker ps``` mostra apenas os containers em execução. O correto então é ```docker ps -a```. A flag ```-a``` faz com que ps mostre todos os containers. Alternativamente você pode usar: ```docker ps --all```.

> B) Funcionalidade 3
> Alternativa correta! O comando ```docker container prune``` realmente apaga todos os containers inativos, mas dá um aviso antes.

> C) Funcionalidade 2
> Alternativa correta! O comando ```docker rm ID_DO_CONTAINER``` permite remover um container especifico.