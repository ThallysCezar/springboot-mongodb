# Project MongoDB

Este é um projeto de exemplo de uma rede social em que cada usuário pode criar seus próprios posts e comentários. O objetivo deste projeto é demonstrar como usar o MongoDB com o framework Spring.

## Funcionalidades

- Cadastro de usuários.
- Criação, leitura, atualização e exclusão de posts.
- Comentários em posts.
- Testes unitários para a camada de serviços.

## Tecnologias Utilizadas

- Spring Boot: para o desenvolvimento da aplicação.
- MongoDB: como banco de dados não relacional.
- Spring Data MongoDB: para integração com o MongoDB.
- JUnit e Mockito: para testes unitários.
- Maven: para gerenciamento de dependências.

## Pré-requisitos

- Java 8 ou superior instalado.
- MongoDB instalado e em execução.
- Uma IDE (Eclipse, IntelliJ, etc.) para execução do projeto.

## Como Executar o Projeto

Siga as etapas abaixo para executar o projeto localmente:


### Rodando Localmente:

1. Clone o repositório do GitHub:

	```bash
	git clone https://github.com/seu-usuario/seu-projeto.git
	cd seu-projeto
	```

2. Importe o projeto em sua IDE.

3. Configure as propriedades do MongoDB no arquivo application.properties:

	```bash
	spring.data.mongodb.host=localhost
	spring.data.mongodb.port=27017
	spring.data.mongodb.database=sua_basededados
	```

  - Execute o aplicativo a partir da classe principal, por exemplo: YourApplication.java.

## Documentação da API: Endpoints da API

### Users

- GET /users: Crie um novo usuário.
- GET /users/{id}: Obtenha informações de um usuário específico.
- POST /users: Crie um novo usuário.
- PUT /users/{id}: Atualize um usuário.
- DELETE /users/{id}: Delete um usuário.

### Posts

- GET /posts/{id}: Obtenha informações de um post específico.
- GET /posts/titlesearch: Obtenha informações de um post com um título específico.
- GET /posts/fullsearch: Obtenha informações de um post.
- GET /users/{id}/posts: Obtenha informações de um post via usuário específico.