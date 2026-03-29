## Backend - Drip Store

API desenvolvida para o sistema *projeto-backend-gt3*, responsável por gerenciar usuários, produtos, categorias e autenticação.

---

##  Estrutura do Projeto


projeto-backend-gt3-main/
├── src/
│   ├── config/         # Configurações do projeto
│   ├── controllers/    # Lógica das rotas
│   ├── database/       # Conexão com banco de dados
│   ├── middleware/     # Middlewares (auth, etc)
│   ├── models/         # Modelos (User, Product, Category...)
│   ├── routes/         # Rotas da API
│   ├── services/       # Regras de negócio
│   ├── app.js          # Configuração do app
│   └── server.js       # Inicialização do servidor
│
├── tests/              # Testes automatizados
│   ├── user.test.js
│   ├── product.test.js
│   └── category.test.js
│
├── .env                # Variáveis de ambiente
├── .gitignore
├── package.json
└── package-lock.json


---

##  Tecnologias Utilizadas

* Node.js
* Express
* Sequelize
* PostgreSQL
* JWT (autenticação)
* Jest (testes)
* Supertest

---

##  Como Rodar o Projeto

###  Instalar dependências

```bash
npm install


---

###  Configurar variáveis de ambiente

Crie um arquivo .env na raiz:

env
DB_HOST=seu_host
DB_USER=seu_usuario
DB_PASSWORD=sua_senha
DB_NAME=seu_banco
JWT_SECRET=sua_chave_secreta


---

### Rodar o servidor

```bash
npm run dev


## O servidor será iniciado em:


http://localhost:3000


---

##  Rodar Testes

```bash
npm test


Se houver erro de tempo:

json
"test": "jest --runInBand --forceExit --testTimeout=30000"


---

## Exemplos de Uso da API
Autenticação
POST /login

Exemplo de payload:

{ "email": "usuario@email.com", "password": "senha" }

Resposta:

{ "token": "jwt_token_aqui" }

Exemplo de rota protegida GET /products Authorization: Bearer


---

##  Funcionalidades

* Cadastro e login de usuários
* Autenticação com token JWT
* CRUD de produtos
* CRUD de categorias
* Middleware de autorização
* Integração com banco de dados

---

##  Observações

* Certifique-se de que o banco de dados está rodando corretamente
* Configure corretamente o .env
* Alguns testes dependem da conexão com o banco

---

## Autor

Desenvolvido por Heliton Silva

## Licença
Este projeto está sob a licença ISC.

