# Timezone Slackbot - TZ

**Nível:** 2-Intermediário

Membros de equipe frequentemente precisam descobrir o fuso horário uns dos outros como primeiro passo para encontrar horários para reuniões e sessões de programação em par. Para ajudar com isso, o Timezone Slack bot aceita uma lista de nomes de usuários do Slack e exibe o fuso horário para cada usuário em formato empilhado da seguinte forma:

```
      -12 -11 -10 -9 -8 -7 -6 -5 -4 -3 -2 -1 0 +1 +2 +3 +4 +5 +6 +7 +8 +9 +10 +11 +12 +13 +14
Fred                           X
Nisha                                                       X
Ming                                                              X
  .
  .
  .
```

Note que este formato é fornecido apenas para fins descritivos. Quando implementado, um formato mais agradável e amigável ao usuário pode ser usado.

## Histórias de Usuário

-   [ ] O usuário pode digitar `/tz <nome-usuario> <nome-usuario>...<nome-usuario>` para exibir representação tabular mostrando o fuso horário de cada usuário
-   [ ] O usuário pode ver informações exibidas usando cores alternadas nas linhas para aumentar a clareza e legibilidade

## Funcionalidades Bônus

-   [ ] O usuário pode ver o fuso horário da pessoa exibido ao lado do nome. Por exemplo, 'IST' para Horário Padrão da Índia

## Links e Recursos Úteis

Mais informações sobre fusos horários podem ser encontradas [aqui](https://www.timeanddate.com/time/current-number-time-zones.html)

## Projetos de Exemplo

[Determine Rapidamente Em Que País e Fuso Horário Seus Colegas Estão Esta Semana Usando Esta Ferramenta](https://lifehacker.com/quickly-determine-what-country-and-time-zone-your-cowor-1833011887)