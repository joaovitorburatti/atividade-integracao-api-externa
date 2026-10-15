# Integração com API Externa

Projeto desenvolvido para a disciplina de programação, utilizando microsserviços e integração com uma API externa.

## Tecnologias utilizadas

- Java
- Spring Boot
- Maven
- PostgreSQL
- Consul
- Resilience4j
- Caffeine Cache
- API Banco Central (PTAX)

## Funcionalidades

- Comunicação entre `product-api` e `currency-api`.
- Consulta de cotações de moedas no Banco Central.
- Utilização do PostgreSQL como alternativa quando a API externa falha.
- Implementação de Retry e Circuit Breaker.
- Cache de cotações para reduzir chamadas externas.

## Execução

Execute os microsserviços individualmente utilizando o Maven Wrapper:

```
.\mvnw.cmd spring-boot:run
```

A `product-api` utiliza a porta `8000` e a `currency-api` utiliza a porta `8001`.

## Autor

João Vitor Buratti
