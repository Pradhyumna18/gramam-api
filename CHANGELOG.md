# Changelog

All notable changes are recorded here. Every PR adds an entry under **Unreleased**.

## [Unreleased]

### Added
- Initial Spring Boot 4.1.2 service on Java 25 (LTS), built with Maven.
- Dependencies: `spring-boot-starter-webmvc`, `spring-boot-starter-validation`, `spring-boot-starter-actuator`.
- `application.yml`: virtual threads enabled, graceful shutdown, `PORT` env override (default 8080), actuator `health` and `info` exposed with liveness/readiness probes.
- Tests: application context load, and `/actuator/health` plus liveness/readiness probes report `UP`.
- README with run, test and build instructions.
