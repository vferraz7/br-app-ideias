# Recipe

**Nível:** 1-Iniciante

Você pode não ter percebido isso, mas receitas nada mais são do que
algoritmos culinários. Como programas, receitas são uma série de passos
imperativos que, se seguidos corretamente, resultam em um prato saboroso.

O objetivo do app Recipe é ajudar o usuário a gerenciar receitas de uma
forma que as torne fáceis de seguir. 

### Restrições

- Para a versão inicial deste app os dados da receita podem ser codificados
  como um arquivo JSON. Após implementar a versão inicial deste app você
  pode expandi-lo para manter receitas em um arquivo ou banco de dados.

## Histórias de Usuário

-   [ ] O usuário pode ver uma lista de títulos de receitas
-   [ ] O usuário pode clicar em um título de receita para exibir um cartão
    de receita contendo o título da receita, tipo de refeição (café da manhã,
    almoço, jantar, or lanche), número de pessoas que serve, seu nível de
    dificuldade (iniciante, intermediário, avançado), a lista
    de ingredientes (incluindo suas quantidades), and os passos de
    preparação.
-   [ ] O usuário clica em um novo título de receita para substituir o cartão
    atual por uma nova receita.

## Funcionalidades Bônus

-   [ ] O usuário pode ver uma foto mostrando como o item fica após ser
    preparado.
-   [ ] O usuário pode buscar uma receita não presente na lista de títulos
    de receitas inserindo o nome da refeição em uma caixa de busca e clicando
    em um botão 'Buscar'. Qualquer API de receitas open source pode ser usada
    como fonte para receitas (veja The MealDB abaixo).
-   [ ] O usuário pode ver uma lista de receitas que correspondem aos termos
    de busca
-   [ ] O usuário pode clicar no nome da receita para exibir seu cartão de
    receita.
-   [ ] O usuário pode ver uma mensagem de aviso se nenhuma receita
    correspondente for encontrada.
-   [ ] O usuário pode clicar em um botão 'Salvar' nos cartões para receitas
    localizadas através da API para salvar uma cópia no arquivo de receitas
    ou banco de dados deste app.

## Links e Recursos Úteis

- [Using Fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch)
- [Axios](https://www.npmjs.com/package/axios)
- [The MealDB API](https://www.themealdb.com/api.php) 

## Projetos de Exemplo

- [Recipe Box - a Free Code Camp Project (FCC)](https://codepen.io/eddyerburgh/pen/xVeJvB)
- [React Recipe Box](https://codepen.io/inkblotty/pen/oxWRme)