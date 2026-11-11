# Minha Biblioteca de Podcasts

**Nível:** 3-Avançado

No [GitHub Status](../1-Beginner/GitHub-Status-App.md) e [Diretório de Podcasts](../2-Intermediate/Podcast-Directory-App.md) você aprendeu o que é web scraping e como você pode usá-lo como uma fonte de dados alternativa quando APIs e bancos de dados backend não estão disponíveis. O app _Minha Biblioteca de Podcasts_ combina seu novo conhecimento de web scraping com suas habilidades de frontend para estender o simples app Diretório de Podcasts em algo mais complexo e útil.

O objetivo do _Minha Biblioteca de Podcasts_ é construir uma biblioteca mais personalizada dos seus podcasts e episódios favoritos. Neste app você usará [Puppeteer](https://github.com/GoogleChrome/puppeteer) e [Podbean](https://www.podbean.com) para criar um app para manter sua biblioteca pessoal de podcasts.

Este projeto é descrito em detalhes pelas seguintes histórias de usuário, mas sinta-se à vontade para usar sua imaginação.

## Histórias de Usuário

### Exibição de Podcasts Favoritos

-   [ ] O usuário pode ver seus podcasts favoritos em uma área de exibição tabular
-   [ ] O usuário pode ver a mensagem 'Nenhum podcast adicionado ainda' em formato de marca d'água nesta área se nenhum podcast foi adicionado.
-   [ ] O usuário pode ver uma visão geral de cada podcast favorito que foi adicionado nesta área. Isso inclui o ícone do podcast, seu nome, e o número de episódios mais recentes.
-   [ ] O usuário pode clicar no ícone do podcast para exibir uma página contendo uma lista dos episódios mais recentes.

### Entrada de Podcast Favorito
-   [ ] O usuário pode ver um botão '+' no topo da área de podcasts favoritos com o texto de hover 'Adicionar um novo podcast'
-   [ ] O usuário pode clicar no botão '+' para exibir um painel popup para permitir adicionar um novo podcast favorito. Este painel contém uma área de entrada contendo uma caixa de texto para a página do podcast no Podbean (ex: [Techpoint Charlie](https://www.podbean.com/podcast-detail/k76vd-8adc7/Techpoint-Charlie-Podcast)), um botão 'Salvar', e um botão 'Cancelar'.
-   [ ] O usuário pode clicar no botão 'Salvar' para validar a URL e adicionar o podcast à área de podcasts favoritos.
-   [ ] O usuário pode ver uma mensagem de aviso se a URL não começar com ```https://www.podbean.com/podcast-detail/``` ou se navegar para a página resultar em erro 404.
-   [ ] O usuário pode ver URLs válidas para podcasts favoritos retidas entre sessões.
-   [ ] O usuário pode clicar no botão 'Cancelar' para descartar quaisquer dados e fechar o popup.

### Episódios Mais Recentes para uma Página de Podcast
-   [ ] O usuário pode ver uma tabela de episódios de podcast
-   [ ] O usuário pode ver linhas nesta tabela mostrando um ícone de episódio clicável, o título do episódio, a data em que foi transmitido originalmente, e um botão de ícone de coração para marcá-lo como favorito.
-   [ ] O usuário pode rolar pela lista
-   [ ] O usuário pode clicar no ícone do episódio para exibir a página desse episódio no site do Podbean.
-   [ ] O usuário pode clicar no ícone de coração de um episódio para marcá-lo como favorito.
-   [ ] O usuário pode clicar no ícone de coração de um episódio para removê-lo como favorito.
-   [ ] O usuário pode ver a tabela ordenada com os episódios mais recentes no topo, seguidos pelos marcados anteriormente como favoritos.
-   [ ] O usuário pode ver episódios favoritos persistirem entre sessões.

## Funcionalidades Bônus

### Avaliações de Episódios
-   [ ] O usuário pode ver 5 ícones de estrela com cada episódio que denota como o usuário o avalia.
-   [ ] O usuário pode clicar nas estrelas da esquerda para direita para avaliar um episódio. Estrelas são preenchidas ou mudam para uma nova cor quando clicadas.
-   [ ] O usuário pode alterar uma avaliação clicando nas estrelas da direita para esquerda para desmarcá-las.
-   [ ] O usuário pode ver a lista de episódios favoritos na página ordenada em sequência de avaliação decrescente.

### Busca e Hashtags
-   [ ] O usuário pode inserir uma hashtag livre com um episódio na página de episódios mais recentes. Esta hashtag não precisa ser predefinida.
-   [ ] O usuário pode ver uma caixa de busca na página principal e um botão 'Buscar'
-   [ ] O usuário pode inserir hashtags na caixa de busca para exibir uma página de episódios de qualquer podcast com o mesmo formato da página de episódios mais recentes.
-   [ ] O usuário pode clicar no botão cancelar na página de resultados da busca para retornar à página principal.

## Links e Recursos Úteis

- [Puppeteer](https://github.com/GoogleChrome/puppeteer)
- [Web Scraping com um Navegador Headless: Um Tutorial Puppeteer](https://www.toptal.com/puppeteer/headless-browser-puppeteer-tutorial)
- [querySelectorAll](https://developer.mozilla.org/en-US/docs/Web/API/ParentNode/querySelectorAll)

## Projetos de Exemplo

N/a