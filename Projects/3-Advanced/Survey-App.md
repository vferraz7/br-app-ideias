# App de Pesquisa

**Nível:** 3-Avançado

Pesquisas são uma parte valiosa da caixa de ferramentas de qualquer desenvolvedor. Elas são úteis para obter feedback de seus usuários sobre uma variedade de tópicos, incluindo satisfação com a aplicação, requisitos, necessidades futuras, problemas, prioridades, e simples aborrecimentos, para citar alguns.

O app de Pesquisa dá a você a oportunidade de aprender desenvolvendo um app completo que você pode adicionar à sua caixa de ferramentas. Ele fornece a capacidade de definir uma pesquisa, permitir que usuários respondam dentro de um período predefinido, e tabular e apresentar resultados.

Usuários deste app são divididos em dois papéis distintos, cada um com requisitos diferentes:

-   _Coordenadores de Pesquisa_ definem e conduzem pesquisas. Esta é uma função administrativa não disponível para usuários normais.
-   _Respondentes de Pesquisa_ Completam pesquisas e visualizam resultados. Eles não têm privilégios administrativos dentro do app.

Ferramentas comerciais de pesquisa incluem funcionalidade de distribuição que envia pesquisas em massa por e-mail para Respondentes de Pesquisa. Por simplicidade, este app assume que pesquisas abertas para respostas serão acessadas a partir da página web do app.

## Histórias de Usuário

### Geral

-   [ ] Coordenadores de Pesquisa e Respondentes de Pesquisa podem definir, conduzir, e visualizar pesquisas e resultados de pesquisas a partir de um site comum
-   [ ] Coordenadores de Pesquisa podem fazer login no app para acessar funções administrativas, como definir uma pesquisa.

### Definindo uma Pesquisa

-   [ ] Coordenador de Pesquisa pode definir uma pesquisa contendo 1-10 perguntas de múltipla escolha.
-   [ ] Coordenador de Pesquisa pode definir 1-5 seleções mutuamente exclusivas para cada pergunta.
-   [ ] Coordenador de Pesquisa pode inserir um título para a pesquisa.
-   [ ] Coordenador de Pesquisa pode clicar no botão 'Cancelar' para retornar à página inicial sem salvar a pesquisa.
-   [ ] Coordenador de Pesquisa pode clicar no botão 'Salvar' para salvar uma pesquisa.

### Conduzindo uma Pesquisa

-   [ ] Coordenador de Pesquisa pode abrir uma pesquisa selecionando uma pesquisa de uma lista de pesquisas definidas anteriormente
-   [ ] Coordenadores de Pesquisa podem fechar uma pesquisa selecionando-a de uma lista de pesquisas abertas
-   [ ] Respondente de Pesquisa pode completar uma pesquisa selecionando-a de uma lista de pesquisas abertas
-   [ ] Respondente de Pesquisa pode selecionar respostas para perguntas da pesquisa clicando em uma caixa de seleção
-   [ ] Respondentes de Pesquisa podem ver que uma resposta selecionada anteriormente será automaticamente desmarcada se uma resposta diferente for clicada.
-   [ ] Respondentes de Pesquisa podem clicar no botão 'Cancelar' para retornar à página inicial sem enviar a pesquisa.
-   [ ] Respondentes de Pesquisa podem clicar no botão 'Enviar' para submeter suas respostas à pesquisa.
-   [ ] Respondentes de Pesquisa podem ver uma mensagem de erro se 'Enviar' for clicado, mas nem todas as perguntas foram respondidas.

### Visualizando Resultados da Pesquisa

-   [ ] Coordenadores de Pesquisa e Respondentes de Pesquisa podem selecionar a pesquisa a ser exibida a partir de uma lista de pesquisas fechadas
-   [ ] Coordenadores de Pesquisa e Respondentes de Pesquisa podem visualizar resultados da pesquisa em formato tabular mostrando o número de respostas para cada uma das possíveis seleções para as perguntas.

## Funcionalidades Bônus

-   [ ] Respondentes de Pesquisa podem criar uma conta única no app
-   [ ] Respondentes de Pesquisa podem fazer login no app
-   [ ] Respondentes de Pesquisa não podem completar a mesma pesquisa mais de uma vez
-   [ ] Coordenadores de Pesquisa e Respondentes de Pesquisa podem visualizar representações gráficas dos resultados da pesquisa (ex: gráficos de pizza, barras, colunas, etc.)

## Links e Recursos Úteis

Bibliotecas para construir pesquisas:

-   [SurveyJS](https://surveyjs.io/Overview/Library/)

Alguns serviços comerciais de pesquisa incluem:

-   [Survey Monkey](https://www.surveymonkey.com/)
-   [Traversy](https://youtu.be/SSDED3XKz-0)
-   [Typeform](https://www.typeform.com/)

## Projetos de Exemplo

[Questionário JavaScript](https://codepen.io/amyfu/pen/oLChg)

[App de Pesquisa React](https://chamatt.github.io/survey-web-app/#/) ([Código](https://github.com/chamatt/survey-web-app))