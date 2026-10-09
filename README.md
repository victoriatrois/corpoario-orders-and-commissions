# Pedidos e Encomendas

Microsserviço inicial da plataforma de ateliê digital, baseado em Java 25 e Quarkus.

## Requisitos

- JDK 25
- Maven 3.9 ou superior
- PostgreSQL disponível durante a execução

## Executar em modo de desenvolvimento

Defina as variáveis de conexão. Exemplo para uma instância local:

```sh
export DB_USERNAME=postgres
export QUARKUS_DATASOURCE_PASSWORD='<senha do banco>'
export DB_JDBC_URL=jdbc:postgresql://localhost:5432/corpoario_orders
mvn quarkus:dev
```

O Quarkus disponibiliza os endpoints de health em `/q/health`, métricas Prometheus
em `/q/metrics` e a especificação OpenAPI em `/q/openapi`.

O projeto contém somente a configuração inicial e as dependências da aplicação.
Entidades, endpoints, regras de negócio e componentes de mensageria serão
implementados posteriormente.