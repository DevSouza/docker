# Interpretando o Inspect - Exercicio

Flavio é um programador com muita experiência no mundo Javascript, porém agora resolveu se aventurar no mundo do Docker. Ao pensar em como iria organizar os caminhos dos volumes em sua máquina e container, ele executou o comando ```docker inspect```. Abaixo temos um pedaço da saída do comando ```docker inspect ID_DO_CONTAINER``` no terminal de Flavio, sobre a saída abaixo é verdade que:

```
"Mounts": [
    {
        "Type": "volume",
        "Name": "5e1cbfd48d07284680552e56087c9d5196659600ccd6874bfa3831b51ddd0576",
        "Source": "/home/Flavio/Desktop/volumes/caminho/_data",
        "Destination": "/var/opt",
        "Driver": "local",
        "Mode": "",
        "RW": true,
        "Propagation": ""
    }
]
```

- [ ] A) "/var/opt" e "/home/Flavio/Desktop/volumes/caminho/_data" pertencem ao container.
> Uma delas pertence à máquina.

- [ ] B) "/var/opt" e "/home/Flavio/Desktop/volumes/caminho/_data" pertencem à máquina.
> Uma delas pertence ao container.

- [ ] C) "/home/Flavio/Desktop/volumes/caminho/_data" pertence ao container e será armazenado no caminho "/var/opt" em nossa máquina.
> Errado, "/var/opt" pertence ao container.

- [x] D) "/var/opt" pertence ao container e será escrito no caminho "/home/Flavio/Desktop/volumes/caminho/_data" em nossa máquina.
> Correto! "/var/opt" pertence ao container enquanto "/home/Flavio/Desktop/volumes/caminho/_data" pertence à máquina e irá armazenar "/var/opt".