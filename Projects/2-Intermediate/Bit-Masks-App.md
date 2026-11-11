# Bit Masks

**Nível:** 2-Intermediário

É difícil encontrar um app que não dependa de alguma forma de lógica
condicional para implementar sua funcionalidade. Isso quase sempre é
realizado usando instruções como:
```
if (processAccount === true) { 
  /* faça algo */
}
```
Se as instruções if and switch funcionam bem para um número limitado de
condicionais, mas e se seu app tivesse 10's ou 100's de condicionais
para avaliar? Felizmente, existe outro caminho.

O objetivo do app Bit Masks é demonstrar como usar bit masks para
avaliar sequências mais longas de interruptores sem precisar confiar em
longas strings de instruções condicionais.

## Histórias de Usuário

-   [ ] O usuário pode ver uma lista vertical de caixas de seleção com as
    seguintes cidades e seus fusos horários:
    - Moscow: GMT +3
    - Paris: GMT +2
    - Berlin: GMT +2
    - Brussels: GMT +2
    - Amsterdam: GMT +2
    - Rome: GMT +2 
    - London: GMT +1
    - Dublin: GMT +1
    - New York: GMT -4
    - Washington, DC: GMT -4
    - St. Louis: GMT -5
    - Los Angeles: GMT -7
    - Tokyo: GMT +9
    - Beijing: GMT +8
    - Ho Chi Mihn City: GMT +7
    - Mumbai: GMT +5
-   [ ] O usuário pode ver uma caixa de busca GMT onde um inteiro representando
    um deslocamento GMT pode ser inserido and um botão 'Buscar Cidades'.
-   [ ] O usuário pode clicar no botão 'Buscar Cidades' para exibir os
    nomes das cidades naquele deslocamento GMT em uma área de saída.

### Notas do Desenvolvedor

Para este exercício o desenvolvedor deve usar sequências de 24 
bits binários, cada um correspondendo a um fuso horário GMT de +12 a -12
para mapear cidades para seus fusos horários. 

Buscas devem ser conduzidas combinando uma bit mask para o fuso horário
desejado contra as sequências específicas das cidades para identificar
correspondências. Determinar se uma cidade atende aos critérios de busca
não deve confiar em uma instrução como
```
if (city[i].gmtOffset === searchOffset ) {
  /* Found it! */
}
```
Em vez disso, deve confiar em uma operação bit-a-bit.

## Funcionalidades Bônus

-   [ ] O usuário pode buscar cidades NÃO no deslocamento GMT inserido na
    caixa de busca.
-   [ ] O usuário pode ver uma contagem de resumo do número de cidades que
    atenderam aos critérios de busca.

## Links e Recursos Úteis

- [World Time Zones](https://greenwichmeantime.com/time-zone/definition/)
- [Bitwise Operators (MDN)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Bitwise_Operators)

## Projetos de Exemplo

[Bitwise Operation](https://codepen.io/Lunoware/pen/VBZgQd)