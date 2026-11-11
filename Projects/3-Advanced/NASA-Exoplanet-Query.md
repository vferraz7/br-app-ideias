# Consulta de Exoplanetas da NASA

**Nível:** 3-Avançado

Desde 1992 mais de 4.000 exoplanetas foram descobertos fora do nosso sistema solar. A Administração Nacional de Aeronáutica e Espaço dos Estados Unidos (NASA) mantém um arquivo publicamente acessível dos dados coletados sobre eles em formato de valores separados por vírgula (CSV).

O objetivo do app Consulta de Exoplanetas da NASA é disponibilizar esses dados para consultas simples por seus usuários.

### Requisitos e Restrições

- O Desenvolvedor deve implementar um meio de carregar eficientemente os dados CSV de exoplanetas obtidos da NASA para minimizar quaisquer atrasos quando a aplicação inicia.
- Da mesma forma, o Desenvolvedor deve utilizar uma estrutura de dados e mecanismo de busca que minimize o tempo necessário para consultar os dados de exoplanetas e exibir os resultados.
- O Desenvolvedor precisará revisar a documentação do Arquivo de Exoplanetas para entender o formato dos campos de dados.

## Histórias de Usuário

-   [ ] O usuário pode ver um painel de entrada de consulta contendo listas suspensas permitindo ao usuário consultar por ano de descoberta, método de descoberta, nome do hospedeiro, e instalação de descoberta.
-   [ ] O usuário também pode ver botões 'Limpar' e 'Buscar' no painel de entrada de consulta.
-   [ ] O usuário pode selecionar um único valor de qualquer uma ou todas as listas suspensas de consulta.
-   [ ] O usuário pode clicar no botão 'Buscar' para buscar exoplanetas correspondentes a todos os valores de consulta selecionados.
-   [ ] O usuário pode ver uma mensagem de erro se o botão 'Buscar' foi clicado, mas nenhum valor de consulta foi selecionado.
-   [ ] O usuário pode ver os dados de exoplanetas correspondentes exibidos em formato tabular em um painel de resultados abaixo do painel de consulta. Apenas os campos consultáveis devem ser exibidos.
-   [ ] O usuário pode clicar no botão 'Limpar' para resetar as seleções de consulta e limpar quaisquer dados exibidos no painel de resultados, se uma busca foi realizada.

## Funcionalidades Bônus

-   [ ] O usuário pode ver o nome do hospedeiro como um hiperlink para a Página de Visão Geral do Planeta Confirmado da NASA para aquele planeta
-   [ ] O usuário pode clicar no nome do hospedeiro para exibir a Página de Visão Geral do Planeta Confirmado em uma nova aba do navegador.
-   [ ] O usuário pode ver ícones (como símbolos de cima e baixo) nos cabeçalhos das colunas
-   [ ] O usuário pode clicar no símbolo de cima para ordenar as linhas no painel de resultados em ordem crescente nos valores daquela coluna.
-   [ ] O usuário pode clicar no símbolo de baixo para ordenar as linhas no painel de resultados em ordem decrescente nos valores da coluna.

## Links e Recursos Úteis

- [Notação Big O (Wikipedia)](https://en.wikipedia.org/wiki/Big_O_notation)
- [CSV2JSON](../1-Beginner/CSV2JSON-App.md)
- [Exoplaneta (Wikipedia)](https://en.wikipedia.org/wiki/Exoplanet)
- [Arquivo de Exoplanetas da NASA](https://exoplanetarchive.ipac.caltech.edu/cgi-bin/TblView/nph-tblView?app=ExoTbls&config=planets)

## Projetos de Exemplo

N/a