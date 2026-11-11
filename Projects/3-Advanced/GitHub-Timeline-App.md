# Linha do Tempo do GitHub

**Nível:** 3-Avançado

APIs e representação gráfica de informações são marcas registradas de aplicações web modernas. Linha do Tempo do GitHub combina as duas para criar um histórico visual da atividade de um usuário no GitHub.

O objetivo da Linha do Tempo do GitHub é aceitar um nome de usuário do GitHub e produzir uma linha do tempo contendo cada repo e anotado com os nomes dos repos, a data em que foram criados, e suas descrições. A linha do tempo deve ser uma que pudesse ser compartilhada com um empregador em potencial. Deve ser fácil de ler e fazer uso eficaz de cor e tipografia.

Apenas repos públicos do GitHub devem ser exibidos.

## Histórias de Usuário

-   [ ] O usuário pode inserir um nome de usuário do GitHub
-   [ ] O usuário pode clicar no botão 'Gerar' para criar e exibir a linha do tempo dos repos do usuário nomeado
-   [ ] O usuário pode ver uma mensagem de aviso se o nome de usuário do GitHub não for um nome de usuário válido do GitHub.

## Funcionalidades Bônus

-   [ ] O usuário pode ver um resumo do número de repos contabilizados pelo ano em que foram criados

## Links e Recursos Úteis

O GitHub oferece duas APIs que você pode usar para acessar dados de repos. Você também pode optar por usar um pacote NPM para acessar a API do GitHub.

A documentação para a API do GitHub pode ser encontrada em:

-   [GitHub REST API V3](https://developer.github.com/v3/)
-   [GitHub GraphQL API V4](https://developer.github.com/v4/)

Exemplos de código mostrando como usar as APIs do GitHub:

-   [Cliente GitHub REST API para JavaScript ](https://github.com/octokit/rest.js/)
-   [Cliente GitHub GraphQL API para navegadores e Node](https://github.com/octokit/graphql.js)

Você pode usar este comando CURL para ver o JSON retornado pela V3 REST API para seus repos:

```
curl -u "user-id" https://api.github.com/users/user-id/repos
```

## Projetos de Exemplo

-   [Linha do Tempo CSS](https://codepen.io/NilsWe/pen/FemfK)
-   [Construindo uma Linha do Tempo Vertical com CSS e um Toque de JavaScript](https://codepen.io/tutsplus/pen/QNeJgR)