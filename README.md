# Z 🦓

[![Node.js](https://img.shields.io/badge/Node.js-16.x-green.svg)](https://nodejs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.x-blue.svg)](https://www.typescriptlang.org/)
[![React](https://img.shields.io/badge/React-18.x-blue.svg)](https://reactjs.org/)
[![MySQL](https://img.shields.io/badge/MySQL-8.x-orange.svg)](https://www.mysql.com/)
[![Build Status](https://img.shields.io/github/actions/workflow/status/ojuansoares/Z/ci.yml)](https://github.com/ojuansoares/|/actions)

---

## 📝 Descrição do Projeto

O **Z** é uma aplicação de exemplo para estudo e prática de desenvolvimento full-stack, simulando as funcionalidades básicas de uma rede social. Este projeto tem como objetivo integrar um front-end desenvolvido em **React**, um back-end em **Node.js** com **TypeScript** e um banco de dados **MySQL**, utilizando o padrão de arquitetura **MVC (Model-View-Controller)** no back-end.

### Funcionalidades Principais
- **Autenticação de Usuários:** Cadastro, login e controle de permissões (usuário comum e administrador).
- **Publicação de Posts:** Os usuários podem criar, editar e excluir publicações (chamadas de "Zats").
- **Comentários:** Possibilidade de comentar em publicações de outros usuários.
- **Gerenciamento de Endereços:** Cada usuário pode associar um endereço ao seu perfil.
- **Administração:** O administrador pode gerenciar usuários e conteúdos.

---

## 🛠️ Tecnologias Utilizadas

### **Back-End**
- [Node.js](https://nodejs.org/) - Ambiente de execução JavaScript
- [TypeScript](https://www.typescriptlang.org/) - Tipagem estática para JavaScript
- [Express.js](https://expressjs.com/) - Framework para criação de APIs RESTful
- [MySQL](https://www.mysql.com/) - Banco de dados relacional
- [Sequelize](https://sequelize.org/) - ORM para comunicação com o banco de dados
- [JWT (Json Web Token)](https://jwt.io/) - Autenticação e controle de sessões
- [Dotenv](https://www.npmjs.com/package/dotenv) - Gerenciamento de variáveis de ambiente

### **Front-End**
- [React](https://reactjs.org/) - Biblioteca para criação de interfaces de usuário
- [Axios](https://axios-http.com/) - Biblioteca para requisições HTTP
- [Tailwind CSS](https://tailwindcss.com/) - Framework CSS para estilização

---

## 🚀 Como Rodar o Projeto

### Pré-requisitos
- **Node.js** (16.x ou superior)
- **MySQL** (8.x ou superior)
- **Git**
- **Postman** (opcional, para testes de API)

### Configuração Inicial
1. Clone o repositório:
   ```bash
   git clone https://github.com/ojuansoares/Z.git
   cd Z
   ```

2. Configure as variáveis de ambiente:
   - Crie um arquivo `.env` no diretório `back-end/` com os seguintes campos:
     ```
     DB_HOST=localhost
     DB_USER=root
     DB_PASSWORD=sua_senha
     DB_NAME=Z
     JWT_SECRET=sua_chave_secreta
     ```

3. Instale as dependências:
   - **Back-End:**
     ```bash
     cd back-end
     npm install
     ```
   - **Front-End:**
     ```bash
     cd ../front-end
     npm install
     ```

4. Inicie os servidores:
   - **Back-End:**
     ```bash
     cd back-end
     npm run dev
     ```
   - **Front-End:**
     ```bash
     cd ../front-end
     npm start
     ```

---

## 📈 Fluxo de Funcionalidades

1. **Cadastro de Usuário:**
   - O usuário cria uma conta fornecendo nome, email, senha e endereço.
   - A senha é criptografada antes de ser armazenada no banco.

2. **Autenticação:**
   - O usuário faz login com email e senha.
   - Um token JWT é gerado para autenticação em futuras requisições.

3. **Publicação de Posts (Zats):**
   - Usuários autenticados podem criar, editar e excluir posts.

4. **Comentários:**
   - Os usuários podem comentar em posts de outros usuários.

5. **Administração:**
   - Usuários com perfil de administrador podem desativar contas ou excluir conteúdos inadequados.

---

## 💡 Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.

---

## 📧 Contato

**Juan Soares**  
- [LinkedIn](https://www.linkedin.com/in/ojuansoares)
