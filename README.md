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

para iniciar o banco de dados sqlite local:

```
npm run knex migrate:latest
```

> **Note**      
> A aplicação roda por padrão na porta ```3333```

## 💠 Rotas da api
- [x] GET ```/transactions``` retorna todas as transações do usuário
- [x] GET ```/transactions/summary``` retorna o resumo de todas as transações do usuário
- [x] GET ```/transactions/:id``` retorna os dados de uma transação específica do usuário
- [x] POST ```/transactions``` cria uma transação para aquele usuário

segue o tipagem do objeto para utilizar na rota de criação da transação:

```
{
  title: string,
  amount: number,
  type: 'credit' || 'debit'
}
```

## 🔱 Ferramentas utilizadas
- Node JS com Fastify
- TypeScript
- Knex
- Eslint
- Vitest
- Zod
- Supertest
- Dotenv
- Sqlite3
- Tsup

