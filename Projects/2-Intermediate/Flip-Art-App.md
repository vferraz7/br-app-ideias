# Arte de Virar

**Nível:** 2-Intermediário

Muitos desenvolvedores descobriram que adicionar animação a uma aplicação é uma técnica útil que adiciona impacto à UI, para torná-la mais atraente para seus usuários, e para explicar assuntos complexos. Mas, como desenvolvedor, como você cria essas animações e como sabe quais imagens fazem animações eficazes?

O objetivo do app Arte de Virar é atender a ambas as necessidades fornecendo uma maneira simples de coletar e organizar um conjunto de imagens em uma sequência animada que pode ser reproduzida e ajustada para alcançar o impacto e efeito desejados.

### Requisitos e Restrições

Os desenvolvedores não devem depender de bibliotecas de animação ou gráficos para implementar este app. Em vez disso, tente usar JavaScript, CSS e HTML puros.

## Histórias de Usuário

-   [ ] O usuário pode ver os seguintes componentes principais na janela do app:
    - Painel de configuração contendo elementos usados para personalizar o processo de animação.
    - Botões de operação
    - Painel de exibição de animação onde as animações serão apresentadas

### Painel de Configuração
-   [ ] O usuário pode ver oito miniaturas que conterão frames individuais de animação
-   [ ] O usuário pode ver um botão sob cada miniatura - '+'
-   [ ] O usuário pode clicar no botão '+' para adicionar uma nova imagem a uma miniatura vazia
-   [ ] O usuário pode ver uma caixa de diálogo de abertura de arquivo quando o botão '+' é clicado para permitir que uma imagem `.jpg` seja carregada na miniatura.
-   [ ] O usuário pode ver o rótulo do botão '+' mudar para '-' após uma miniatura ser carregada.
-   [ ] O usuário pode clicar no botão '-' para remover ou substituir uma miniatura.
-   [ ] O usuário pode ver um controle deslizante 'Velocidade de Transição'.
-   [ ] O usuário pode ajustar o controle deslizante 'Velocidade de Transição' de lento para rápido para ajustar o tempo de transição entre miniaturas na Exibição de Animação.

### Botões de Operação
-   [ ] O usuário pode ver dois botões - 'Limpar Configuração' e 'Iniciar Animação'
-   [ ] O usuário pode ver o botão 'Iniciar Animação' desabilitado até que pelo menos uma miniatura tenha sido adicionada via Painel de Configuração.
-   [ ] O usuário pode clicar no botão 'Limpar Configuração' para limpar todas as miniaturas do painel de configuração.
-   [ ] O usuário pode clicar no botão 'Iniciar Animação' para começar o painel de Exibição de Animação
-   [ ] O usuário pode ver o rótulo do botão 'Iniciar Animação' mudar para 'Parar Animação' uma vez que uma animação tenha sido iniciada.
-   [ ] O usuário pode clicar no botão 'Parar Animação' para interromper a animação na exibição de animação
-   [ ] O usuário pode ver o rótulo do botão 'Parar Animação' mudar para 'Iniciar Animação' quando uma animação foi parada.

### Painel de Exibição de Animação
-   [ ] O usuário pode ver miniaturas adicionadas no painel de Configuração exibidas quando o botão 'Iniciar Animação' é clicado.
-   [ ] O usuário pode ver miniaturas fazerem transição de uma para a próxima na taxa definida pelo controle deslizante 'Velocidade de Transição'.

## Funcionalidades Bônus

-   [ ] O usuário pode ver a borda ao redor da miniatura no Painel de Configuração destacada quando essa miniatura é exibida no painel de Exibição de Animação.
-   [ ] O usuário pode adicionar dinamicamente qualquer número de miniaturas em vez de ser restrito a apenas oito.
-   [ ] O usuário pode ouvir sons únicos associados à modificação de miniaturas no Painel de Configuração.
-   [ ] O usuário pode ver uma lista suspensa de tipo de transição no Painel de Configuração para definir o efeito de transição entre miniaturas na Exibição de Animação - ease, ease-in, ease-out, ease-in-out
-   [ ] O usuário pode arrastar e soltar miniaturas para reordená-las
-   [ ] O usuário pode salvar a animação como um arquivo `.gif`.

## Links e Recursos Úteis

- [Como Fazer Animação de Flip Book](https://www.youtube.com/watch?v=Njl-uqnmBGA)
- [Animação CSS (MDN)](https://developer.mozilla.org/en-US/docs/Web/CSS/animation)
- [Usando Transições CSS (MDN)](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Transitions/Using_CSS_transitions)
- [Transição CSS (MDN)](https://developer.mozilla.org/en-US/docs/Web/CSS/transition)

## Projetos de Exemplo

[FlipAnim](http://flipanim.com/)