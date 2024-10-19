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
