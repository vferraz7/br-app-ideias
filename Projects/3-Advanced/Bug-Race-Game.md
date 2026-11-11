# Corrida de Insetos

**Nível:** 3-Avançado

Neste projeto você testará suas habilidades de animação criando um jogo que permite ao usuário fazer insetos correrem enquanto tenta adivinhar o vencedor. Como parte disso, você precisará fornecer ao usuário vários controles que permitem personalizar o jogo, incluindo ícones de insetos, atribuição de nomes aos insetos, escolha de quem pode ser o vencedor, e velocidade dos insetos.

### Restrições
- O desenvolvedor precisará selecionar os ícones de insetos a serem usados no jogo
- O desenvolvedor deve ajustar aleatoriamente a velocidade de cada inseto antes de uma corrida começar para que eles viajem em taxas diferentes dentro da velocidade selecionada pelo usuário (lento, normal, ou rápido).
- Cabe ao desenvolvedor definir os intervalos de velocidade associados às configurações lento, normal e rápido.
- Você pode usar uma biblioteca de animação, mas tirará mais proveito deste projeto se tentar implementá-lo usando recursos nativos da linguagem.

## Histórias de Usuário

-   [ ] O usuário pode ver:
    - Um painel de entrada contendo controles para configurar a UI e operação do jogo.
    - Uma pista de corrida consistindo de quatro faixas horizontais nas quais os insetos viajarão
    - Um botão de rádio associado a cada faixa para permitir que o usuário selecione um vencedor potencial
    - Um botão 'Iniciar'.

### Controles do Jogo
-   [ ] O usuário pode ver os seguintes controles no painel de entrada.
    - Uma lista de números das faixas de corrida com botões de rádio para cada uma mostrando miniaturas de três insetos únicos, e uma caixa de texto que o usuário pode usar para dar um nome ao inseto.
    - Um controle de seleção de velocidade com três botões de rádio - Lento, Normal, Rápido
-   [ ] O usuário pode clicar em um botão de rádio para selecionar o ícone do inseto a ser atribuído a uma faixa.
-   [ ] O usuário pode ver uma mensagem de aviso se o mesmo ícone for selecionado para mais de uma faixa.
-   [ ] O usuário pode inserir um nome para o inseto em cada faixa.
-   [ ] O usuário pode ver uma mensagem de erro se o mesmo nome for repetido para mais de um inseto.
-   [ ] O usuário pode selecionar a velocidade do inseto clicando em um dos botões de rádio de Velocidade

### Corrida

-   [ ] O usuário pode selecionar um vencedor potencial clicando no botão de rádio em qualquer faixa.
-   [ ] O usuário pode iniciar uma corrida clicando no botão 'Iniciar'
-   [ ] O usuário pode ver o botão 'Iniciar' desabilitado até que a corrida termine
-   [ ] O usuário pode ver uma mensagem de erro se nenhum vencedor foi selecionado.
-   [ ] O usuário pode ver os insetos correrem através de suas faixas atribuídas até a linha de chegada
-   [ ] O usuário pode ver todos os insetos pararem de se mover quando o primeiro alcança a linha de chegada
-   [ ] O usuário pode ver as métricas do jogo atualizadas para mostrar o número de corridas executadas nesta sessão.

## Funcionalidades Bônus

-   [ ] O usuário pode ver métricas de corrida para cada inseto mostrando o número de corridas executadas, número de vitórias, e número de derrotas.
-   [ ] O usuário pode ver o inseto vencedor quicar quando vence uma corrida
-   [ ] O usuário pode ver os insetos perdedores virarem de costas quando perdem uma corrida
-   [ ] O usuário pode ouvir sons únicos tocados quando a corrida inicia e termina.

## Links e Recursos Úteis

- [Imagens de Insetos 3D](https://www.google.com/search?q=3d+bug+drawings&tbm=isch&source=hp&sa=X&ved=2ahUKEwjxkNT7--jhAhUI-6wKHW3_CgQQsAR6BAgHEAE&biw=1279&bih=550)
- [Animações Básicas (MDN)](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_animations)
- [Como Construir uma Animação de Sprite Simples em JavaScript](https://medium.com/dailyjs/how-to-build-a-simple-sprite-animation-in-javascript-b764644244aa)
- [Animações em JavaScript](https://javascript.info/animation)

## Projetos de Exemplo

- [Jogo Arcade](https://jdmedlock.github.io/arcadegame/)
- [Animação de Corrida de Arrancada](https://codepen.io/Delime/pen/IyuAr)
- [Corrida de Cavalos](https://codepen.io/nathanielzanzouri/pen/jVgEZY)