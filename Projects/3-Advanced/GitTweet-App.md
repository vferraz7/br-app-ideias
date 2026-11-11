# GitTweet

**Nível:** 3-Avançado

No app [Linha do Tempo do GitHub](./GitHub-Timeline-App.md) você usou a API do GitHub para criar uma linha do tempo dos seus repos. O que poderia ser mais poderoso do que usar uma API como esta? Usar duas APIs, é claro.

O objetivo do GitTweet é criar um app do GitHub para twittar quando um pull request é criado para um dos seus repos.

## Histórias de Usuário

-   [ ] O usuário pode ver uma área de entrada com exibição tabular preenchida com linhas para cada um dos repos do GitHub que ela possui e uma caixa de seleção ao lado de cada nome do repo, um único campo de data de entrada, e um botão 'Escanear'.
-   [ ] O usuário pode clicar nas caixas de seleção na lista de repos para selecionar ou deselecionar repos para processamento.
-   [ ] O usuário pode inserir uma data no campo de data. Isso define o ponto após o qual quaisquer novas solicitações de PR serão tuitadas.
-   [ ] O usuário pode clicar no botão 'Escanear' para identificar repos que tiveram um novo PR criado que não foi tuitado anteriormente. Em outras palavras. Inserir consecutivamente a mesma data para escanear deve gerar tuítes apenas para PRs que ainda não foram tuitados.
-   [ ] O usuário pode ver uma mensagem de erro se nenhuma data foi inserida, se não é uma data válida, ou se é uma data futura.
-   [ ] O usuário pode ver repos destacados se um tuíte será gerado para eles e o botão 'Escanear' mudará para 'Tuítar'.
-   [ ] O usuário pode deselecionar um repo clicando em sua caixa de seleção. Fazer isso mudará o botão de volta para 'Escanear' e clicá-lo repetirá a busca por repos que tiveram novos PRs (ainda não tuitados) criados desde a data de escaneamento inserida pelo usuário.
-   [ ] O usuário pode inserir uma nova data de escaneamento neste ponto, o que também muda o botão de volta para 'Escanear'.
-   [ ] O usuário pode clicar no botão 'Tuítar' para enviar um tuíte com a seguinte mensagem - `Pull Requst #<pr-number> created for repo <repo name> - <repo description>`.
-   [ ] O usuário pode ver este tuíte enviado de sua conta do Twitter.

## Funcionalidades Bônus

-   [ ] O usuário não precisa inserir manualmente uma data de escaneamento. Se omitida, o escaneamento será retomado a partir da última data de escaneamento que deve persistir entre sessões.
-   [ ] O usuário pode inserir uma mensagem de tuíte personalizada
-   [ ] As seleções de repos do usuário persistirão entre sessões para que não precisem ser reselecionadas cada vez.

## Links e Recursos Úteis

- [Documentação de Desenvolvedores do Twitter](https://developer.twitter.com/en.html)
- [Apps do GitHub](https://developer.github.com/apps//)
- O GitHub oferece duas APIs que você pode usar para acessar dados de repos. Você também pode optar por usar um pacote NPM para acessar a API do GitHub. A documentação para a API do GitHub pode ser encontrada em:

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

[Integração GitHub do Zapier](https://zapier.com/apps/github/integrations/twitter)