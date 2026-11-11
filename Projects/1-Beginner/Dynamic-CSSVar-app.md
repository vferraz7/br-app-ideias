# Dynamic CSS Variables

**Nível:** 1-Iniciante

Variáveis CSS são uma ferramenta poderosa que permite ao desenvolvedor associar um
nome simbólico a um valor, e então usar esse nome na folha de estilos onde
quer que esse valor seja necessário. A vantagem é que quando uma alteração
nesse valor for requerida, ela só precisa ser feita na definição da
variável CSS em vez de em todos os locais onde pode ser usada.

O que pode tornar isso ainda mais poderoso é alterar dinamicamente o valor de uma
variável CSS em tempo de execução.

O objetivo deste app é alterar dinamicamente a cor de fundo de caixas de texto
para permitir que você ganhe experiência usando tanto variáveis CSS quanto
alterando-as dinamicamente de dentro do app.

## Histórias de Usuário

-   [ ] O usuário pode ver três duas caixas para serem usadas para inserir um ID de Usuário e Senha
junto com os botões 'Cancelar' e 'Entrar' abaixo delas. A cor de fundo
padrão das caixas de texto é branca.
-   [ ] O usuário pode inserir um ID de usuário e senha nas caixas de texto.
-   [ ] O usuário pode clicar no botão 'Entrar' para validar o ID de usuário e senha.
-   [ ] O usuário pode ver uma mensagem de aviso se uma ou ambas as caixas de texto contém
espaços e a cor de fundo da caixa de texto vazia mudará para
amarelo claro.
-   [ ] O usuário pode ver uma mensagem de aviso se o ID de usuário não corresponder a 'testuser'
e a cor de fundo da caixa de texto mudará para vermelho claro.
-   [ ] O usuário pode ver uma mensagem de aviso se a senha não corresponder a 'mypassword'
e a cor de fundo da caixa de texto mudará para vermelho claro.
-   [ ] O usuário pode clicar no botão 'Cancelar' para limpar as caixas de texto e
resetar suas cores de fundo para branco.

## Funcionalidades Bônus

-   [ ] O usuário pode ver a cor da borda da caixa de texto mudar quando um erro for
detetado
-   [ ] O usuário pode ver o tamanho e a fonte do conteúdo da caixa de texto mudar
quando um erro for detetado.

## Links e Recursos Úteis

- [Custom properties (--*): CSS variables (MDN)](https://developer.mozilla.org/en-US/docs/Web/CSS/--*)
- [CSSStyleDeclaration (MDN)](https://developer.mozilla.org/en-US/docs/Web/API/CSSStyleDeclaration)

## Projetos de Exemplo

[Dynamic CSS Variables](https://codepen.io/gordawn/pen/oOWBXX)