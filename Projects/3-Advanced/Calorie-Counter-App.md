# Contador de Calorias

**Nível:** 3-Avançado

Ficar e se manter saudável requer uma combinação de equilíbrio mental, exercício e nutrição. O objetivo do app Contador de Calorias é ajudar o usuário a atender necessidades nutricionais contando calorias de vários alimentos.

Este app fornece o número de calorias baseado no resultado de uma busca do usuário por um tipo de alimento. Os Dados Brutos de Alimentos MyPyramid do Departamento de Agricultura dos EUA serão buscados para determinar os valores de calorias.

O Contador de Calorias também fornece a você, o desenvolvedor, experiência em transformar dados brutos em um formato que facilitará a busca. Neste caso, o arquivo de Dados Brutos de Alimentos MyPyramid, que é uma planilha do MS Excel, deve ser baixado e transformado em um arquivo JSON que será mais fácil de carregar e buscar em tempo de execução (dica: dê uma olhada no formato de arquivo CSV).

## Histórias de Usuário

-   [ ] O desenvolvedor criará um arquivo JSON contendo os itens de alimentos a serem buscados. Isso será carregado quando o app for iniciado.
-   [ ] O usuário pode ver um painel contendo uma caixa de texto de descrição do alimento, um botão 'Buscar', e um botão 'Limpar'.
-   [ ] O usuário pode inserir termos de busca na caixa de texto de descrição do alimento.
-   [ ] O usuário pode clicar no botão 'Buscar' para buscar o alimento correspondente.
-   [ ] O usuário pode ver uma mensagem de aviso se nenhum termo de busca foi inserido.
-   [ ] O usuário pode ver uma mensagem de aviso se nenhuma correspondência foi encontrada.
-   [ ] O usuário pode ver uma lista dos itens de alimentos correspondentes, tamanhos das porções, e calorias em um painel de resultados rolável limitado a 25 entradas.
-   [ ] O usuário pode clicar no botão 'Limpar' para limpar os termos de busca e a lista de resultados.

## Funcionalidades Bônus

-   [ ] O usuário pode ver a contagem do número de itens de alimentos correspondentes adjacente à lista de resultados.
-   [ ] O usuário pode usar um caractere curinga nos termos de busca.
-   [ ] O usuário pode ver mais de 25 entradas de uma busca clicando no botão de ícone Para Baixo para adicionar mais itens de alimentos correspondentes à lista de resultados da busca.
-   [ ] O desenvolvedor implementará o carregamento dos dados MyPyramid em um banco de dados ou estrutura de dados diferente de um array para buscas mais rápidas.

## Links e Recursos Úteis

[Dados Brutos de Alimentos MyPyramid](https://catalog.data.gov/dataset/mypyramid-food-raw-data)

## Projetos de Exemplo

[Calculadora de Alimentos](https://www.webmd.com/diet/healthtool-food-calorie-counter)