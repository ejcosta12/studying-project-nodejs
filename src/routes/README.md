<h3 align="center">
  Aplicando Requisições e Respostas com NodeJS
</h3>

<p align="center">
  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/ejcosta12/studying-project-nodejs">
  <img alt="javaScript" src="https://img.shields.io/github/languages/top/ejcosta12/studying-project-nodejs">
  <img alt="Size" src="https://img.shields.io/github/repo-size/ejcosta12/studying-project-nodejs">
</p>

## Sobre
API desenvolvida para cadastro de transações em uma conta bancária, podendo ser entrada "income" ou saída "outcome", realizando atualização dos valores disponíveis e informando a soma de entradas, saídas, bem como o total. Caso for efetuada alguma operação de saída que ultrapasse o total disponível em conta, este sistema retorna um erro informando que não é possível ter saldo negativo.

### Tecnologias

- NodeJs
- Express
- UuidV4

### Scripts CLI

#### yarn
Instalação de todas as dependências necessárias.

#### yarn dev:server
Inicialização do sistema pelo node, porta 3333.

#### Testes
Foram realizados testes utilizando o software insomnia, através das seguintes rotas:

- POST http://localhost:3333/transactions

Exemplo body(JSON):
```js
{
	"title": "Desenvolvimento de Sistema",
	"value": 6000,
	"type": "income",
	"category": "Salario"
}
```

- GET http://localhost:3333/transactions
