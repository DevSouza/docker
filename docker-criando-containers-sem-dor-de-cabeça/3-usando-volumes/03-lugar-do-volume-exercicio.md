# Lugar do volume

Um volume fica salvo:

- [ ] A) Na Imagem
> Errado, pois o volume fica no Docker Host. Lembrando, imagens são read-only e não guardam informação após serem construídas.

- [x] B) No Docker Host
> Correto, o volume fica no Docker Host. Ou seja, fica salvo no computador onde a Docker Engine está rodando.

- [ ] No Container
> Errado, pois o volume fica no Docker Host. O container possui apenas o "Link" para o volume.