# Rastreador de Contribuições

**Nível:** 3-Avançado

No projeto [Charity Finder](../2-Intermediate/Charity-Finder-App.md) você criou um app para ajudar a localizar uma instituição de caridade digna de suas contribuições. Uma vez que uma contribuição foi feita, o objetivo do app Rastreador de Contribuições é rastreá-la para fornecer aos usuários um registro de todas as contribuições para uso no monitoramento de como os fundos estão sendo direcionados e para fornecer registros para fins de relatórios financeiros. Por exemplo, para relatórios fiscais.

### Restrições

- Desenvolvedores podem usar Vanilla JS, ou um framework de sua escolha (como React, VueJS, etc.).

- Desenvolvedores não devem usar bibliotecas para calcular e manipular valores monetários. Todos os cálculos e formatação devem ser feitos na linguagem escolhida para desenvolver a aplicação.

- Desenvolvedores podem usar uma biblioteca ou serviço de apresentação gráfica de sua escolha, como [AMCharts](https://www.amcharts.com/).

- Desenvolvedores podem optar por fazer transações persistirem entre sessões usando arquivos ou bancos de dados. Dados sensíveis, como transações, não devem ser mantidos no armazenamento local. Lembre-se que, embora você possa implementar proteções, é impossível proteger totalmente aplicações de navegador.

## Histórias de Usuário

-   [ ] O usuário pode ver uma Barra de Navegação no topo de cada página contendo o nome da aplicação e um menu "hambúrguer" com estas opções:
    - Dashboard
    - Transações
-   [ ] O usuário pode ver uma Barra de Rodapé na parte inferior de cada página contendo um link Sobre

### Página Dashboard
-   [ ] O usuário pode ver a página Dashboard quando o app é iniciado contendo resumos gráficos das seguintes métricas chave. A representação gráfica para cada uma é deixada a cargo do Desenvolvedor.
    - Contribuições por mês para o ano atual
    - Total de contribuições por ano
    - Aumento/diminuição de contribuições por ano
    - Valor médio de contribuição por mês e ano
-   [ ] O usuário pode retornar à página Dashboard, se estiver atualmente em outra página, clicando na opção 'Dashboard' no menu hambúrguer na Barra de Navegação.

### Página Transações
-   [ ] O usuário pode ver um painel de entrada de transação contendo o seguinte:
    - Data da transação
    - Nome do beneficiário
    - Valor
    - Memo
    - Botões de ação - 'Limpar', 'Adicionar'
-   [ ] O usuário pode ver um livro-razão de transação tabular contendo transações inseridas anteriormente. Cada linha também conterá um botão 'Modificar' e um 'Excluir'.
-   [ ] O usuário pode inserir valores descrevendo a transação nos campos de entrada
-   [ ] O usuário pode clicar no botão 'Limpar' para resetar todos os campos de entrada para um estado vazio.
-   [ ] O usuário pode clicar no botão 'Adicionar' para validar a entrada que foi inserida, adicionar a entrada validada ao livro-razão de transação, e limpar os campos de entrada.
-   [ ] O usuário pode ver uma mensagem de erro consolidada detalhando quaisquer erros detectados nos campos de entrada, incluindo:
    - Data inválida
    - Nome do beneficiário em branco
    - Campo de valor não numérico
-   [ ] O usuário pode clicar no botão 'Atualizar' para modificar uma transação inserida anteriormente. Os detalhes da transação serão copiados para o painel de entrada de transação e o botão 'Adicionar' mudará para 'Modificar'.
-   [ ] O usuário pode alterar valores nos campos de entrada e clicar no 'Modificar' para validar a entrada e atualizar a entrada daquela transação no livro-razão. Se bem-sucedido, o botão 'Modificar' voltará a 'Adicionar' e os campos de entrada serão limpos.
-   [ ] O usuário pode clicar no botão 'Excluir' para remover uma transação inserida anteriormente. Uma caixa de diálogo popup será exibida contendo botões 'Cancelar' e 'Ok' para cancelar ou confirmar a exclusão. Se a exclusão for confirmada, a transação será removida do livro-razão.
-   [ ] O usuário pode retornar à página Transações, se estiver atualmente em outra página, clicando na opção 'Transações' no menu hambúrguer na Barra de Navegação.

### Página Sobre
-   [ ] O usuário pode clicar no link Sobre na Barra de Rodapé para exibir informações sobre o Desenvolvedor.
-   [ ] O usuário pode ver links para o GitHub e contas de mídia social do Desenvolvedor incluindo ícones de mídia social (como o ícone do Twitter).

## Funcionalidades Bônus

-   [ ] O usuário pode clicar no campo de data da transação para exibir um calendário do qual a data pode ser selecionada em vez de digitá-la manualmente.
-   [ ] O usuário pode ver cores de fundo alternadas nas linhas do livro-razão de transação.
-   [ ] O usuário pode clicar em um cabeçalho de coluna no livro-razão de transação para alternar a sequência de ordenação nos valores daquela coluna.
-   [ ] O usuário pode ver uma opção PDF próximo ao Livro-Razão de Transação para criar um PDF de todas as transações (Dica: veja como essa capacidade pode ser implementada via [Puppeteer](https://github.com/GoogleChrome/puppeteer)).

## Links e Recursos Úteis

- [Como Lidar com Valores Monetários em JavaScript](https://frontstuff.io/how-to-handle-monetary-values-in-javascript)
- [Como Formatar Número como Moeda](https://flaviocopes.com/how-to-format-number-as-currency-javascript/)
- [Mintable (GitHub)](https://github.com/kevinschaich/mintable)

## Projetos de Exemplo

N/a