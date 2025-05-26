
# 🎫 Reticketify

**Reticketify** é uma aplicação web para **divulgação de eventos**, onde usuários podem **criar**, **deletar**, **comentar** e **avaliar eventos**. O sistema é composto por um backend que gerencia os dados e por um frontend que permite a visualização e interação dos usuários.

---

## 🧠 Resumo da Aplicação

- 🔥 **Funcionalidades principais:**
  - ✅ Cadastrar eventos
  - ✅ Deletar eventos
  - ✅ Visualizar eventos
  - ✅ Comentar eventos (comentários locais no frontend)
  - ✅ Avaliar eventos com estrelas (também locais no frontend)
  - ✅ Comunicação em tempo real (WebSocket) para novos eventos

- 💻 **Arquitetura:**
  - Backend em Node.js
  - Frontend em Next.js

---

## 🌐 Link da aplicação online

- 🔗 **Frontend (Vercel):** [https://reticketify-vercel-git-main-gustavos-projects-a438ad4b.vercel.app](https://reticketify-vercel-git-main-gustavos-projects-a438ad4b.vercel.app)

---

## 🚀 Tecnologias Utilizadas

| Tecnologia          | Finalidade                                      |
|---------------------|--------------------------------------------------|
| **Frontend**        |                                                  |
| Next.js             | Framework React fullstack                       |
| React               | Biblioteca de UI                                 |
| Axios               | Requisições HTTP                                 |
| Socket.IO Client    | WebSocket para comunicação em tempo real         |
| CSS Modules         | Estilização dos componentes                     |
|                     |                                                  |
| **Backend**         |                                                  |
| Express             | Framework web para rotas                         |
| Socket.IO           | WebSocket para tempo real                        |
| Knex.js             | Query builder + migrations                       |
| SQLite3             | Banco de dados leve e local                      |
| Zod                 | Validação de dados                               |
| @faker-js/faker     | Geração de dados fake para seeds                 |

---

## 🔧 Como rodar o projeto localmente

### 👉 1. Clone o projeto
```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
```

---

### 👉 2. Backend
```bash
cd Back
npm install

# Rodar migrations e seeds
npx knex migrate:latest --env development
npx knex seed:run --env development

# Iniciar backend
npm start
```

O backend estará rodando na porta:
```
http://localhost:3000
```

---

### 👉 3. Frontend
```bash
cd reticketfy-Front
npm install

# Iniciar frontend
npm run dev
```

O frontend estará rodando na porta:
```
http://localhost:3001 (ou porta padrão do Next.js)
```