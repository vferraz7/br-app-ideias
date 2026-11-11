# JSON2CSV

**Nível:** 1-Iniciante

Desenvolvedores e usuários finais são especialistas em seus próprios domínios e, como
tais, cada um fala usando uma linguagem e terminologia específicas do domínio.
Isso também se estende às ferramentas usadas para manipular dados. Desenvolvedores
encontraram no JSON um método universalmente aceito para transferir dados entre
aplicações. Usuários finais, por outro lado, confiam em planilhas para
organizar e analisar dados.

O objetivo do JSON2CSV é ajudar a preencher a lacuna entre JSON e CSV
convertendo JSON para CSV para facilitar a revisão de dados em uma planilha.
Permite que o usuário cole JSON em uma caixa de texto para gerar seu
equivalente em CSV.

### Restrições ###

- Você não pode usar nenhuma biblioteca ou pacote projetado para realizar este
tipo de conversão.
- Se você optar por implementar isso em JavaScript não use loops complexos
em sua primeira implementação. Em vez disso, use `Object.keys()` e `Object.values`
para gerar CSV para o cabeçalho e linhas de dados.
- Estruturas JSON aninhadas não são suportadas.

## Histórias de Usuário

-   [ ] O usuário pode colar sintaxe JSON em uma caixa de texto
-   [ ] O usuário pode clicar em um botão 'Converter' para validar a caixa de
    texto JSON e convertê-la para CSV
-   [ ] O usuário pode ver o CSV convertido em outra caixa de texto
-   [ ] O usuário pode ver uma mensagem de aviso se a caixa de texto JSON estiver
    vazia ou se não contiver JSON válido
-   [ ] O usuário pode clicar em um botão 'Limpar' para limpar o conteúdo das
    caixas de texto JSON and CSV.

## Funcionalidades Bônus

-   [ ] O usuário pode inserir o caminho para o arquivo JSON no sistema de
    arquivos local em uma caixa de texto
-   [ ] O usuário pode clicar em um botão 'Abrir' para carregar arquivo contendo
    o JSON na caixa de texto
-   [ ] O usuário pode ver uma mensagem de aviso se o arquivo JSON não for
    encontrado
-   [ ] O usuário pode inserir o caminho para onde o arquivo CSV deve ser salvo
    em uma caixa de texto
-   [ ] O usuário pode clicar em um botão 'Salvar' para salvar o arquivo CSV no
    sistema de arquivos local
-   [ ] O usuário pode ver uma mensagem de aviso se a caixa de texto CSV estiver
    vazia ou se a operação de salvamento falhar.
-   [ ] O usuário pode converter dados CSV para JSON. Veja [CSV2JSON](./CSV2JSON-App.md)

## Links e Recursos Úteis

- [Comma Separated Values (CSV)](https://en.wikipedia.org/wiki/Comma-separated_values)
- [JavaScript Object Notation (JSON)](https://www.json.org/)
- [MDN Javascript Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)
- [Saving a file with pure JS](https://codepen.io/davidelrizzo/pen/cxsGb)
- [Reading files in Javascript](https://codepen.io/jduprey/details/xbale)

## Projetos de Exemplo

Tente completar sua implementação JSON2CSV antes de revisar o(s)
projeto(s) de exemplo.

- [JSON to CSV Converter](https://codepen.io/JFarrow/pen/umjGF)
- [JSV Converter](https://gpaiva00.github.io/json-csv)