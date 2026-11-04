# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objective

Construa uma API REST para administrar um catálogo de livros usando FastAPI. Você praticará rotas HTTP, validação de dados com modelos Pydantic e respostas com códigos de status apropriados.

## 📝 Tasks

### 🛠️ Criar a API e consultar livros

#### Descrição
Crie uma aplicação FastAPI para um catálogo de livros. Armazene os livros em uma lista em memória; cada livro deve ter um identificador inteiro, título e autor. Comece com pelo menos dois livros de exemplo.

#### Requisitos
A aplicação concluída deve:

- Iniciar com FastAPI e poder ser executada localmente com Uvicorn.
- Oferecer `GET /books` para retornar todos os livros.
- Oferecer `GET /books/{book_id}` para retornar um livro pelo identificador.
- Retornar o status HTTP `404` quando o identificador solicitado não existir.
- Permitir que as rotas sejam exploradas pela documentação interativa em `/docs`.


### 🛠️ Adicionar livros com validação

#### Descrição
Permita que clientes adicionem livros ao catálogo. Defina um modelo Pydantic para os dados recebidos e use-o para validar o corpo da requisição.

#### Requisitos
A aplicação concluída deve:

- Oferecer `POST /books` com um corpo contendo título e autor.
- Validar que título e autor não estejam vazios.
- Gerar um identificador único para cada livro criado.
- Adicionar o livro ao catálogo e retornar o livro criado com status HTTP `201`.
- Retornar uma resposta de erro de validação quando os dados enviados forem inválidos.


### 🛠️ Atualizar e remover livros

#### Descrição
Complete as operações do catálogo permitindo atualizar e remover um livro existente. Escolha e documente se a atualização será parcial (`PATCH`) ou substituirá todos os campos (`PUT`).

#### Requisitos
A aplicação concluída deve:

- Oferecer uma rota `PATCH` ou `PUT` em `/books/{book_id}` para atualizar um livro existente.
- Oferecer `DELETE /books/{book_id}` para remover um livro existente.
- Retornar o livro atualizado após uma atualização bem-sucedida.
- Retornar o status HTTP `204` ao remover um livro com sucesso.
- Retornar o status HTTP `404` para atualização ou remoção de um identificador inexistente.
- Demonstrar os fluxos de leitura, criação, atualização e remoção usando `/docs` ou um cliente HTTP.
