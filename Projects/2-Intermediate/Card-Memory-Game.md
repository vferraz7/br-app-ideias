# Card Memory Game

**Nível:** 2-Intermediário

O jogo de memória de cartas é um jogo onde você precisa clicar em uma
carta para ver qual imagem está embaixo dela and tentar encontrar a
imagem correspondente embaixo das outras cartas.

## Histórias de Usuário

-   [ ] O usuário pode ver uma grade com n x n cartas (`n` é um inteiro).
    Todas as cartas estão viradas para baixo inicialmente (estado `hidden`)
-   [ ] O usuário pode clicar em um botão para iniciar o jogo. Quando este
    botão é clicado, um temporizador iniciará
-   [ ] O usuário pode clicar em qualquer carta para revelar a imagem que
    está embaixo dela (mude para estado `visible`). A imagem será exibida
    até o usuário clicar em uma 2ª carta

Quando o Usuário clica na 2ª carta:

-   [ ] Se houver correspondência, as 2 cartas serão eliminadas do jogo
    (esconda/remova elas ou deixe-as no estado `visible`)
-   [ ] Se não houver correspondência, as 2 cartas voltarão para seu
    estado original (`hidden`)
-   [ ] Quando todas as correspondências forem encontradas, O Usuário pode
    ver uma caixa de diálogo com mensagem de Parabéns com um contador
    exibindo o tempo que levou para terminar o jogo

## Funcionalidades Bônus

-   [ ] O usuário pode escolher entre múltiplos níveis de dificuldade
    (Fácil, Médio, Difícil). Dificuldade aumentada significa:
    diminuição do tempo disponível para completar and/ou aumento do
    número de cartas
-   [ ] O usuário pode ver as estatísticas do jogo (núm. de vezes que
    ganhou / perdeu, melhor tempo para cada nível)

## Links e Recursos Úteis

-   [Wikipedia](<https://en.wikipedia.org/wiki/Concentration_(game)>)

## Projetos de Exemplo

-   [Flip - card memory game](https://codepen.io/zerospree/full/bNWbvW)
-   [Memory Game](https://jdmedlock.github.io/memorygame/)
-   [SMB3 Memory Card Game](https://codepen.io/hexagoncircle/full/OXBJxV)
-   [BHMBS - Memory Game](https://barhouum7.github.io/JS-MemoryGame.github.io/)