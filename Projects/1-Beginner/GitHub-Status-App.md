# GitHub Status

**Nível:** 1-Iniciante

Apps Web adquirem dados de muitas formas. Através de entrada do usuário em páginas
web, através de APIs para sistemas de backend, de arquivos e bancos de dados, e
às vezes através de "scraping" de websites. O objetivo do app GitHub Status
é introduzi-lo a uma forma de obter informações de outro website.

O GitHub Status usa o pacote NPM Request para recuperar o status atual do
site GitHub do website [GitHub Status](https://www.githubstatus.com/). O
pacote Request permite que websites sejam recuperados não para uma janela de
navegador, mas como um documento JSON que pode ser prontamente acessado pelo
seu código.

Embora esta especificação de aplicação dependa fortemente de Javascript, sinta-se
à vontade para desenvolvê-la usando sua linguagem de preferência!

## Histórias de Usuário

-   [ ] O usuário pode ver o status atual para Git Operations do GitHub, API Requests,
Problemas Operacionais, PRs, Dashboard & Projects, Notificações Operacionais,
Operational Gists, and Operational GitHub Pages como uma lista na
janela principal do app.
-   [ ] O usuário pode recuperar o status mais recente do website GitHub Status
clicando no botão 'Obter Status'.

## Funcionalidades Bônus

-   [ ] O usuário pode ver quaisquer componentes do GitHub que não estejam com status
'Operacional' destacados com uma cor diferente, animação de fundo, ou
qualquer outra técnica para torná-lo evidente. Use sua imaginação!

## Links e Recursos Úteis

- [Web Scraping (Wikipedia)](https://en.wikipedia.org/wiki/Web_scraping)
- [NPM Request](https://www.npmjs.com/package/request)
- [Javascript JSON (MDN)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/JSON)
- [Javascript Object Notation](https://json.org/)
- Dica! Você pode usar o seguinte código para exibir o JSON do website
GitHub Status a partir da linha de comando `node ghstatus`. Você pode usar essa
saída para determinar quais elementos JSON contêm as informações de status
que você precisará para desenvolver este app.
```
ghstatus.js

const request = require('request');
request('https://www.githubstatus.com/',  { json: true }, (err, res, body) => {  
    console.log(body);
});
```

## Projetos de Exemplo

- [Exemplo de Peter Luczynski](https://peterluczynski.github.io/github-status/)
- [Exemplo de Diogo Moreira](https://diogomoreira.github.io/github-status/)