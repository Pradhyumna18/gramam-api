# gramam-api

Backend service for Gramam (companion to [gramam-ui](https://github.com/Pradhyumna18/gramam-ui)).

| | |
|---|---|
| Language | Java 25 (LTS) |
| Framework | Spring Boot 4.1.2 (Spring Framework 7) |
| Build | Maven 3.9+ |
| Package | `com.gramam.api` |

## Prerequisites

JDK 25 (e.g. [Temurin 25](https://adoptium.net/temurin/releases/?version=25)) and Maven 3.9+. Check with `java -version` and `mvn -v`.

## Run

```bash
mvn spring-boot:run          # starts on http://localhost:8080 (override with PORT=9000)
```

Health checks:

- `GET /actuator/health`
- `GET /actuator/health/liveness`
- `GET /actuator/health/readiness`

## Test and build

```bash
mvn verify                   # compiles, runs unit tests, builds target/gramam-api-*.jar
java -jar target/gramam-api-0.0.1-SNAPSHOT.jar
```

## Layout

```
src/main/java/com/gramam/api/   application code
src/main/resources/application.yml
src/test/java/com/gramam/api/   tests
```

## Conventions

- Every PR adds a detailed entry to [CHANGELOG.md](CHANGELOG.md).
- New behaviour ships with unit tests.
