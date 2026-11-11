# Vigenere Cipher

**Nível:** 1-Iniciante

A taxa e impacto de violações de segurança nos últimos anos torna
imperativo que desenvolvedores entendam os métodos que atores mal-intencionados
usam para comprometer apps. 
Entender como um app pode ser comprometido é o primeiro passo para
criar medidas de proteção eficazes.

Uma das formas mais fáceis de atores mal-intencionados comprometerem um app é
acessando dados que são deixados sem criptografia pelo desenvolvedor. Existem
vários algoritmos de criptografia fortes disponíveis para garantir que
dados não sejam legíveis mesmo se o acesso for comprometido. Entre eles
estão AES, Blowfish, and TripleDES para citar alguns. 

No entanto, esses algoritmos podem ser bastante complexos de implementar então
o objetivo deste app é implementar um algoritmo de criptografia clássico,
a Cifra de Vigenère para aprender o básico de como cifras funcionam.

### Requisitos & Restrições

- Desenvolvedores devem usar apenas recursos nativos da linguagem para implementar
  a Cifra de Vigenère. Bibliotecas não são permitidas.
- Desenvolvedores devem projetar e implementar sua própria solução usando
  apenas a descrição dos passos do algoritmo da Cifra de Vigenère.
- Após implementar com sucesso este algoritmo, o desenvolvedor deve se
  perguntar:
    - Você se sentiria confiante criptografando suas informações financeiras
      usando a Cifra de Vigenère? Por quê?
    - Como você detectaria que uma mensagem foi criptografada usando a
      Cifra de Vigenère?
    - Como você iria tentar quebrar essa criptografia?

## Histórias de Usuário

-   [ ] O usuário pode ver a janela do app com estes componentes:
    - Campo de entrada de texto em claro
    - Campo de entrada de chave de criptografia
    - Botões de ação - 'Criptografar' and 'Decifrar'
    - Resultado da mensagem criptografada or decifrada
-   [ ] O usuário pode inserir o texto a ser criptografado no campo de
    entrada de texto em claro
-   [ ] O usuário pode inserir a Chave de Criptografia que o algoritmo de
    Vigenère usará para criptografar o texto em claro.
-   [ ] O usuário pode ver o botão 'Decifrar' desabilitado até que o texto
    em claro tenha sido criptografado.
-   [ ] O usuário pode clicar no botão 'Criptografar' para criptografar o
    texto em claro
-   [ ] O usuário pode ver a mensagem criptografada exibida no campo de
    resultado.
-   [ ] O usuário pode ver o botão 'Decifrar' habilitado após a mensagem
    criptografada ser exibida.
-   [ ] O usuário pode clicar no botão 'Decifrar' para decifrar a mensagem
    criptografada and exibir seu conteúdo no campo de resultado.

## Funcionalidades Bônus

-   [ ] O usuário pode ver um botão 'Comparar' após a decifração que
    compara a
    mensagem original em claro com a mensagem decifrada
-   [ ] O usuário pode ver uma mensagem de erro se o 'Comparar' detectar
    diferenças
    no conteúdo desses dois campos.

## Links e Recursos Úteis

- [Bad Actors](http://solenski.com/resources/introduction-to-cybersecurity/part-1-cybersecurity-overview)
- [Vigenere Cypher](https://www.geeksforgeeks.org/vigenere-cipher/)

## Projetos de Exemplo

[Vigenere Encryption](https://codepen.io/max1128/pen/VdyJmd)