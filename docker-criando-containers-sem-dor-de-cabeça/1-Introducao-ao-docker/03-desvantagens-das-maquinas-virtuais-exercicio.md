# Desvantagens das máquinas virtuais - Exercicio

Vimos que utilizar um servidor físico separado para cada serviço do nosso sistema gera vários problemas, entre eles o custo de luz e rede, e o seu alto tempo de ociosidade.  

A solução para esses problemas foi a **virtualização** dos recursos físicos, reduzindo assim os custos de luz e rede, já que não teremos mais vários servidores físicos, e não teremos mais ociosidade do hardware.  

Mas as máquinas virtuais também possuem problemas, que estão listados abaixo, **exceto um**. Qual?  

- [ ] A) Como as máquinas virtuais possuem sistemas operacionais, os mesmos possuem um custo de hardware para manter suas funcionalidades.
> Esse é um problema das máquinas virtuais! Precisamos instalar um sistema operacional em cada uma delas, que por sua vez possui um custo de hardware para funcionar. Se houver várias máquinas virtuais, o seu custo de manutenção acaba se tornando bem alto.
  
- [ ] B) Como as máquinas virtuais possuem sistemas operacionais, os mesmos possuem configurações iniciais a serem feitas, e devem ser atualizados com frequência.  
> Esse é um problema das máquinas virtuais! Como devemos instalar sistemas operacionais nelas, eles devem ser configurados (liberação de portas, instalação de bibliotecas, etc) e estar sempre atualizados, principalmente por questões de segurança.

- [ ] C) Manter vários sistemas operacionais requer muito tempo de trabalho, chegando a equivaler ao tempo requerido para manter as aplicações
> Esse é um problema das máquinas virtuais! Manter vários sistemas operacionais gera trabalho, consumindo tempo que poderia estar sendo utilizada para manter/criar aplicações.

- [x] D) A dificuldade em fazer um backup dos dados.  
> Esse não é um problema das máquinas virtuais! O backup dos dados de uma máquina virtual pode ser feito com certa facilidade, seja por softwares externos ou através das próprias VMs.