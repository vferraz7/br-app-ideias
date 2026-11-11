# Diretório de Podcasts

**Nível:** 2-Intermediário

No app [GitHub Status](../1-Beginner/GitHub-Status-App.md) você aprendeu como usar o pacote Request para extrair informações de uma página web. O Diretório de Podcasts continua este processo e apresenta a você outro pacote de web scraping - [Puppeteer](https://github.com/GoogleChrome/puppeteer).

Embora o Request seja um pacote útil, ele não foi construído especificamente para web scraping como o Puppeteer. À medida que você ganha experiência com web scraping, você descobrirá que existem sites e aplicações onde o web scraping é facilitado pelo uso de uma ferramenta como o Puppeteer, especificamente construída para scraping.

É importante notar que, embora o web scraping tenha seu lugar, o uso de uma API ou uma fonte de dados como um arquivo ou banco de dados é sempre preferível a raspar informações de uma página. A razão é que até mesmo pequenas mudanças no estilo da página podem tornar seu web scraper inoperante. Por exemplo, a mudança de um nome de classe CSS no qual sua lógica de scraping depende.

O objetivo do app Diretório de Podcasts é obter os episódios mais recentes dos podcasts [Javascript Jabber](https://www.podbean.com/podcast-detail/d4un8-57595/JavaScript-Jabber-Podcast) e [Techpoint Charlie](https://www.podbean.com/podcast-detail/k76vd-8adc7/Techpoint-Charlie-Podcast) do [Podbean](https://www.podbean.com) e criar uma nova página que cria uma lista combinada de episódios, ordenados por data de transmissão.

## Histórias de Usuário

-   [ ] O usuário pode ver uma tabela de episódios de podcasts
-   [ ] O usuário pode ver linhas nesta tabela mostrando um ícone de episódio clicável, o título do episódio e a data em que foi transmitido originalmente.
-   [ ] O usuário pode rolar pela lista
-   [ ] O usuário pode clicar no ícone do episódio para exibir a página desse episódio no site do Podbean.

## Funcionalidades Bônus

-   [ ] O usuário pode ver linhas na tabela de episódios com cores de fundo alternadas.
-   [ ] O usuário pode ver um resumo acima da tabela de episódios mostrando o número de episódios para cada podcast.
-   [ ] O usuário pode ver uma caixa de seleção clicável ao lado de cada nome de podcast no resumo acima da tabela de episódios.
-   [ ] O usuário pode clicar no botão de rádio ao lado do nome do podcast para incluir episódios desse podcast na tabela de episódios.

## Links e Recursos Úteis

- [Puppeteer](https://github.com/GoogleChrome/puppeteer)
- [Web Scraping com um Navegador Headless: Um Tutorial Puppeteer](https://www.toptal.com/puppeteer/headless-browser-puppeteer-tutorial)
- [querySelectorAll](https://developer.mozilla.org/en-US/docs/Web/API/ParentNode/querySelectorAll)
- Dica! Você pode usar o seguinte código para ajudá-lo a começar com este projeto. Você pode executar isso usando o comando de linha de comando `node puptest`.
```
puptest.js
const puppeteer = require('puppeteer');

const run = async () => {
  return new Promise(async (resolve, reject) => {
    try {
      const browser = await puppeteer.launch();
      const page = await browser.newPage();
      await page.goto("https://www.podbean.com/podcast-detail/d4un8-57595/JavaScript-Jabber-Podcast");
      let episodeLinks = await page.evaluate(() => {
        return Array.from(document.querySelectorAll('a.title')).map((item) => ({
            url:  item.getAttribute('href'),
            text: item.innerText
          })
        );
      });
      browser.close();
      return resolve(episodeLinks);
    } catch (e) {
      return reject(e);
    }
  })
}

run()
.then(console.log)
.catch(console.error);
```
- Quando você completar este projeto, confira o projeto avançado [MyPodcast Library](../3-Advanced/MyPodcast-Library-app.md)

## Projetos de Exemplo

N/a