
```markdown
# Desafio Neurotech - API REST para Cadastro de Produtos

## Descrição do Desafio
Desenvolvimento de uma API REST para cadastro de produtos com deploy na AWS e banco de dados MySQL.

## Objetivo
Criar uma aplicação backend em Java 17 utilizando Spring Boot, que permita o cadastro completo de produtos (CRUD: Create, Read, Update e Delete). A API deverá ser implantada na AWS utilizando o banco de dados MySQL.

## Requisitos Funcionais

### 1. Cadastro de Produtos (CRUD Completo)
- **Modelo de Produto:**
```json
{
  "id": Long,
  "nome": String,
  "descricao": String,
  "preco": Double,
  "quantidadeEstoque": Integer,
  "dataCriacao": LocalDateTime
}
```
- **Endpoints REST:**
  - `POST /produtos`: Criar um novo produto.
  - `GET /produtos`: Listar todos os produtos.
  - `GET /produtos/{id}`: Obter detalhes de um produto por ID.
  - `PUT /produtos/{id}`: Atualizar um produto existente por ID.
  - `DELETE /produtos/{id}`: Remover um produto por ID.

### 2. Validações
- O nome do produto é obrigatório.
- O preço deve ser maior que zero.
- A quantidade em estoque deve ser um número inteiro positivo.

### 3. Filtros e Ordenação
- Permitir filtrar produtos por nome.
- Possibilitar a ordenação dos resultados pelo preço (ascendente ou descendente).

### 4. Documentação da API
- Utilizar Swagger ou OpenAPI para documentar a API.

## Requisitos Não Funcionais

### 1. Estrutura do Projeto
- Utilizar Java 17 e Spring Boot.
- Arquitetura REST.
- Configurar o projeto com o Maven.

### 2. Banco de Dados
- Utilizar MySQL como base de dados.
- Configurar o acesso ao banco de dados no `application.properties` ou `application.yml`.

### 3. Implantação na AWS
- Implantar a API utilizando Elastic Beanstalk ou EC2.
- O banco de dados deve ser criado no AWS RDS.

### 4. Segurança
- Implementar autenticação básica ou utilizando JWT (opcional, mas será um diferencial).

## Acesso Remoto
Após subir o projeto, você pode acessar a API através do seguinte link:

- **API Produtos:** [http://ec2-18-207-231-146.compute-1.amazonaws.com:8000/produtos](http://ec2-18-207-231-146.compute-1.amazonaws.com:8000/produtos)

- **Swagger UI:** [http://18.207.231.146:8000/swagger-ui/swagger-ui/index.html#/](http://18.207.231.146:8000/swagger-ui/swagger-ui/index.html#/)
```

