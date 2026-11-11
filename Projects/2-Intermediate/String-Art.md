# StringArt

**Nível:** 2-Intermediário

O propósito da String Art é fornecer ao desenvolvedor prática na criação de um gráfico animado simples, usando geometria no algoritmo de animação, e criando algo visualmente agradável de assistir.

A String Art desenha uma única linha multicolorida que se move suavemente até que uma extremidade toque o lado da janela envolvente. No ponto em que toca, um efeito de "rebote" é aplicado para mudar sua direção.

Um efeito de ondulação é criado retendo apenas 10-20 imagens da linha enquanto ela se move. Imagens mais antigas são progressivamente desbotadas até desaparecerem.

Bibliotecas de animação não são permitidas. Use apenas HTML/CSS/JavaScript puros.

## Histórias de Usuário

-   [ ] Comece desenhando uma linha multicolorida em uma posição aleatória dentro do limite de sua janela envolvente
-   [ ] A cada 20ms desenhe uma nova cópia da linha em uma nova posição baseada em uma trajetória - a distância incremental da linha anterior baseada nos pontos finais
-   [ ] Quando qualquer ponto final da linha tocar o limite da janela envolvente, mude sua direção e altere aleatoriamente seu ângulo
-   [ ] Desbote progressivamente a intensidade das linhas antigas para que apenas as 10-20 linhas mais recentes sejam visíveis para criar a sensação de movimento ou "ondulação"

## Funcionalidades Bônus

-   [ ] O usuário pode especificar o comprimento da linha e sua velocidade
-   [ ] O usuário pode especificar múltiplas linhas dentro da janela, todas se movendo ao longo de diferentes trajetórias e velocidades

## Links e Recursos Úteis

-   [Usando Animações e Transições Multietapas](https://css-tricks.com/using-multi-step-animations-transitions/)
-   [Noções Básicas de Animação](https://www.khanacademy.org/computing/computer-programming/programming/animation-basics/a/what-are-animations)

## Projetos de Exemplo

Este projeto é muito próximo, mas tem uma janela envolvente pequena e é monocromático.
[Daniel Cortes](https://codepen.io/dgca/pen/dpxreO)