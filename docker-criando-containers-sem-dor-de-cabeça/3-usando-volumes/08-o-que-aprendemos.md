# O que aprendemos?

Nessas aulas avançamos bastante e aprendemos:

- Que Container são voláteis, isso é, ao remover um, removemos os dados juntos
- Para deixar os dados persistente devemos usar **Volumes**
- Que volumes salvos não ficam no container e sim no Docker Host
- Como criar um ambiente de execução node.js

Segue também uma breve lista dos comandos utilizados:

- ```docker run -v "[CAMINHO_VOLUME_LOCAL:]CAMINHO_VOLUME_CONTAINER" NOME_DA_IMAGEM``` - cria um volume no respectivo caminho do container, caso seja especificado um caminho local monta o volume local no volume do container.
- ```docker inspect ID_CONTAINER``` - retorna diversas informações sobre o container.