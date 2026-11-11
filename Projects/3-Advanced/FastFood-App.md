# App Simulador de Fast Food

**Nível:** 3-Avançado

Fast Food simula a operação de um simples restaurante de take-away e é projetado para ajudar o desenvolvedor a colocar seu conhecimento de Promises e princípios de design SOLID em prática.

Este app simula clientes de um restaurante de take-away fazendo pedidos e esperando que eles sejam preparados e entregues a um balcão de retirada. Após fazer o pedido, o cliente espera o pedido ser anunciado antes de pegá-lo e ir para a área de refeições.

As histórias de usuário que compõem este app giram em torno de quatro papéis distintos:

- Usuário - o usuário final usando a aplicação
- Cliente - o Cliente simulado
- Atendente de Pedidos - o Atendente de Pedidos simulado
- Cozinheiro - o Cozinheiro simulado
- Atendente - o Atendente simulado

Este app tem várias Histórias de Usuário. Não se assuste. Reserve tempo para esboçar não apenas a UI, mas como os diferentes atores (papéis) interagem e construa o app incrementalmente seguindo princípios Ágeis.

### Restrições

- Tíquetes de pedido podem ser representados como dois tipos diferentes de Promises - um que o Atendente espera enquanto o Cozinheiro prepara o pedido e outro que o Cliente espera enquanto na fila de atendimento.
- Use o equivalente nativo de JS Promises na linguagem que você escolher para desenvolver. Desenvolvedores JS devem usar Promises nativas e não `async/await`.
- Crie este app usando recursos nativos da linguagem. Você NÃO pode usar um pacote ou biblioteca de simulação.
- Novos clientes chegam na fila de pedidos em um intervalo de tempo fixo. Em outras palavras, novos clientes chegam a uma taxa constante.
- Tíquetes de pedido são atendidos em um intervalo de tempo fixo também. Eles são completados a uma taxa constante.

## Histórias de Usuário

### Operação da Aplicação
-   [ ] O usuário pode ver uma área de entrada que permite a inserção do intervalo de tempo para chegada de clientes e um intervalo de tempo para o atendimento de um _tíquete de pedido_ pelo cozinheiro.
-   [ ] O usuário pode ver uma mensagem de aviso personalizada se o intervalo de chegada do cliente ou o intervalo de atendimento do pedido for inserido incorretamente.
-   [ ] O usuário pode iniciar a simulação clicando em um botão Iniciar.
-   [ ] O usuário pode ver uma área de fila de pedidos contendo uma caixa de texto mostrando o número de clientes esperando para fazer pedidos.
-   [ ] O usuário pode ver uma área de pedidos contendo caixas de texto mostrando o _número do pedido_ sendo atendido no momento.
-   [ ] O usuário pode ver uma área de cozinha contendo uma caixa de texto mostrando o _número do pedido_ sendo preparado e uma caixa de texto listando os pedidos em espera em sequência, junto com uma contagem do número de pedidos em espera.
-   [ ] O usuário pode ver uma área de Retirada contendo uma caixa de texto mostrando o _número do pedido_ atualmente disponível para retirada pelo Cliente e uma caixa de texto mostrando o número de Clientes esperando na fila de atendimento.
-   [ ] O usuário pode parar a simulação a qualquer momento clicando em um botão Parar.

## Funcionalidades Bônus

-   [ ] O usuário pode especificar quanto tempo leva para um Atendente de Pedidos criar um _tíquete de pedido_.
-   [ ] O usuário pode especificar quanto tempo leva para o Atendente entregar um pedido ao cliente.
-   [ ] O usuário pode especificar a quantidade total de tempo que a simulação deve rodar uma vez que o botão Iniciar foi clicado.
-   [ ] O usuário pode ver uma visualização animada de Clientes e pedidos enquanto eles se movem pelo fluxo de trabalho.

## Links e Recursos Úteis

- [Fast Food Simulator - Fluxo de Trabalho Lógico](https://drive.google.com/file/d/1Thfm5cFDm1OjTg_0LsIt2j1uPL5fv-Dh/view?usp=sharing)
- [Manifesto Ágil e 12 Princípios de Software Ágil](http://agilemanifesto.org/)
- [Princípios SOLID que Todo Desenvolvedor Deve Conhecer](https://blog.bitsrc.io/solid-principles-every-developer-should-know-b3bfa96bb688)
- [Usando Promises](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Using_promises)
- [Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)

## Projetos de Exemplo

- N/a