# MultiNova

O **MultiNova** é um sistema de gestão de vendas desenvolvido para auxiliar pequenos negócios no controle de **produtos, estoque, clientes, vendas e contas**.

Este repositório concentra a **documentação pública do projeto**, incluindo requisitos, arquitetura, modelagem de dados, diagramas e contrato da API.

> Os repositórios responsáveis pela implementação do backend e frontend são mantidos de forma privada.

## Tecnologias

### Backend

* Java
* Spring Boot
* Spring Security
* JWT
* PostgreSQL

### Frontend

* React

## Documentação

A documentação do projeto está disponível no diretório [`docs`](./docs).

```text
docs/
├── architecture/
│   ├── adr/            # Architecture Decision Records
│   ├── diagrams/       # Diagramas de arquitetura e fluxos
│   └── der.md          # Modelo de dados
│
├── requirements/
│   ├── functional.md   # Requisitos do sistema
│   └── use-cases.md    # Casos de uso
│
└── api/
    └── openapi.yaml    # Contrato OpenAPI da API
```

## Principais funcionalidades

* Gerenciamento de produtos e estoque
* Histórico de preços
* Cadastro e acompanhamento de clientes
* Registro e histórico de vendas
* Controle de contas e pagamentos
* Autenticação e gerenciamento de usuários

## Arquitetura

A aplicação é composta por um **frontend web independente** e uma **API REST**, responsável pelas regras de negócio, persistência e autenticação.

Mais detalhes estão disponíveis em [`docs/architecture`](./docs/architecture).

## API

O contrato da API é documentado utilizando **OpenAPI 3.0.3**:

[`docs/api/openapi.yaml`](./docs/api/openapi.yaml)

## Status

🚧 **Em desenvolvimento**

O projeto está sendo desenvolvido de forma incremental, com documentação e arquitetura evoluindo juntamente com a implementação.

