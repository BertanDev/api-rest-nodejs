# 🧪 Api rest NodeJS🧪
Api Node JS criada usando Fastify e Knex com testes E2E durante aula da @Rocketseat

A api tem a função de controlar o fluxo de caixa do usuário, que pode inserir transações de Crédito e Débito na aplicação.
Não há um sistema de login, porém todo o contexto de usuário é realizado por cookies no próprio navegador, assim a api sabe exatamente qual usuário está realizando a requisição a determinada rota

**O objetivo do projeto é estudo, mas a aplicação está 100% capacitada a ser utilizada por um client front end**

## ▶️ Testando aplicação

com o projeto em sua máquina, rode na raíz
```
npm install
```

em seguida: 

```
npm run dev
```

> **Note**      
> A aplicação roda por padrão na porta ```3333```

## 💠 Rotas da api
- GET ```/transactions``` retorna todas as transações do usuário
- GET ```/transactions/summary``` retorna o resumo de todas as transações do usuário
- GET ```/transactions/:id``` retorna os dados de uma transação específica do usuário
- POST ```/transactions``` cria uma transação para aquele usuário

segue a tipagem da transação:

```
{
  title: string,
  amount: number,
  type: 'credit' || 'debit'
}
```
