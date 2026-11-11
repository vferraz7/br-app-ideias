# Comprovantes de Vendas

**Nível:** 2-Intermediário

No app [First DB App](../1-Beginner/First-DB-App.md) você aprendeu o básico de como usar o banco de dados IndexedDB embutido no navegador. Em Comprovantes de Vendas você dará um passo adiante criando um app que registra comprovantes de ponto de venda, presumivelmente para posterior conciliação com o dinheiro no caixa da loja.

O objetivo dos Comprovantes de Vendas é implementar funcionalidade de ponto de venda para um comerciante e registrar todas as vendas em um banco de dados.

### Requisitos e Restrições

- O desenvolvedor deve implementar este app como uma aplicação frontend que usa o banco de dados IndexedDB no navegador para registrar todos os comprovantes de vendas.

- O desenvolvedor pode implementar o inventário de itens disponíveis para venda como um array de objetos no código-fonte da aplicação. Cada item deve ser definido com os seguintes atributos:
    - Número do item (único)
    - Descrição
    - Preço unitário

- O desenvolvedor deve usar suas habilidades de UI/UX para criar um layout de janela agradável e eficiente que torne fácil para o usuário comprar itens e exibir o histórico de compras.

- O caso de uso principal para um banco de dados baseado no navegador é manter informações de estado ou status que precisam persistir entre sessões, ou como uma área de trabalho para dados temporários. Por exemplo, dados recuperados de um servidor que devem ser reformatados ou limpos antes de serem apresentados ao usuário.

- É importante lembrar que, como o ambiente do navegador do lado do cliente não pode ser protegido, você não deve manter nenhuma informação confidencial ou de identificação pessoal (PII) em um banco de dados baseado no navegador.

## Histórias de Usuário

-   [ ] O usuário pode ver um painel de compra contendo botões para cada item contendo o número do item, descrição, e preço unitário, bem como botões 'Limpar' e 'Finalizar Compra'.
-   [ ] O usuário pode clicar no botão de um item para fazer uma compra.
-   [ ] O usuário pode ver um campo exibindo o valor total da venda incrementado à medida que itens são comprados.
-   [ ] O usuário pode ver um painel de comprovante exibindo a data e hora da venda, bem como todos os itens selecionados para compra. Isso inclui o número do item, descrição, e preço unitário.
-   [ ] O usuário pode clicar no botão 'Limpar' para limpar todas as compras a qualquer momento antes de finalizar.
-   [ ] O usuário pode clicar no botão 'Finalizar Compra' para completar a compra de todos os itens selecionados. O valor total final da compra será adicionado ao final do painel do comprovante e todos os itens selecionados serão adicionados ao banco de dados.
-   [ ] O usuário pode ver o painel do comprovante limpo após todos os itens terem sido adicionados ao banco de dados.
-   [ ] O usuário pode ver um botão 'Vendas Diárias' e um botão 'Limpar Tudo' na parte inferior da janela do app.
-   [ ] O usuário pode clicar no botão 'Vendas Diárias' para exibir todos os itens comprados por todos os clientes no painel do comprovante junto com o total de todos eles.
-   [ ] O usuário pode clicar no botão 'Limpar Tudo' para limpar o painel do comprovante e excluir o registro de todas as compras do banco de dados.

## Funcionalidades Bônus

-   [ ] O usuário pode ver uma imagem em miniatura dos itens nos botões dos itens.
-   [ ] O usuário pode ver o botão 'Limpar' substituído pelos botões 'Limpar Entrada' e 'Cancelar Tudo' sob o painel de compra
-   [ ] O usuário pode clicar no botão 'Limpar Entrada' para limpar o último item selecionado do painel do comprovante. Isso tem o efeito de desselecionar aquele item.
-   [ ] O usuário pode clicar no botão 'Cancelar Tudo' para limpar todas as compras feitas antes de finalizar.
-   [ ] O usuário pode ver um campo de entrada no painel de entrada onde o usuário pode inserir o nome do cliente quando uma compra é feita. O nome do cliente será adicionado a todos os itens comprados por aquele cliente no painel do comprovante e nas linhas adicionadas ao banco de dados.

## Links e Recursos Úteis

- [Conceitos do IndexedDB (MDN)](http://tinyw.in/7TIr)
- [Usando IndexedDB (MDN)](http://tinyw.in/w6k0)
- [API do IndexedDB (MDN)](http://tinyw.in/GqnF)
- [Suporte do Navegador ao IndexedDB](https://caniuse.com/#feat=indexeddb)

## Projetos de Exemplo

- N/a