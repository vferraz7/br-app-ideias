# Windchill

**Nível:** 1-Iniciante

O Windchill combina a temperatura real com a velocidade do vento para
calcular o fator de sensação térmica, ou qual é a temperatura percebida
em comparação à temperatura real.

## Histórias de Usuário

-   [ ] O usuário pode selecionar o sistema de medida em que os cálculos
    serão realizados - Métrico or Inglês
-   [ ] O usuário pode inserir a temperatura real and a velocidade do
    vento
-   [ ] O usuário pode pressionar o botão `Calcular` para exibir o
    fator de sensação térmica
-   [ ] O usuário receberá uma mensagem de erro quando `Calcular` for
    clicado se os valores de dados não forem inseridos

## Funcionalidades Bônus

-   [ ] O usuário receberá uma mensagem de erro quando `Calcular` for
    clicado se o fator de sensação térmica resultante for maior ou igual
    à temperatura real. Como isso significa um erro interno no
    cálculo você também pode satisfazer este requisito usando uma
    asserção
-   [ ] O usuário será solicitado a inserir novos valores de dados se
    `Calcular` for pressionado sem antes alterar pelo menos um dos
    campos de entrada
-   [ ] O usuário verá um fator de sensação térmica atualizado sempre
    que novos valores de temperatura real or velocidade do vento forem
    inseridos, sem ser obrigado a clicar no botão `Calcular`

## Links e Recursos Úteis

-   [Wikipedia Wind Chill](https://en.wikipedia.org/wiki/Wind_chill)
-   [JavaScript Assert](https://developer.mozilla.org/en-US/docs/Web/API/console/assert)

## Projetos de Exemplo

[Wind Chill Calculator](http://www.jsmadeeasy.com/javascripts/Calculators/Wind%20Chill%20Calculator/index.htm)
[Svelte Wind Chill Index by Gabriele Corti](https://codepen.io/borntofrappe/pen/WNNrrJg)