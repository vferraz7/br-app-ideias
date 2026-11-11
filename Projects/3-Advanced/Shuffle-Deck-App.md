# Embaralhar Baralho de Cartas

**Nível:** 3-Avançado

Como Desenvolvedor Web, você será solicitado a criar aplicações inovadoras que resolvem problemas do mundo real para pessoas reais. Mas algo que você aprenderá rapidamente é que não importa quantos recursos maravilhosos você coloque em um app, os usuários não o usarão se ele não tiver desempenho. Em outras palavras, existe uma ligação direta entre como um app performa e se os usuários o percebem como utilizável.

O objetivo do app Embaralhar Baralho de Cartas é encontrar a técnica mais rápida para embaralhar um baralho de cartas que você pode usar em apps de jogos que criar. Mas, mais importante, ele fornecerá a você experiência em medir e avaliar o desempenho do app.

Sua tarefa é implementar o algoritmo de avaliação de desempenho, o gerador de números pseudoaleatórios Xorshift, bem como o algoritmo WELL512a.c se você escolher tentar a funcionalidade bônus.

## Histórias de Usuário

-   [ ] O usuário pode ver um painel contendo uma caixa de texto onde o usuário pode inserir o número de rodadas, três caixas de texto de saída para conter o tempo de início, tempo de fim, e tempo total do teste, e dois botões - 'JS Random', 'Xorshift'.
-   [ ] O usuário pode inserir um número de 1 a 10.000 para especificar o número de vezes (ou rodadas) que o número aleatório selecionado deve ser executado.
-   [ ] O usuário pode clicar em um dos três botões para iniciar a avaliação do algoritmo de número aleatório selecionado. O algoritmo de número aleatório será executado pelo número de rodadas inserido pelo usuário acima.
-   [ ] O usuário pode ver uma mensagem de aviso se o número de rodadas não foi inserido, se não está dentro do intervalo 1 a 10.000, ou se não é um inteiro válido.
-   [ ] O usuário pode ver uma área de saída tabular onde os resultados de cada algoritmo são exibidos - nome do algoritmo, tempo de início, tempo de fim, e tempo total.
-   [ ] O usuário pode ver uma caixa de diálogo de aviso com botões 'Cancelar' e 'OK' se o número de rodadas for alterado antes que todos os três testes tenham sido executados.
-   [ ] O usuário pode clicar no botão 'Cancelar' na caixa de diálogo de aviso para fechar a caixa de diálogo sem alterações.
-   [ ] O usuário pode clicar no botão 'OK' na caixa de diálogo de aviso para limpar a área de saída e fechar a caixa de diálogo de aviso.

## Funcionalidades Bônus

-   [ ] O usuário pode ver um terceiro botão de algoritmo - 'WELL512a.c'.
-   [ ] O desenvolvedor deve revisar a saída e determinar por que o algoritmo mais rápido é mais rápido que o mais lento.

## Links e Recursos Úteis

- [Geração de Números Aleatórios (Wikipedia)](https://en.wikipedia.org/wiki/Random_number_generation)
- [Math.random (MDN)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random)
- [Xorshift (Wikipedia)](https://en.wikipedia.org/wiki/Xorshift)
- [WELL512a.c](http://www.iro.umontreal.ca/~panneton/well/WELL512a.c)
- [console.time (MDN)](https://developer.mozilla.org/en-US/docs/Web/API/Console/time)
- [Usando o Recurso de Auditoria do Chrome DevTools para Medir e Otimizar Desempenho (Parte 1)](https://medium.com/chingu/using-the-chrome-devtools-audit-feature-to-measure-and-optimize-performance-part-1-868a20bbfde8)
- [Usando o Recurso de Auditoria do Chrome DevTools para Medir e Otimizar Desempenho (Parte 2)](https://medium.com/chingu/using-the-chrome-devtools-audit-feature-to-measure-and-optimize-performance-part-2-af4a78bc6cf0)

## Projetos de Exemplo

Adicione um ou mais exemplos de projetos que tenham funcionalidades semelhantes a esta aplicação. Isso atuará como um guia para o desenvolvedor.