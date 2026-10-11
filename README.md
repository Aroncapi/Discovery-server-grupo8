# discovery-server-grupo08

Servidor de descubrimiento **Netflix Eureka** para la red hospitalaria y plataforma de
telemedicina **ClinicaCloud S.A.C.** (Curso 0268 - Desarrollo de Aplicaciones Web II).

Todos los microservicios y el API Gateway se registran en este servidor.

## Requisitos

| Elemento | Versión |
|----------|---------|
| Java | 25 |
| Spring Boot | 4.1.1 |
| Spring Cloud | 2025.1.3 |
| Maven | 3.9+ |
| Puerto | 8761 |

## Ejecutar

```bash
mvn spring-boot:run
```

o empaquetar y ejecutar:

```bash
mvn clean package
java -jar target/discovery-server-grupo08-1.0.0.jar
```

## Verificar

* Dashboard: <http://localhost:8761/>
* Health: <http://localhost:8761/actuator/health>

## Servicios esperados en el dashboard

| Servicio | Puerto |
|----------|--------|
| discovery-server-grupo08 | 8761 |
| api-gateway-grupo08 | 8070 |
| cita-service-grupo08 | 8081 |
| paciente-service-grupo08 | 8082 |
| config-server-grupo08 | 8888 |
