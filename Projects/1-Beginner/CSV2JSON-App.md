# CSV2JSON

**Nível:** 1-Iniciante

No aplicativo [JSON2CSV](./JSON2CSV-App.md) você traduziu JSON 
para um formato de valores separados por vírgula (CSV). O objetivo do CSV2JSON é 
inverter esse processo convertendo um bloco de texto CSV para JSON.

No CSV2JSON você começará copiando o app JSON2CSV que criou e então
modificá-lo para permitir conversão de CSV para JSON além da
conversão de JSON para CSV já existente. Além de fornecer uma
função útil, este desafio também dará prática na modificação de
aplicações existentes para adicionar nova funcionalidade.

### Restrições ###

- Leia atentamente as histórias de usuário abaixo. Algumas das funcionalidades criadas
para JSON2CSV precisarão ser modificadas.
- Você não pode usar nenhuma biblioteca ou pacote projetado para realizar este
tipo de conversão.
- Estruturas JSON aninhadas não são suportadas.

## Histórias de Usuário

-   [ ] O usuário pode colar sintaxe CSV em uma caixa de texto
-   [ ] O usuário pode clicar em um botão 'Converter para JSON' para validar a caixa de texto CSV e convertê-la para JSON
-   [ ] O usuário pode ver uma mensagem de aviso se a caixa de texto CSV estiver vazia ou se não contiver CSV válido
-   [ ] O usuário pode ver o CSV convertido na caixa de texto JSON

### Histórias já implementadas no JSON2CSV 
-   [ ] O usuário pode colar sintaxe JSON em uma caixa de texto
-   [ ] O usuário pode clicar em um botão 'Converter para CSV' para validar a caixa de texto JSON e convertê-la para CSV
-   [ ] O usuário pode ver uma mensagem de aviso se a caixa de texto JSON estiver vazia ou se não contiver JSON válido
-   [ ] O usuário pode clicar em um botão 'Limpar' para limpar o conteúdo das caixas de texto JSON e CSV.

## Funcionalidades Bônus

-   [ ] O usuário pode inserir o caminho para o arquivo CSV no sistema de arquivos local em uma caixa de texto
-   [ ] O usuário pode clicar em um botão 'Abrir CSV' para carregar arquivo contendo o CSV na caixa de texto
-   [ ] O usuário pode ver uma mensagem de aviso se o arquivo CSV não for encontrado
-   [ ] O usuário pode clicar em um botão 'Salvar CSV' para salvar o arquivo CSV no caminho inserido na mesma caixa de texto usada para abrir o arquivo CSV
-   [ ] O usuário pode ver uma mensagem de aviso se a caixa de texto CSV estiver vazia ou se a operação de salvamento falhar.
-   [ ] O usuário pode inserir o caminho para o arquivo JSON no sistema de arquivos local em uma caixa de texto
-   [ ] O usuário pode clicar em um botão 'Abrir JSON' para carregar arquivo contendo o JSON na caixa de texto
-   [ ] O usuário pode ver uma mensagem de aviso se o arquivo JSON não for encontrado
-   [ ] O usuário pode clicar em um botão 'Salvar JSON' para salvar o arquivo JSON no  arquivo inserido na mesma caixa de texto usada para abrir o arquivo JSON
-   [ ] O usuário pode ver uma mensagem de aviso se a caixa de texto JSON estiver vazia ou se a operação de salvamento falhar.

## Links e Recursos Úteis

- [Valores Separados por Vírgula (CSV)](https://en.wikipedia.org/wiki/Comma-separated_values)
- [JavaScript Object Notation (JSON)](https://www.json.org/)
- [Salvando arquivo com JS puro](https://codepen.io/davidelrizzo/pen/cxsGb)
- [Lendo arquivos em Javascript](https://codepen.io/jduprey/details/xbale)

## Projetos de Exemplo

- [Conversor CSV para JSON](https://codepen.io/JFarrow/pen/CAwyo)
- [JSV Converter](https://gpaiva00.github.io/json-csv)