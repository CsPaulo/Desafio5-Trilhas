1. Inicializar o Projeto
   No terminal, vá para a pasta do servidor (exemplo: server/):
   cd server
   npm init -y

2. Instalar Dependências
   Instale as principais dependências:
   npm install express cors dotenv
   Instale o nodemon para desenvolvimento (reinício automático):
   npm install -D nodemon

3. Estrutura Básica do Projeto
   /server
   ├── src/
   │ ├── server.js ← arquivo principal do servidor
   │ ├── routes/
   │ ├── controllers/
   │ ├── models/
   │ ├── middlewares/
   │ └── config/
   └── package.json

4. Configurar Script de Desenvolvimento no package.json
   Edite o arquivo package.json e adicione o script:
   "scripts": {
   "dev": "nodemon src/index.js"
   }
   Importante: Se mudar o nome do arquivo principal (index.js), atualize o caminho no script. Exemplo:
   "scripts": {
   "dev": "nodemon src/server.js"
   }

5. Rodar o Servidor
   No terminal, execute:
   npm run dev
