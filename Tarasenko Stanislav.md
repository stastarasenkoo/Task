# Tarasenko Stanislav
## Project name
GS(Gold Specialist)
## Description
Application for hosting a wide range of services. On this platform, any user can use the service of various specialists (tutor, plumber, driver, electrician, programmer). The customer can order the service of any specialist. Specialists, in turn, can post a list of their services and their work schedule.
## Tecnology stack
* .NET 6
* ASP.NET Core
* EF Core
* MS SQL
* PostgreSQL
* Docker
* Kafka
* Envoy
* IdentityServer4
* MediatR
* AutoMapper
* FluentValidation

## Microservices
* Identity service
  * Architecture: N-tier (WebApi tier, Logic tier, Data access tier)
  * Technologies: AutoMapper, FluentValidation, IdentityServer 4, EF Core
  * Responsibilities: registration, authentication, changing user data
  * Database: MS SQL

* Catalog service
  * Architecture: CQRS
  * Technologies: AutoMapper, FluentValidation, EF Core, MediatR
  * Responsibilities: catalog management, it's display
  * Database: PostgreSQL

* Basket service
  * Architecture: N-tier (WebApi tier, Logic tier, Data access tier)
  * Technologies: AutoMapper, FluentValidation, EF Core
  * Responsibilities: orders management, it's display
  * Database: PostgreSQL
## Architecture schema
![Screenshot_1](https://user-images.githubusercontent.com/64153866/180670264-5a45cccb-69e2-414a-8bda-56ba391795ca.png)
