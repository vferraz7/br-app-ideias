# Countdown Timer

**Nível:** 1-Iniciante

Todos temos eventos importantes que esperamos na vida, aniversários,
aniversários de casamento, e feriados para citar alguns. Não seria ótimo ter um app
que faça contagem regressiva de meses, dias, horas, minutos, e segundos para um evento?
O Countdown Timer é exatamente esse app!

O objetivo do Countdown Timer é fornecer uma exibição continuamente decrescente
dos meses, dias, horas, minutos, e segundos para um evento inserido pelo
usuário.

### Restrições

- Use apenas funções nativas da linguagem para seus cálculos em vez de confiar
em uma biblioteca ou pacote como [MomentJS](https://momentjs.com/). Isso assume,
é claro, que a linguagem de sua escolha tenha funções adequadas de
manipulação de data e hora nativas.
- Você não pode usar geradores de código como o
[Counting Down To](https://countingdownto.com/). Você deve desenvolver sua
própria implementação original. 

## Histórias de Usuário

-   [ ] O usuário pode ver uma caixa de entrada de evento contendo um campo para nome do evento,
campo de data, hora opcional, e um botão 'Iniciar'.
-   [ ] O usuário pode definir o evento inserindo seu nome, a data em que
está agendado para acontecer, e uma hora opcional do evento. Se a hora for
omitida, assume-se que seja à Meia-noite na data do evento no fuso
horário local.
-   [ ] O usuário pode ver uma mensagem de aviso se o nome do evento estiver em branco.
-   [ ] O usuário pode ver uma mensagem de aviso se a data ou hora do evento estiverem
incorretos. 
-   [ ] O usuário pode ver uma mensagem de aviso se o tempo até a data e hora
do evento inserido exceder a precisão do temporizador de contagem regressiva.
-   [ ] O usuário pode clicar no botão 'Iniciar' para ver o temporizador de contagem regressiva
começar exibindo os dias, horas, minutos, e segundos até o evento.
-   [ ] O usuário pode ver os elementos do temporizador de contagem regressiva
decrementarem automaticamente. Por exemplo, quando a contagem de segundos
restantes chega a 0, a contagem de minutos restantes decrementará em 1 e
os segundos começarão a contar regressivamente de 59. Essa progressão deve
ocorrer desde os segundos até a posição de dias restantes na
exibição da contagem regressiva. 

## Funcionalidades Bônus

-   [ ] O usuário pode salvar o evento para que persista entre sessões
-   [ ] O usuário pode ver um alerta quando o evento for atingido
-   [ ] O usuário pode especificar mais de um evento. 
-   [ ] O usuário pode ver temporizadores de contagem regressiva para cada evento definido.

## Links e Recursos Úteis

- Imagens de temporizadores de contagem regressiva analógicos baseados em tubos podem ser encontrados 
[aqui](https://nixieshop.com/)
- [`clearInterval` MDN](https://developer.mozilla.org/en-US/docs/Web/API/WindowOrWorkerGlobalScope/clearInterval)
- [`setInterval` MDN](https://developer.mozilla.org/en-US/docs/Web/API/WindowOrWorkerGlobalScope/setInterval)
- [Date MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)

## Projetos de Exemplo

[Relógio/Countdown Timer Simples](https://codepen.io/karlo-stekovic/pen/OajKVK)
[Countdown Timer construído com React](https://www.florin-pop.com/blog/2019/05/countdown-built-with-react/)