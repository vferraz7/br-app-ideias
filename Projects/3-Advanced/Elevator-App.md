# Elevador

**Nível:** 3-Avançado

É difícil imaginar um mundo sem elevadores. Especialmente se você tem que subir e descer 20 andares de escada todos os dias. Mas, se você pensar sobre isso, elevadores foram uma das implementações originais de eventos e manipuladores de eventos muito antes de aplicações web entrarem em cena.

O objetivo do app Elevador é simular a operação de um elevador e, mais importante, como lidar com os eventos gerados quando os ocupantes do prédio o usam. Este app simula ocupantes chamando um elevador de qualquer andar e pressionando os botões dentro do elevador para indicar o andar para o qual desejam ir.

### Restrições

- Você deve implementar um único manipulador de eventos para os botões de subir e descer em cada andar. Por exemplo, se houver 4 andares, um único manipulador de eventos deve ser implementado em vez de 8 (dois botões por andar).
- Da mesma forma, um único manipulador de eventos deve ser implementado para todos os botões no painel de controle no elevador em vez de um manipulador de eventos único para cada botão.

## Histórias de Usuário

-   [ ] O usuário pode ver um diagrama de seção transversal de um prédio com quatro andares, um poço de elevador, o elevador, e um botão de subir no primeiro andar, botões de subir e descer no segundo e terceiro andares, e um botão de descer no quarto andar.
-   [ ] O usuário pode ver o painel de controle do elevador com um botão para cada um dos andares ao lado do diagrama.
-   [ ] O usuário pode clicar nos botões de subir e descer em qualquer andar para chamar o elevador.
-   [ ] O usuário pode esperar que clicar nos botões de subir e descer em qualquer andar para solicitar o elevador será enfileirado e atendido na sequência em que foram clicados.
-   [ ] O usuário pode ver o elevador mover-se para cima e para baixo no poço até o andar para o qual foi chamado.
-   [ ] O usuário pode clicar no painel de controle do elevador para selecionar o andar para o qual ele deve viajar.
-   [ ] O usuário pode esperar que o elevador pause por 5 segundos esperando que um botão de andar no painel de controle seja clicado. Se um botão de andar não for clicado dentro desse tempo, o elevador processará a próxima solicitação de chamada.
-   [ ] O usuário pode esperar que o elevador retorne ao primeiro andar quando não houver solicitações para processar.

## Funcionalidades Bônus

-   [ ] O usuário pode ouvir um som de aviso se o número de solicitações do elevador exceder o máximo permitido. Este limite fica a cargo do desenvolvedor.
-   [ ] O usuário pode ouvir um som quando o elevador chega a um andar.
-   [ ] O usuário pode ver um ocupante chegar aleatoriamente a um andar para indicar quando o usuário deve clicar no botão de chamada do elevador para subir ou descer naquele andar.
-   [ ] O usuário pode especificar o intervalo de tempo entre novos ocupantes chegando para chamar um elevador.

## Links e Recursos Úteis

[Fila First-in, first out (Wikipedia)](https://en.wikipedia.org/wiki/FIFO_(computing_and_electronics))

## Projetos de Exemplo

[Elevador](https://codepen.io/nibalAn/pen/prWdjq)