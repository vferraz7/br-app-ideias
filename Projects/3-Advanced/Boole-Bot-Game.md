# Jogo Boole Bots

**Nível:** 3-Avançado

Boole Bots é um jogo que não é apenas divertido, mas também um auxílio para ajudar a entender a lógica booleana básica. Este jogo tem uma arena de 8x8 ladrilhos de jogo nos quais seus bots se movem em velocidades e trajetórias aleatórias. Os Bots recebem valores booleanos 0 ou 1 e operações booleanas - AND, OR, NOR, NOT.

Quando um bot colide com outro bot, sua operação booleana é aplicada a ambos, seu valor booleano e o do outro bot, para determinar qual vence ou perde, ou se a colisão resulta em empate. Bots perdedores desaparecem e bots vencedores continuam se movendo pela arena até que apenas um reste.

### Requisitos e Restrições

- Desenvolvedores podem usar bibliotecas de gráficos e física de jogos para construir o jogo.

## Histórias de Usuário

-   [ ] O usuário pode ver a janela do jogo com estes componentes
    - Painel de entrada de configuração do jogo
    - Ranking mostrando bots ordenados por suas pontuações
    - Controles do jogo
    - Arena de 8x8 ladrilhos de jogo onde os bots batalham

### Painel de Configuração do Jogo
-   [ ] O usuário pode ver um painel de configuração do jogo com estes subcomponentes:
    - Quatro painéis de bot com controles para permitir que o usuário insira um nome único de bot, selecione seu valor e operação booleana, selecione a velocidade do bot usando um controle deslizante, e uma lista suspensa para especificar sua direção inicial - Norte, Sul, Leste, Oeste
-   [ ] O usuário pode inserir um nome único para cada bot em uma caixa de texto
-   [ ] O usuário pode ver uma mensagem de erro se o nome inserido for o mesmo nome atribuído a outro bot.
-   [ ] O usuário pode selecionar o valor booleano do bot (0 ou 1) em uma lista suspensa.
-   [ ] O usuário pode selecionar uma operação booleana do bot em uma lista suspensa - AND, OR, XOR, ou NOT.
-   [ ] O usuário pode mover o controle deslizante de velocidade para definir a velocidade de um bot
-   [ ] O usuário pode selecionar a direção inicial de um bot na lista suspensa de direção.
-   [ ] O usuário pode ver o bot atribuído aleatoriamente a um ladrilho na arena uma vez que seu nome foi definido.

### Controles do Jogo
-   [ ] O usuário pode ver um botão no painel de controle do jogo para 'Batalhar!'
-   [ ] O usuário pode clicar no botão 'Batalhar!' para iniciar a batalha dos bots na arena.
-   [ ] O usuário pode ver os bots se moverem com base na velocidade e direção atribuídas a eles.
-   [ ] O usuário pode ver o texto do botão 'Batalhar!' mudar para 'Parar!' uma vez que uma batalha é iniciada.
-   [ ] O usuário pode clicar no botão 'Parar!' para interromper o jogo
-   [ ] O usuário pode ver o texto do botão 'Parar!' voltar para 'Batalhar!' uma vez que um único bot vence a partida.

### Arena
-   [ ] O usuário pode ver os bots ricochetearem nas paredes de fronteira da arena em uma nova direção
-   [ ] O usuário pode ver os bots pausarem por um instante quando colidem.
-   [ ] O usuário pode ver um bot desaparecer após colidir se o resultado de sua operação booleana aplicada ao seu valor booleano e ao do bot com o qual colidiu resultar em 0.
-   [ ] O usuário pode ver um bot que vence uma colisão retomar seu caminho na mesma velocidade e direção.
-   [ ] O usuário pode ver ambos os bots em colisão retomarem seus caminhos na mesma velocidade e direção no caso de empate. Em outras palavras, quando a colisão resultou no mesmo resultado booleano (0 ou 1) para ambos.
-   [ ] O usuário pode ver o jogo parar quando apenas um bot resta.

### Ranking
-   [ ] O usuário pode ver a exibição de vitórias e derrotas para cada bot no ranking
-   [ ] O usuário pode ver a contagem de vitórias incrementada para bots que vencem uma colisão.
-   [ ] O usuário pode ver a contagem de derrotas decrementada para bots que perdem uma colisão.

## Funcionalidades Bônus

-   [ ] O usuário pode ver um painel de log exibindo os detalhes dos marcos do jogo. Dica: Isso pode ser útil para o Desenvolvedor durante o desenvolvimento e depuração.
-   [ ] O usuário pode ver um relógio do jogo exibindo o tempo de jogo decorrido atual que é atualizado a cada segundo.
-   [ ] O usuário pode escolher a direção inicial de um bot como Norte, Nordeste, Sudeste, Sul, Sudoeste, Oeste, ou Noroeste.
-   [ ] O usuário pode especificar as dimensões da arena.
-   [ ] O usuário pode selecionar um ícone único para um bot a partir de uma paleta de ícones. Ícones na paleta são desabilitados uma vez atribuídos.
-   [ ] O usuário pode ver o bot com mais vitórias destacado de alguma forma no Ranking.

## Links e Recursos Úteis

- [George Boole (Wikipedia)](https://en.wikipedia.org/wiki/George_Boole)
- [Álgebra Booleana (Wikipedia)](https://en.wikipedia.org/wiki/Boolean_algebra)
- [Tutorial de Física de Jogos - Parte I: Introdução à Dinâmica de Corpos Rígidos](https://www.toptal.com/game/video-game-physics-part-i-an-introduction-to-rigid-body-dynamics)

## Projetos de Exemplo

- N/a