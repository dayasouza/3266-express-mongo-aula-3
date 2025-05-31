# Livraria
API RESTful para gerenciamento de livros e autores, desenvolvida com Node.js, Express e MongoDB.
Desenvolvida durante o curso de *Node.js: criando uma API Rest com Express e MongoDB da* [Alura](https://github.com/alura-cursos)

## Funcionalidades
- CRUD de livros
- CRUD de autores
- Busca de livros por editora
## Estrutura do Projeto
```
.env
.gitignore
package.json
server.js
src/
  app.js
  config/
    dbConnect.js
  controller/
    autorController.js
    livroController.js
  models/
    Autor.js
    Livro.js
  routes/
    autoresRoutes.js
    index.js
    livrosRoutes.js
```

## Instalação
1. Clone o repositório.
2. Instale as dependências:
```
npm install
```
3. Crie um arquivo .env na raiz do projeto com a variável:
## Uso
Inicie o servidor em modo desenvolvimento:
```
node server.js
```
##### O servidor estará disponível em http://localhost:3000.

## Rotas
### Livros
- GET /livros — Lista todos os livros
- GET /livros/:id — Busca um livro por ID
- GET /livros/busca?editora=NomeEditora — Lista livros por editora
- POST /livros — Cadastra um novo livro
- PUT /livros/:id — Atualiza um livro existente
- DELETE /livros/:id — Remove um livro
### Autores
- GET /autores — Lista todos os autores
- GET /autores/:id — Busca um autor por ID
- POST /autores — Cadastra um novo autor
- PUT /autores/:id — Atualiza um autor existente
- DELETE /autores/:id — Remove um autor
## Tecnologias
- Node.js
- Express
- MongoDB
- Mongoose
- dotenv

Desenvolvido para fins de estudo.