# 11 Preparando o ambiente: Instalando Docker no MacOs

Vamos agora detalhar o processo de instalação do **Docker for Mac** e do **Docker Toolbox**.

### Instalando com Docker for Mac

Primeiramente você deve se atentar aos requisitos do uso do **Docker for Mac**, ou seja, deve possuir um macOS:

- Modelo 2010 ou mais recente
- Versão OS X El Capitan 10.11 ou mais recente
- Com no mínimo 4GB de memória RAM
- Sem VirtualBox instalada na versão 4.3.30 ou anterior, pois causa incompatibilidade com o Docker

A página dos requisitos pode ser acessada [aqui](https://docs.docker.com/docker-for-mac/install/#what-to-know-before-you-install).

Na página do [Docker for Mac](https://store.docker.com/editions/community/docker-ce-desktop-mac), baixe o instalador clicando [aqui](https://download.docker.com/mac/stable/Docker.dmg). Instale o Docker, clicando no **.dmg** baixado anteriormente e arrastando o Docker para as aplicações. Após isso, pesquise pelo Docker, confirme que quer utilizá-lo e dê acesso privilegiado a ele, clicando em **OK** e digitando a senha de administrador em seguida.

No menu superior do macOS, à direita, o ícone do Docker aparecerá. Ele pode demorar um pouco para inicializar, mas quando a mensagem **Docker is now up and running!** for exibida, significa que ele já pode ser utilizado.

### Instalando com Docker Toolbox

Para instalar o Docker Toolbox, primeiramente baixe-o [aqui](https://download.docker.com/mac/stable/DockerToolbox.pkg).

O **Docker Toolbox** vai instalar tudo que é necessário para que você possa trabalhar com o Docker em seu computador, pois ele irá instalar também a **Oracle VirtualBox**, a máquina virtual da Oracle que vai permitir executar o Docker sem maiores problemas.

A diferença é que, quando você trabalha com o **Docker for Mac**, você pode utilizar o terminal nativo do macOS, pois o terminal está sendo executado dentro do próprio sistema operacional. Já no **Docker Toolbox**, ele instalará o **Docker Machine**, que deverá ser utilizado no lugar do terminal nativo do macOS.