# Engine de Jogo de Batalha Naval

**Nível:** 3-Avançado

O Engine de Jogo de Batalha Naval (BGE) implementa o clássico jogo de tabuleiro baseado em turnos como um pacote separado de qualquer camada de apresentação. Este é um tipo de padrão arquitetural útil em muitas aplicações, pois permite que qualquer número de apps utilize o mesmo serviço.

O BGE em si é invocado através de uma série de chamadas de função em vez de ações do usuário final diretamente acopladas. Neste aspecto, usar o BGE é semelhante a usar uma API ou uma série de rotas expostas por um servidor web.

Este desafio requer que você desenvolva o BGE e uma camada de apresentação baseada em texto muito fina para testes, separada do próprio engine. Devido a isso, as Histórias de Usuário abaixo são divididas em dois conjuntos - um para o BGE e outro para a camada de apresentação baseada em texto.

O BGE é responsável por manter o estado do jogo.

## Histórias de Usuário

### BGE

-   [ ] O chamador pode invocar uma função `startGame()` para iniciar um jogo de 1 jogador. Esta função gerará um tabuleiro de jogo 8x8 consistindo de 3 navios com largura de um quadrado e comprimento de:

    -   Destroyer: 2 quadrados
    -   Cruzador: 3 quadrados
    -   Couraçado: 4 quadrados

    `startGame()` colocará estes navios aleatoriamente no tabuleiro em qualquer direção e retornará um array representando a colocação dos navios.

-   [ ] O chamador pode invocar uma função `shoot()` passando as coordenadas de linha e coluna da célula alvo no tabuleiro de jogo. `shoot()` retornará indicadores representando se o tiro resultou em acerto ou erro, o número de navios restantes (ou seja, ainda não afundados), o array de colocação dos navios, e um array atualizado de acertos e erros.

    Células no array de acertos e erros conterão um espaço se ainda não foram alvejadas, `O` se foram alvejadas mas nenhuma parte de um navio estava naquele local, ou `X` se a célula era ocupada por parte de um navio.

### Camada de Apresentação Baseada em Texto

-   [ ] O usuário pode ver o array de acertos e erros exibido como uma representação de caracteres 2-dimensional do tabuleiro de jogo retornado pela função `startGame()`.
-   [ ] O usuário pode ser solicitado a inserir as coordenadas de um quadrado alvo no tabuleiro de jogo.
-   [ ] O usuário pode ver um array de acertos e erros atualizado após fazer um tiro.
-   [ ] O usuário pode ver uma mensagem após cada tiro indicando se o tiro resultou em acerto ou erro.
-   [ ] O usuário pode ver uma mensagem de parabéns após o tiro que afunda o último navio restante.
-   [ ] O usuário pode ser solicitado a jogar novamente ao final de cada jogo. Recusar a jogar novamente encerra o jogo.

## Funcionalidades Bônus

### BGE

-   [ ] O chamador pode especificar o número de linhas e colunas no tabuleiro de jogo como parâmetro para a função `startGame()`.
-   [ ] O chamador pode invocar uma função `gameStats()` que retorna um objeto JavaScript contendo métricas do jogo atual. Por exemplo, número de turnos jogados, número atual de acertos e erros, etc.
-   [ ] O chamador pode especificar o número de jogadores (1 ou 2) ao chamar `startGame()`, que gerará um tabuleiro para cada jogador populado aleatoriamente com navios.

    `shoot()` aceitará o número do jogador para o qual o tiro está sendo feito junto com as coordenadas do tiro. Os dados que ele retorna serão para aquele jogador.

### Camada de Apresentação Baseada em Texto

-   [ ] O usuário pode ver as estatísticas atuais do jogo a qualquer momento digitando a palavra `stats` no lugar das coordenadas do alvo. (Note que isso requer a função `gameStats()` no BGE)
-   [ ] O usuário pode especificar que um jogo de dois jogadores será jogado, com cada jogador alternando turnos na mesma sessão do terminal (Note que isso requer as Funcionalidades Bônus correspondentes no BGE)
-   [ ] O usuário pode ver o número do jogador nos prompts associados às entradas em cada turno.
-   [ ] O usuário pode ver os tabuleiros de ambos os jogadores ao final de cada turno.

## Links e Recursos Úteis

-   [Jogo de Batalha Naval (Wikipedia)](<https://en.wikipedia.org/wiki/Battleship_(game)>)
-   [Regras do Jogo de Batalha Naval (Hasbro)](https://www.hasbro.com/common/instruct/battleship.pdf)

## Projetos de Exemplo

Este vídeo do YouTube mostra como um [Jogo de Batalha Naval](https://www.youtube.com/watch?v=TKksu3JXTTM) baseado em texto é jogado.

O exemplo a seguir é fornecido como demonstração do jogo de Batalha Naval caso você não esteja familiarizado com ele. Lembre-se que você deve implementar uma camada de apresentação baseada em texto para testes.

-   [Jogo de Batalha Naval por Chris Brody](https://codepen.io/CodifyAcademy/pen/ByBEOz)