# Seu Primeiro App com DB

**Nível:** 1-Iniciante

Entender conceitos de banco de dados e como usá-los em suas aplicações é
conhecimento que todos os desenvolvedores precisam adquirir. O objetivo do Seu Primeiro App com DB
é fornecer uma introdução suave aos conceitos de banco de dados e aprender um
caso de uso para bancos de dados em um app frontend.

Então, você sabia que navegadores modernos têm um sistema de gerenciamento de
banco de dados embutidos neles? O IndexedDB está presente na maioria dos
navegadores modernos e fornece aos desenvolvedores recursos básicos de banco de
dados, suporte a transações, e persistência cross-session do lado do cliente.

### Requisitos e Restrições

- O caso de uso principal para um banco de dados baseado no navegador é manter estado ou
informações de status que precisam persistir entre sessões, ou como uma área
de trabalho para dados temporários. Por exemplo, dados recuperados de um servidor que
devem ser reformatados ou limpos antes de serem apresentados ao usuário.

- É importante lembrar que, já que o ambiente de cliente do
navegador não pode ser seguro, você não deve manter nenhuma informação
confidencial ou de identificação pessoal (PII) em um banco de dados baseado
no navegador.

- A seguinte classe JavaScript é fornecida com a funcionalidade para
permitir que seu app inicialmente preencha e limpe o banco de dados do
navegador para que você possa testar a lógica de consulta que adicionará. Você
precisará conectar os botões na página web que construir às
funções `clearDB` e `loadDB`, e escrever seu próprio manipulador `queryDB` para
conectar ao botão `Query DB`. Você também precisará adicionar uma
função `queryAllRows` à classe Customer.
```js
class Customer {
  constructor(dbName) {
    this.dbName = dbName;
    if (!window.indexedDB) {
      window.alert("Your browser doesn't support a stable version of IndexedDB. \
        Such and such feature will not be available.");
    }
  }

  /**
   * Remove todas as linhas do banco de dados
   * @memberof Customer
   */
  removeAllRows = () => {
    const request = indexedDB.open(this.dbName, 1);

    request.onerror = (event) => {
      console.log('removeAllRows - Database error: ', event.target.error.code,
        " - ", event.target.error.message);
    };

    request.onsuccess = (event) => {
      console.log('Deleting all customers...');
      const db = event.target.result;
      const txn = db.transaction('customers', 'readwrite');
      txn.onerror = (event) => {
        console.log('removeAllRows - Txn error: ', event.target.error.code,
          " - ", event.target.error.message);
      };
      txn.oncomplete = (event) => {
        console.log('All rows removed!');
      };
      const objectStore = txn.objectStore('customers');
      const getAllKeysRequest = objectStore.getAllKeys();
      getAllKeysRequest.onsuccess = (event) => {
        getAllKeysRequest.result.forEach(key => {
          objectStore.delete(key);
        });
      }
    }
  }

  /**
   * Preencha o banco de dados do Cliente com um conjunto inicial de dados de clientes
   * @param {[object]} customerData Dados a adicionar
   * @memberof Customer
   */
  initialLoad = (customerData) => {
    const request = indexedDB.open(this.dbName, 1);

    request.onerror = (event) => {
      console.log('initialLoad - Database error: ', event.target.error.code,
        " - ", event.target.error.message);
    };

    request.onupgradeneeded = (event) => {
      console.log('Populating customers...');
      const db = event.target.result;
      const objectStore = db.createObjectStore('customers', { keyPath: 'userid' });
      objectStore.onerror = (event) => {
        console.log('initialLoad - objectStore error: ', event.target.error.code,
          " - ", event.target.error.message);
      };

      // Cria um índice para buscar clientes por nome e email
      objectStore.createIndex('name', 'name', { unique: false });
      objectStore.createIndex('email', 'email', { unique: true });

      // Preencha o banco de dados com o conjunto inicial de linhas
      customerData.forEach(function(customer) {
        objectStore.put(customer);
      });
      db.close();
    };
  }
}

// Manipuladores de eventos da página web
const DBNAME = 'customer_db';

/**
 * Limpe todos os dados do cliente do banco de dados
 */
const clearDB = () => {
  console.log('Delete all rows from the Customers database');
  let customer = new Customer(DBNAME);
  customer.removeAllRows();
}

/**
 * Adicione dados do cliente ao banco de dados
 */
const loadDB = () => {
  console.log('Load the Customers database');

  // Clientes para adicionar para preencher inicialmente o banco de dados
  const customerData = [
    { userid: '444', name: 'Bill', email: 'bill@company.com' },
    { userid: '555', name: 'Donna', email: 'donna@home.org' }
  ];
  let customer = new Customer(DBNAME);
  customer.initialLoad(customerData);
}
```

## Histórias de Usuário

-   [ ] O usuário pode ver uma página web contendo um painel de controle com três
    botões - 'Carregar DB', 'Consultar DB', e 'Limpar DB'.
-   [ ] O usuário pode ver um painel de notificações onde mensagens de status serão exibidas.
-   [ ] O usuário pode ver um painel de log rolável onde detalhes de execução descrevendo 
    a operação do app e interface com a instância Customer serão exibidos. 
-   [ ] O usuário pode ver um histórico em andamento de mensagens do painel de notificações no
    painel de log.
-   [ ] O usuário pode ver uma área de resultados de consulta rolável onde dados de clientes
    recuperados serão exibidos.
-   [ ] O usuário pode clicar no botão 'Carregar DB' para preencher o banco de dados com dados.
    O botão 'Carregar DB' na sua UI deve ser conectado ao manipulador de eventos
    `loadDB` fornecido. 
-   [ ] O usuário pode ver uma mensagem exibida no painel de notificações quando a 
    operação de carregamento de dados começa e termina.
-   [ ] O usuário pode clicar no botão 'Consultar DB' para listar todos os clientes na 
    área de resultados de consulta. O botão 'Consultar DB' na sua UI deve ser conectado a um
    manipulador de eventos `queryDB` que você adicionará ao programa.
-   [ ] O usuário pode ver uma mensagem no painel de notificações quando a consulta
    começa e termina.
-   [ ] O usuário pode ver uma mensagem na área de resultados de consulta se não houver
    linhas para exibir.
-   [ ] O usuário pode clicar no botão 'Limpar DB' para remover todas as linhas do 
    banco de dados. O botão 'Limpar DB' na sua UI deve ser conectado à
    função `clearDB` fornecida.
-   [ ] O usuário pode ver uma mensagem no painel de notificações quando a
    operação de limpeza começa e termina.

## Funcionalidades Bônus

-   [ ] O usuário pode ver os botões habilitados e desabilitados de acordo com a
    seguinte tabela.

    | Estado                | Carregar DB | Consultar DB | Limpar DB |
    |---------------------|----------|----------|----------|
    | Exibição inicial do app | habilitado  | habilitado  | desabilitado |
    | Carregar DB clicado     | desabilitado | habilitado  | habilitado  |
    | Consultar DB clicado    | desabilitado | habilitado  | habilitado  |
    | Limpar DB clicado     | habilitado  | habilitado  | desabilitado |
    
-   [ ] O usuário pode ver campos de dados adicionais do Cliente incluídos
    além dos presentes no código fornecido. O desenvolvedor deve adicionar data do
    último pedido e total de vendas do ano.
-   [ ] O desenvolvedor deve conduzir uma retrospectiva sobre este projeto:
    - Quais casos de uso você vê para usar IndexedDB em seus apps frontend?
    - Quais vantagens e desvantagens você vê em relação ao uso de um arquivo ou 
    armazenamento local?
    - Em geral, quais critérios você poderia usar para determinar se IndexedDB é
    adequado para seu app. (Dica: 100% sim ou não não é uma resposta válida).


## Links e Recursos Úteis

- [IndexedDB Concepts (MDN)](http://tinyw.in/7TIr)
- [Using IndexedDB (MDN)](http://tinyw.in/w6k0)
- [IndexedDB API (MDN)](http://tinyw.in/GqnF)
- [IndexedDB Browser Support](https://caniuse.com/#feat=indexeddb)

## Projetos de Exemplo

- N/a