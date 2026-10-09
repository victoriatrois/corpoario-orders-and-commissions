# Orders and Commissions

Initial microservice for the digital atelier platform, built with Java 25 and Quarkus.

## Requirements

- JDK 25
- Maven 3.9 or later
- PostgreSQL available at runtime

## Run in development mode

Set the database connection variables. Example for a local instance:

```sh
export DB_USERNAME=postgres
export QUARKUS_DATASOURCE_PASSWORD='<database password>'
export DB_JDBC_URL=jdbc:postgresql://localhost:5432/corpoario_orders
mvn quarkus:dev
```

Quarkus provides health endpoints at `/q/health`, Prometheus metrics at `/q/metrics`,
and the OpenAPI specification at `/q/openapi`.

This project contains only the initial configuration and application dependencies.
Entities, endpoints, business rules, and messaging components will be implemented
later.
