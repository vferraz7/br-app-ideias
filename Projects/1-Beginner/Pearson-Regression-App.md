# Pearson Regression

**Nível:** 1-Iniciante

Existem poucas, se alguma, aplicações que não requerem alguma forma de
conhecimento transdisciplinar para implementar funcionalidade útil para
um usuário. No caso de um app para a profissão médica pode ser
conhecimento em biologia ou farmacologia. Um fabricante de tintas ou um
negócio de ciências agrícolas pode confiar em apps com conhecimento íntimo
de química. E um aplicativo de folha de pagamento certamente incorporará
conceitos de RH e contabilidade.

Não importa o segmento industrial para o qual um app é desenvolvido, uma
especialização transdominio comum a todos é a matemática. Como um
desenvolvedor de aplicações você não precisa ser um matemático, mas é útil
ter um entendimento de como aplicar conceitos matemáticos aos problemas
que você está tentando resolver.

O objetivo deste app é aplicar o Coeficiente de Correlação de Pearson
contra dois conjuntos de dados para fornecer ao usuário o grau com o
qual eles podem ou não ser relacionados. Por exemplo, dado um conjunto de
temperaturas e outro conjunto de preços de carros isso permitiria ao
usuário testar se eles são relacionados (alerta de spoiler: eles não
são relacionados!).

### Restrições

- O Desenvolvedor deve programar todos os cálculos sem confiar em um
  pacote.

## Histórias de Usuário

-   [ ] O usuário pode ver um painel de entrada com dois campos permitindo
    entrada de coordenadas `x` e `y`, e botões 'Adicionar' and 'Calcular'.
-   [ ] O usuário pode inserir números nestas caixas onde `x` and `y` são
    observações dos dois conjuntos de dados.
-   [ ] O usuário pode clicar no botão 'Adicionar' para adicionar `x` and `y`
    a uma área de saída tabular listando os pares de observações.
-   [ ] O usuário pode ver uma mensagem de erro se algum dos dois campos de
    entrada estiver vazio ou não contiver números reais válidos.
-   [ ] O usuário pode ver o botão 'Calcular' desabilitado até que os erros
    sejam corrigidos.
-   [ ] O usuário pode clicar no botão 'Calcular' para realizar a análise de
    regressão e exibir seus resultados.
-   [ ] O usuário pode ver os resultados do cálculo que incluem:
    - Médias aritméticas para ambas as observações `x` and `y`
    - Desvios padrão para ambas as observações `x` and `y`
    - Coeficiente de correlação de Pearson com uma das seguintes
      interpretações:
      - Sem correlação
      - Neutro
      - Alguma correlação

## Funcionalidades Bônus

-   [ ] O usuário pode ver um gráfico de dispersão das observações
-   [ ] O usuário pode carregar observações de um arquivo da máquina local.
-   [ ] O usuário pode ver uma linha de regressão sobreposta ao gráfico
    de dispersão

## Links e Recursos Úteis

- [Pearson Correlation Coefficient (Wikipedia)](https://en.wikipedia.org/wiki/Pearson_correlation_coefficient)
- [Linear Regression](https://en.wikipedia.org/wiki/Linear_regression)
- [Pearson's Correlation Coefficient](http://www.code-in-javascript.com/pearsons-correlation-coefficient-in-javascript/)

## Projetos de Exemplo

[Correlation](https://memory.psych.mun.ca/tech/js/correlation.shtml)