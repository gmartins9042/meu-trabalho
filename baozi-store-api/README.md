# Baozi Store API

API REST simples em Java com Spring Boot, Spring Data JPA e banco H2 para o trabalho de Desenvolvimento Web Back-End.

## Tecnologias

- Java 21
- Spring Boot
- Spring Data JPA
- Banco relacional H2
- JSON nos endpoints
- Arquitetura MVC com pacotes `model`, `repository` e `controller`

## Como executar

1. Abra a pasta `baozi-store-api` no IntelliJ IDEA ou em outra IDE Java.
2. Aguarde a IDE baixar as dependencias do Maven.
3. Execute a classe `BaoziStoreApiApplication`.
4. A API ficara disponivel em `http://localhost:8080`.

Se o Maven estiver no PATH, tambem e possivel executar:

```bash
mvn spring-boot:run
```

## Endpoints

### Clientes

- `POST /clientes`
- `GET /clientes`
- `GET /clientes/{id}`
- `PUT /clientes/{id}`
- `DELETE /clientes/{id}`

### Produtos

- `POST /produtos`
- `GET /produtos`
- `GET /produtos/{id}`
- `PUT /produtos/{id}`
- `DELETE /produtos/{id}`

### Pedidos

- `POST /pedidos`
- `GET /pedidos`
- `GET /pedidos/{id}`
- `PUT /pedidos/{id}`
- `DELETE /pedidos/{id}`

## Exemplos de JSON

Cliente:

```json
{
  "nome": "Aluno123456",
  "clienteDesde": "2026-09-14"
}
```

Produto:

```json
{
  "nome": "Baozi Tradicional",
  "preco": 9.90,
  "estoque": true
}
```

Pedido:

```json
{
  "clienteId": 1,
  "produtoId": 1,
  "quantidade": 3
}
```

## Postman

Importe o arquivo `postman/Baozi Store API.postman_collection.json` no Postman e execute as requisicoes na ordem em que aparecem.
