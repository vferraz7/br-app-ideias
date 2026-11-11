# Kudo's Slackbot

**Nível:** 3-Avançado

Você já reconheceu a contribuição ou assistência de um colega em um canal do Slack apenas para descobrir que se perdeu após alguns dias? Deixe o _*Kudo's*_ vir ao resgate.

Kudo's é um Slackbot que permite que você crie um reconhecimento pelos esforços de outra pessoa e o torne disponível através de um simples comando do Slack.

## Histórias de Usuário

-   [ ] O usuário pode criar um kudo usando o comando do Slack: `/kudo add <slack-id> <texto>` onde:

    -   `<slack-id>` define o indivíduo que receberá o reconhecimento
    -   `<texto>` é seu kudo para essa pessoa

-   [ ] O usuário pode modificar um kudo usando o comando do Slack: `/kudo replace <kudo-id> <texto>` onde:

    -   `<ação>` é 'replace' ou 'delete'
    -   `<kudo-id>` é o identificador do kudo
    -   `<texto>` é seu kudo para essa pessoa

-   [ ] O usuário pode excluir um kudo usando o comando do Slack: `/kudo delete <kudo-id>`

-   [ ] O usuário pode exibir os _n_ kudos mais recentes usando o comando do Slack: `/kudo list <n>` onde `n` é um inteiro ou `*` para todos os kudos

-   [ ] O usuário pode exibir todos os kudos de um indivíduo com o comando do Slack: `/kudo user <slack-id>`

## Funcionalidades Bônus

-   [ ] O usuário pode listar o indivíduo com mais kudos, em ordem decrescente, usando o comando do Slack: `/kudo top <n>` onde `n` é um inteiro ou `*` para todos os indivíduos que receberam um kudo

## Links e Recursos Úteis

-   [API do Slack](https://api.slack.com/)

## Projeto de Exemplo

-   [Exemplo Kudos Slackbot](https://cubic-quince.glitch.me/)