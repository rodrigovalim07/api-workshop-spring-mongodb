# Projeto WorkshopMongo

Este projeto é uma API RESTful desenvolvida em Spring Boot com MongoDB, permitindo a manipulação de usuários e posts.

## Tecnologias Utilizadas

- Spring Boot
- MongoDB
- Maven
- Postman

## Estrutura do Projeto

O projeto está estruturado em diferentes pacotes, cada um responsável por uma camada lógica:

- `config`: Configurações do Spring Boot.
- `domain`: Classes de domínio (entidades).
- `dto`: DTOs (Data Transfer Objects) para transferência de dados.
- `repository`: Interfaces de repositório para acesso ao banco de dados.
- `resources`: Controllers REST para manipulação de recursos.
- `services`: Camada de serviço para regras de negócio.
- `resources.exception`: Classes para tratamento de exceções.

Abaixo está uma representação visual do modelo de domínio:
![design](https://github.com/rodrigovalim07/workshop-SpringBoot-MongoDB/assets/109677118/5e6387c6-1a1a-43e5-a208-4a53b4b15bb2)

## Como Executar

Para executar o projeto localmente, siga estas etapas:

1. Clone este repositório.
2. Abra o projeto em sua IDE favorita.
3. Certifique-se de ter o MongoDB instalado e em execução localmente.
4. Execute a classe principal `WorkshopMongoApplication`.
5. Acesse os endpoints REST conforme documentado abaixo.

## Endpoints

### Usuários

- **GET /users**: Retorna todos os usuários.
- **GET /users/{id}**: Retorna um usuário pelo ID.
- **POST /users**: Cria um novo usuário.
- **PUT /users/{id}**: Atualiza um usuário existente.
- **DELETE /users/{id}**: Exclui um usuário existente.

### Posts

- **GET /posts**: Retorna todos os posts.
- **GET /posts/{id}**: Retorna um post pelo ID.
- **GET /posts/titlesearch?text={text}**: Pesquisa posts por título.
- **GET /posts/fullsearch?text={text}&minDate={minDate}&maxDate={maxDate}**: Pesquisa avançada de posts.
  
## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para enviar pull requests ou abrir issues para reportar bugs ou solicitar novas funcionalidades.
