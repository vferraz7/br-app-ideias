# Loja Online Simples

**Nível:** 2-Intermediário

No projeto [Página de Destino do Produto](../1-Beginner/Product-Landing-Page.md) você implementou uma página de destino para fornecer aos seus usuários informações sobre um produto e, esperançosamente, aumentar a taxa de conversão do seu site.

O objetivo da Loja Online Simples é dar aos seus usuários a capacidade de selecionar um produto para comprar, visualizar informações de compra, adicioná-lo a um carrinho de compras online e, finalmente, efetivamente comprar os produtos no carrinho de compras.

### Restrições

- Inicialmente, você pode implementar seu inventário de produtos como um array de objetos JavaScript se estiver desenvolvendo em JavaScript. Para outras linguagens, sinta-se à vontade para escolher a solução em memória de sua escolha.

## Histórias de Usuário

-   [ ] O usuário pode clicar no botão `Ver Produtos` na Página de Destino para exibir a Página de Produtos.
-   [ ] O usuário pode ver um card na Página de Produtos para cada Produto mostrando a miniatura do produto, nome, preço, uma descrição curta, e um botão `Selecionar`.
-   [ ] O usuário pode ver uma Página de Detalhes do Produto exibida quando o botão `Selecionar` é clicado mostrando as mesmas informações do card do produto, mas também um ID único do produto, uma descrição longa, botão `Adicionar ao Carrinho`, e um botão `Ver Mais Produtos`.
-   [ ] O usuário pode ver uma mensagem de confirmação quando o produto é adicionado ao carrinho de compras.
-   [ ] O usuário pode clicar na página `Ver Mais Produtos` para retornar à Página de Produtos.
-   [ ] O usuário pode ver um botão `Carrinho de Compras` tanto na Página de Destino quanto na Página de Produtos. Dica: uma barra superior pode ser um bom local comum para este botão.
-   [ ] O usuário pode clicar no botão `Carrinho de Compras` para exibir a página do Carrinho de Compras contendo o ID do produto, nome, preço, e caixa de entrada de quantidade ordenada para cada produto adicionado anteriormente ao Carrinho de Compras.
-   [ ] O usuário pode ver um valor total de compra no Carrinho que é calculado como a soma das quantidades multiplicadas pelo preço unitário para cada produto ordenado.
-   [ ] O usuário pode ajustar a quantidade ordenada para qualquer produto para ajustar o valor total da compra.
-   [ ] O usuário pode clicar no botão `Fazer Pedido` na Página do Carrinho de Compras para completar o pedido. O usuário verá um número de confirmação quando o pedido tiver sido feito.
-   [ ] O usuário pode clicar no botão `Cancelar Pedido` na Página do Carrinho de Compras para cancelar o pedido. O usuário verá as quantidades dos produtos e o valor total da compra resetados para zero.
-   [ ] O usuário pode clicar no botão `Ver Mais Produtos` na Página do Carrinho de Compras para retornar à Página de Produtos. Se o pedido não tiver sido feito ainda, isso não limpará os produtos que já foram adicionados à Página de Produtos.

## Funcionalidades Bônus

-   [ ] O usuário pode ver uma mensagem de erro se a quantidade ordenada exceder a quantidade "em estoque" do produto.
-   [ ] O usuário pode especificar endereços de cobrança e entrega quando o pedido é feito na Página do Carrinho de Compras
-   [ ] O usuário pode ver taxas de envio adicionadas ao valor total da compra
-   [ ] O usuário pode ver impostos de venda adicionados ao valor total da compra
-   [ ] O desenvolvedor implementará o inventário de produtos em um arquivo externo ou banco de dados.

## Links e Recursos Úteis

Existem muitas Páginas de Sites de eCommerce por aí. Você pode usar o [Dribbble](https://www.dribbble.com) e [Behance](https://www.behance.net) para inspiração.

## Projetos de Exemplo

-   [Animações de eCommerce](https://codepen.io/RSH87/pen/RagqEv)