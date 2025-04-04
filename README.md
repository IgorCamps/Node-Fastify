# CRUD com Node.js, Fastify e PostgreSQL

Este projeto consiste em um CRUD (Create, Read, Update, Delete) desenvolvido com **Node.js** e **Fastify**, utilizando **PostgreSQL** como banco de dados, hospedado no **Neon Console**, e deploy realizado no **Render**.

## 🚀 Tecnologias Utilizadas
- **Node.js**
- **Fastify**
- **PostgreSQL** (Neon Console)
- **Render** (Deploy)
- **dotenv** (Gerenciamento de variáveis de ambiente)
- **pg** (Cliente PostgreSQL para Node.js)

## 📌 Funcionalidades
- Criar um novo registro (Create)
- Listar registros existentes (Read)
- Atualizar um registro (Update)
- Remover um registro (Delete)

## 🔧 Como Executar o Projeto

### 1. Clone o repositório
```sh
git clone https://github.com/seu-usuario/nome-do-repo.git
cd nome-do-repo
```

### 2. Instale as dependências
```sh
npm install
```

### 3. Configure as variáveis de ambiente
Crie um arquivo **.env** na raiz do projeto e adicione as credenciais do banco de dados:
```env
PGHOST='seu-host-no-neon'
PGDATABASE='seu-banco'
PGUSER='seu-usuario'
PGPASSWORD='sua-senha'
```

### 4. Execute as migrações (caso tenha scripts para criar tabelas)
```sh
npm run migrate
```

### 5. Inicie o servidor
```sh
npm run dev
```
O servidor será iniciado em `http://localhost:3000`

## 🌍 Deploy no Render
Este projeto está hospedado no **Render**. Para acessar a aplicação, utilize o link:
🔗 [Seu-Link-No-Render](https://seu-app.render.com)

## 📜 Rotas da API
### Criar um vídeo
```http
POST /videos
```
**Body:**
```json
{
  "title": "Nome do vídeo",
  "description": "Descrição do vídeo",
  "duration": 120
}
```

### Listar vídeos
```http
GET /videos
```

### Atualizar um vídeo
```http
PUT /videos/:id
```
**Body:**
```json
{
  "title": "Novo Nome",
  "description": "Nova Descrição",
  "duration": 150
}
```

### Deletar um vídeo
```http
DELETE /videos/:id
```

## 🛠 Possíveis Melhorias
- Adicionar autenticação com JWT
- Implementar testes automatizados
- Criar uma interface frontend para consumir a API

## 📝 Licença
Este projeto está sob a licença MIT. Sinta-se à vontade para utilizá-lo e melhorá-lo!

---
Feito com 💙 por [Seu Nome](https://github.com/seu-usuario)

