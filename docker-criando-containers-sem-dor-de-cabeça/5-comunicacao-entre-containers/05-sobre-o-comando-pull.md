# 05 Sobre o comando pull

No último video usei o comando docker pull ```douglasq/alura-books:cap05``` sem ter explicado antes. Fique tranquilo pois esse comando faz nada mais do que baixar, sem rodar, a imagem desejada do Docker Hub :)

Por exemplo, para baixar a imagem ```ubuntu``` do Docker Hub você pode usar:

```docker pull ubuntu```
Isso é diferente do comando ```run```, que baixa a imagem (se não existe local) e depois cria e roda o container. O ```pull``` apenas baixa!

Para baixar uma imagem de um usuário especifico vimos a sintaxe:

```docker pull NOME_USUARIO/NOME_IMAGEM```
Além disso, uma imagem pode ter um **tag** que serve para pegar uma determinada versão dessa imagem. Alias, você já viu a tag ```:latest``` e no video eu usei a tag ```:cap05```, por exemplo:

```docker pull douglasq/alura-books:cap05```

Isso baixará a versão (ou tag) ```cap05``` da imagem ```alura-books``` do usuário ```douglasq```.