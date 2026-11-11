# CauseEffect

**Nível:** 1-Iniciante

Padrões são fundamentais na engenharia de software e representam componentes potencialmente
reutilizáveis na lógica do programa. No entanto, padrões não são usados apenas
para lógica de programa, eles existem em outros domínios como DevOps, suporte ao usuário,
e interface do usuário.

Um padrão comum de interface do usuário é resumir dados em uma seção de uma página
que consiste em algum tipo de lista (como texto, imagens, ou ícones) que descreve
ou categoriza um conjunto de dados. Quando um item da lista é clicado, os dados
detalhados por trás dele são exibidos em um painel adjacente na página.

Por exemplo, em um site imobiliário clicar em um endereço em uma lista de
imóveis à venda exibe detalhes sobre o imóvel em outra parte da
página.

Este desafio requer que o desenvolvedor siga estas restrições:

-   Você é responsável por criar seus próprios dados de teste. Use um objeto
    JavaScript com valores fixos para definir seus dados de teste (veja abaixo).
-   Use apenas HTML/CSS/Javascript nativos na primeira versão deste app
-   Você pode usar outros pacotes ou bibliotecas ao implementar versões
    posteriores.

## Histórias de Usuário

-   [ ] O usuário pode ver uma lista de nomes de pessoas dispostos verticalmente em um
        painel de resumo na página.
-   [ ] O usuário pode clicar em um nome da lista para atualizar um painel adjacente na
        página com o nome completo, endereço, número de telefone e
        data de aniversário daquela pessoa.
-   [ ] O usuário pode clicar em outro nome da lista para atualizar o painel
        de detalhes com as informações daquela pessoa.

## Funcionalidades Bônus

-   [ ] O usuário pode ver o nome da pessoa no painel de resumo destacado quando o
        cursor passa sobre ele.
-   [ ] O usuário pode ver o nome da pessoa no painel de resumo destacado
        usando um efeito de seleção (cor, tamanho, etc.) quando clicado. Este é um
        efeito diferente do efeito de hover
-   [ ] O usuário pode ver o efeito de seleção removido de um nome no painel
        de resumo quando um novo nome é clicado.

## Links e Recursos Úteis

-   [Eventos DOM](https://developer.mozilla.org/en-US/docs/Web/API/Event)
-   Considere definir seus dados de teste em um objeto JavaScript com
    formato como este:

```
const people = [
  {name: "...", street: "...", city: "...", state: "...", country: "...", telephone: "...", birthday: "..."},
  .
  .
  .
  {name: "...", street: "...", city: "...", state: "...", country: "...", telephone: "...", birthday: "..."}
];
```

## Projetos de Exemplo

Confira a interação entre os itens de navegação no lado esquerdo
da página e o corpo principal da página no [site MDN de JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)