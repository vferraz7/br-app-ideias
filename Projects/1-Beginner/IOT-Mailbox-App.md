# IOT Mailbox Simulator

**Nível:** 1-Iniciante

O objetivo do IOT Mailbox Simulator é imitar como uma caixa de correio física
habilitada para Internet das Coisas (IOT) poderia ser usada para notificá-lo quando
a "correio lento" chegar. Ao fazer isso, ele fornecerá experiência no uso
de callbacks para comunicar estado entre diferentes componentes de um app
que dependem uns dos outros.

### Requisitos e Restrições

- Embora este app seja especificado usando conceitos e terminologia de
Javascript, você é livre para implementá-lo na linguagem de sua escolha. 

- A seguinte classe Javascript é fornecida para iniciar e parar o processo de
monitoramento, e para sinalizar a página web do app com o estado da porta da
caixa de correio (aberta ou fechada) em intervalos pré-definidos. Lembre-se que
o intervalo que você especificar não deve exceder o tempo que normalmente leva
para abrir ou fechar a porta ou você pode perder uma entrega!
```
/**
 * Monitor light levels inside an IOT enabled snail mailbox to detect
 * when the mailbox door has been opened and closed.
 * @class IOTMailbox
 */
class IOTMailbox {
  /**
   * Creates an instance of IOTMailbox.
   * @param {number} [signalInterval=500] Timer interval for checking mailbox status.
   * @param {function} signalCallback Function to invoke when the timer interval expires.
   * @memberof IOTMailbox
   */
  constructor(signalInterval = 500, signalCallback) {
    this.signalInterval = signalInterval;
    this.signalCallback = signalCallback;
    this.intervalID = null;
    this.lastLightLevel = 0;
  }

  /**
   * Start monitoring of the mailbox and invoke the caller specified callback
   * function when the interval expires.
   * @memberof IOTMailbox
   */
  startMonitoring = () => {
    console.log(`Starting monitoring of mailbox...`);
    this.intervalID = window.setInterval(this.signalStateChange, this.signalInterval);
  }

  /**
   * Stop monitoring the mailbox status
   * @memberof IOTMailbox
   */
  stopMonitoring = () => {
    if (this.intervalID === null) return;
    window.clearInterval(this.intervalID);
    this.intervalID = null;
    console.log(`Mailbox monitoring stopped...`);
  }

  /**
   * Pass the current light level inside the mailbox to the users callback
   * function. The positive light levels indicate the door is open while 
   * negative levels indicate it is closed. Depending on the sampling interval 
   * the mailbox door could be in any position from fully closed to fully open. 
   * This means the light level varies from interval-to-interval.
   * @memberof IOTMailbox
   */
  signalStateChange = () => {
    const lightLevel = this.lastLightLevel >= 0 
      ? Math.random().toFixed(2) * -1 
      : Math.random().toFixed(2);
    console.log(`Mailbox state changed - lightLevel: ${lightLevel}`);
    this.signalCallback(this.lightLevel);
    this.lastLightLevel = lightLevel;
  }
};
```

## Histórias de Usuário

-   [ ] O usuário pode ver uma página web contendo um painel de controle com três
    botões - 'Iniciar Monitoramento', 'Parar Monitoramento', e 'Reset'.
-   [ ] O usuário pode ver um painel de notificações onde o status da caixa de
    correio será exibido.
-   [ ] O usuário pode ver um painel de log rolável onde detalhes de execução
    descrevendo a operação do app e interface com a instância IOTMailbox
    serão exibidos.
-   [ ] O usuário pode clicar no botão 'Iniciar Monitoramento' para começar a
    receber notificações de estado da caixa de correio.
-   [ ] O usuário pode ver uma mensagem adicionada ao painel de log quando o
    monitoramento inicia.
-   [ ] O usuário pode ver uma mensagem adicionada ao painel de log para nível de
    luz passado através da função de callback. Isso deve incluir o nível
    numérico de luz e se a porta está aberta ou fechada.
-   [ ] O usuário pode ver uma mensagem adicionada ao painel de notificações quando
    a porta tiver sido aberta.
-   [ ] O usuário pode clicar no botão 'Parar Monitoramento' para parar de receber
    notificações de estado da caixa de correio. 
-   [ ] O usuário pode ver uma mensagem adicionada ao painel de log quando o
    monitoramento para.

## Funcionalidades Bônus

-   [ ] O usuário pode ver o botão 'Iniciar Monitoramento' desabilitado até que o
    monitoramento seja parado.
-   [ ] O usuário pode ver o botão 'Parar Monitoramento' desabilitado até que o
    monitoramento seja iniciado.
-   [ ] O usuário pode ver um campo no painel de controle permitindo que o
    comprimento do intervalo de monitoramento seja especificado. 
-   [ ] O usuário pode ver uma mensagem adicionada ao painel de notificações se a
    porta for deixada aberta.
-   [ ] O usuário pode ouvir um alerta audível quando a porta for aberta.

## Links e Recursos Úteis

- [Snail Mail (Wikipedia)](https://en.wikipedia.org/wiki/Snail_mail)
- [Internet of Things (Wikipedia)](https://en.wikipedia.org/wiki/Internet_of_things)
- [IOT Mailbox: An Introduction](https://iotexpert.com/2018/08/13/iot-mailbox-an-introduction/)
- [What the Heck is a Callback?](https://codeburst.io/javascript-what-the-heck-is-a-callback-aba4da2deced)
- [window.setInterval (MDN)](https://developer.mozilla.org/en-US/docs/Web/API/WindowOrWorkerGlobalScope/setInterval)

## Projetos de Exemplo

N/a