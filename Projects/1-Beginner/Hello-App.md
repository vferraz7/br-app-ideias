# Hello

**Nível:** 1-Iniciante

É um fato que aplicações devem fornecer aos usuários a funcionalidade
necessária para realizar alguma tarefa ou objetivo. A eficácia da
funcionalidade do app é o primeiro determinante de como os usuários percebem
os apps que usam. No entanto, não é a única coisa que influencia a
satisfação do usuário.

Os recursos de Interface do Usuário e Experiência do Usuário (UI/UX) que os
desenvolvedores incluem nos apps têm pelo menos uma influência igual na
percepção dos usuários sobre um app. Pode ser uma simplificação, mas UI/UX é
largamente (mas não exclusivamente) preocupado com a "forma" de um app. A
personalização é um aspecto da UX que adapta características e ações ao
usuário individual. Personalizar a funcionalidade do app dessa forma
torna o app mais fácil e agradável de usar.

O objetivo do app Hello é aproveitar geolocalização para obter o país do
usuário para que ele possa então gerar uma saudação personalizada no
idioma nativo do usuário.

### Restrições

-   Desenvolvedores devem usar o serviço [IP-API](http://ip-api.com/docs/api:json)
    para obter o IP dos usuários.
-   Desenvolvedores devem usar o
    serviço [Fourtonfish](https://www.fourtonfish.com/hellosalut/hello/) para
    obter a saudação no idioma nativo dos usuários passando o IP dos
    usuários.
-   Desenvolvedores devem usar uma decodificação de entidades HTML para
    decodificar a mensagem de saudação.

## Histórias de Usuário

-   [ ] O usuário pode ver um painel de login simulado contendo um campo de texto para
        nome de usuário, um campo de texto para senha, e os botões 'Login' e 'Logout'.
-   [ ] O usuário pode inserir um nome de usuário simulado no campo Nome de Usuário.
-   [ ] O usuário pode inserir uma senha simulada no campo Senha. A entrada deve
        ser mascarada para que o usuário veja asteriscos (`*`) para cada caractere
        inserido em vez da senha em texto plano.
-   [ ] O usuário pode clicar no botão 'Login' para realizar um login simulado.
-   [ ] O usuário pode ver uma mensagem se algum ou ambos os campos de entrada estiverem
        vazios e a cor da borda do(s) campo(s) com erro deve ser alterada para
        vermelho.
-   [ ] O usuário pode ver uma mensagem de confirmação de login no formato:
        `<saudação-em-idioma-nativo> <nome-usuario> você logou com sucesso!`
-   [ ] O usuário pode clicar no botão 'Logout' para limpar os campos de texto
        e quaisquer mensagens anteriores.
-   [ ] O usuário pode ver uma nova mensagem quando logado com sucesso no formato:
        `Tenha um ótimo dia <nome-usuario>!`

## Funcionalidades Bônus

-   [ ] O usuário pode ver um campo de texto adicional para um código de idioma que
        será usado para substituir o IP obtido através de geolocalização. Dica:
        isso é um ótimo recurso para testar seu app.
-   [ ] O usuário pode ver informações adicionais de geolocalização após logar que
        inclui pelo menos o endereço IP local, cidade, região, nome do país, CEP,
        longitude, latitude, e fuso horário.

## Links e Recursos Úteis

-   [Form Follows Function (Wikipedia)](https://en.wikipedia.org/wiki/Form_follows_function)
-   [Personalização (Wikipedia)](https://en.wikipedia.org/wiki/Personalization)
-   [Fourtonfish](https://www.fourtonfish.com/hellosalut/hello/)
-   [IP-API](http://ip-api.com/docs/api:json)

## Projetos de Exemplo

[Fourtonfish Hello World](https://fourtonfish.com/hellosalut/helloworld/)