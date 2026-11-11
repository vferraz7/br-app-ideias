# Gerador de Badge com QRCode

**Nível:** 2-Intermediário

Em algum momento da sua carreira, você provavelmente se verá envolvido ajudando a coordenar um evento patrocinado por uma empresa ou um Meetup técnico local. Não é incomum nesses tipos de encontros que os participantes queiram trocar informações de contato entre si.

Mas como fazer isso? Os participantes poderiam sempre trocar cartões de visita ou anotar o e-mail ou nomes de contas de mídia social uns dos outros, mas isso pode ser lento e propenso a erros. Não seria legal poder escanear os badges uns dos outros para capturar esse tipo de informação rapidamente e de forma mais confiável?

Se você respondeu "Sim!" a esta pergunta, o Gerador de Badge com QRCode é um app no qual você se interessará em criar. O objetivo desta aplicação é coletar o nome de um participante do encontro, endereço de e-mail, Twitter e nomes de contas do GitHub e imprimir um crachá com um QRcode que pode ser escaneado usando um smartphone.

### Requisitos e Restrições

- Para este app, você vai querer usar o pacote NPM [Gerador de QRCode](https://www.npmjs.com/package/qrcode-generator) para codificar as informações que você coleta do participante em um QR code.

- Para testar sua implementação, você precisará baixar um leitor de QR code no seu smartphone ou tablet. Existem muitos desses leitores que são gratuitos. Verifique a loja de aplicativos do seu dispositivo para encontrar o que melhor atende às suas necessidades.

## Histórias de Usuário

-   [ ] O usuário pode ver um painel de entrada contendo campos de entrada para o nome do participante, endereço de e-mail, nome da conta do Twitter, nome da conta do GitHub, e botões 'Cancelar' e 'Criar'.
-   [ ] O usuário pode inserir dados nestes campos de entrada. Note que o nome do participante e o endereço de e-mail são obrigatórios, mas os nomes das contas do Twitter e GitHub são campos opcionais.
-   [ ] O usuário pode clicar no botão 'Cancelar' para limpar todos os campos de entrada, bem como o painel do badge (veja abaixo) se ele tiver sido criado.
-   [ ] O usuário pode clicar no botão 'Criar' para gerar uma imagem do crachá do participante.
-   [ ] O usuário pode ver uma mensagem de erro se qualquer um dos seguintes for verdadeiro:
    - Campos obrigatórios estão vazios
    - Nome e sobrenome não foram inseridos
    - O campo de e-mail não é um endereço de e-mail formatado corretamente
    - O nome da conta do Twitter não começa com '@'
-   [ ] O usuário pode ver um painel de badge exibido na tela contendo estas informações, mais um QR code codificado com estas informações.

## Funcionalidades Bônus

-   [ ] O usuário pode ver um botão 'Imprimir' abaixo do painel do badge.
-   [ ] O usuário pode ver o botão 'Imprimir' habilitado apenas após os campos de entrada terem sido validados e o badge exibido no painel do badge.
-   [ ] O usuário pode fazer correções nos campos de entrada e clicar em 'Criar' para atualizar o conteúdo do painel do badge.
-   [ ] O usuário pode clicar no botão 'Imprimir' para reproduzir o painel do badge em uma etiqueta ou impressão física.
-   [ ] O usuário pode ver o símbolo '@' adicionado automaticamente ao nome da conta do Twitter para que não precise ser inserido manualmente.

## Links e Recursos Úteis

- [QR code (Wikipedia)](https://en.wikipedia.org/wiki/QR_code)
- [Gerador de QRCode](https://www.npmjs.com/package/qrcode-generator)

## Projetos de Exemplo

[Gerador de QRCode](https://kazuhikoarase.github.io/qrcode-generator/js/demo/)