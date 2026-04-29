# Documentación Arquitectónica

[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
[![Architecture Documentation](https://img.shields.io/badge/Architecture%20Documentation-2026-blue.svg)](https://github.com/RichardLitt/standard-readme)

Colección completa de diagramas arquitectónicos del sistema de turismo digital en formato PlantUML, incluyendo modelos C4, diagramas de despliegue AWS, integración continua, flujos de negocio y atributos de calidad.

## Table of Contents

* [Background](#background)
* [Usage](#usage)
* [Project Structure](#project-structure)
* [Documentation](#documentation)
* [Contributors](#contributors)

## Background

Este directorio contiene la documentación visual completa de la arquitectura del sistema de turismo digital inteligente. Los diagramas están organizados siguiendo el modelo C4 para proporcionar diferentes niveles de abstracción, desde el contexto de negocio hasta los detalles técnicos de implementación.

La colección incluye diagramas especializados que cubren todos los aspectos arquitectónicos del sistema: desde la vista general del negocio hasta los detalles específicos de infraestructura AWS, pipelines de CI/CD, modelos de datos, flujos de negocio y atributos de calidad.

## Usage

### Exploración por Tipo de Diagrama

* **Modelos C4 (Niveles 1-3):**

  * `c4-model/level-1-context.puml`: Vista general del sistema con actores principales (viajeros, operadores turísticos) y su relación con la plataforma y la nube.
  * `c4-model/level-2-containers.puml`: Aplicaciones principales del sistema (Web, Android, Backend, IA) y su interacción con servicios cloud.
  * `c4-model/level-3-components/web-client.puml`: Arquitectura interna del cliente web (React)
  * `c4-model/level-3-components/android-app.puml`: Clean Architecture de la app Android
  * `c4-model/level-3-components/backend/core.puml`: Componentes core del backend
  * `c4-model/level-3-components/backend/infrastructure.puml`: Componentes de infraestructura del backend
  * `c4-model/level-3-components/backend/integrations.puml`: Integraciones externas del backend
  * `c4-model/level-3-components/ai-microservice.puml`: Componentes del microservicio de IA

* **Infraestructura y Despliegue:**

  * `uml/deployment/deployment-diagram.puml`: Despliegue UML con nodos, artefactos y entornos
  * `uml/deployment/aws-services.puml`: Servicios cloud y flujos de comunicación
  * `uml/deployment/network-topology.puml`: Topología de red (VPC, subredes, seguridad)

* **Integración Continua (CI/CD):**

  * `uml/deployment/cicd-pipeline.puml`: Flujo CI/CD por repositorio con GitHub Actions

* **Modelo de Negocio y Dominio:**

  * `uml/behavior/context/system-context.puml`: Contexto UML con actores y relaciones (alternativa al modelo C4)
  * `uml/behavior/activities/authentication.puml`: Flujo de autenticación
  * `uml/behavior/activities/logout.puml`: Flujo de cierre de sesión
  * `uml/behavior/activities/planning.puml`: Flujo de planificación de viajes
  * `uml/behavior/activities/suggestion.puml`: Flujo de generación de sugerencias
  * `uml/behavior/use-cases.puml`: Casos de uso completos del sistema

* **Datos y Entidades:**

  * `uml/structure/er-diagram.puml`: Modelo entidad-relación con entidades JPA y persistencia en RDS

* **Arquitectura Empresarial:**

  * `uml/enterprise/archimate.puml`: Vista estratégica de arquitectura empresarial y gobernanza

* **Atributos de Calidad (Qify):**

  * `quality-attributes/scenarios.md`: Escenarios de atributos de calidad definidos para el sistema
  * `quality-attributes/quality-attributes.qify`: Diagrama de atributos de calidad (Qify)

### Herramientas de Visualización

* **PlantUML Online:** [https://plantuml.com/online](https://plantuml.com/online)
* **Qify:** [https://github.com/LePeanutButter/qify](https://github.com/LePeanutButter/qify)
* **VS Code Extension:** PlantUML
* **IntelliJ IDEA:** Integración con PlantUML
* **Miro/Draw.io:** Importación de archivos PlantUML

---

### Cambios importantes:

* **Renombramiento de diagramas:** Los nombres de los archivos ahora siguen una convención más clara, consistente y modular para facilitar su localización y gestión.

* **Agrupación lógica:** Se ha hecho una agrupación más explícita de los diagramas según su función y tipo (C4, infraestructura, CI/CD, atributos de calidad, etc.).

* **Atributos de calidad (Qify):** Se han añadido los **escenarios de atributos de calidad** y el **diagrama Qify** que describen los requisitos no funcionales y cómo se manejan dentro del sistema.

## Project Structure

```
architecture/
├── README.md
├── diagrams/
│   ├── c4-model/
│   │   ├── level-1-context.puml
│   │   ├── level-2-containers.puml
│   │   ├── level-3-components/
│   │   │   ├── web-client.puml
│   │   │   ├── android-app.puml
│   │   │   ├── backend/
│   │   │   │   ├── core.puml
│   │   │   │   ├── infrastructure.puml
│   │   │   │   └── integrations.puml
│   │   │   └── ai-microservice.puml
│   │
│   ├── uml/
│   │   ├── deployment/
│   │   │   ├── deployment-diagram.puml
│   │   │   ├── network-topology.puml
│   │   │   ├── aws-services.puml
│   │   │   └── cicd-pipeline.puml
│   │   │
│   │   ├── structure/
│   │   │   ├── component-overview.puml
│   │   │   └── er-diagram.puml
│   │   │
│   │   ├── behavior/
│   │   │   ├── activities/
│   │   │   │   ├── authentication.puml
│   │   │   │   ├── logout.puml
│   │   │   │   ├── planning.puml
│   │   │   │   └── suggestion.puml
│   │   │   └── use-cases.puml
│   │   │
│   │   └── context/
│   │       └── system-context.puml
│   │
│   └── enterprise/
│       └── archimate.puml
├── quality-attributes/
│   ├── scenarios.md
│   ├── quality-attributes.qify
│   └── exports/
```

## Documentation

### Modelos C4 - Arquitectura por Capas

#### Nivel 1 - Contexto del Sistema

* **level-1-context.puml:** Vista general del sistema con actores principales (viajeros, operadores turísticos) y su relación con la plataforma y la nube.

#### Nivel 2 - Contenedores

* **level-2-containers.puml:** Aplicaciones principales del sistema (Web, Android, Backend, IA) y su interacción con servicios cloud.

#### Nivel 3 - Componentes

* **level-3-components/web-client.puml:** Arquitectura interna del cliente web (React)
* **level-3-components/android-app.puml:** Clean Architecture de la app Android
* **level-3-components/backend/core.puml:** Componentes core del backend
* **level-3-components/backend/infrastructure.puml:** Componentes de infraestructura del backend
* **level-3-components/backend/integrations.puml:** Integraciones externas del backend
* **level-3-components/ai-microservice.puml:** Componentes del microservicio de IA

---

### UML - Infraestructura y Despliegue

#### Arquitectura Cloud

* **deployment/deployment-diagram.puml:** Despliegue UML con nodos, artefactos y entornos
* **deployment/aws-services.puml:** Servicios cloud y flujos de comunicación
* **deployment/network-topology.puml:** Topología de red (VPC, subredes, seguridad)

#### Entrega Continua (CI/CD)

* **deployment/cicd-pipeline.puml:** Flujo CI/CD por repositorio (por ejemplo, GitHub Actions)

---

### UML - Estructura del Sistema

* **structure/component-overview.puml:** Vista técnica integrada de todos los componentes
* **structure/er-diagram.puml:** Modelo entidad-relación con entidades y persistencia

---

### UML - Comportamiento

#### Flujos

* **behavior/activities/authentication.puml:** Flujo de autenticación
* **behavior/activities/logout.puml:** Flujo de cierre de sesión
* **behavior/activities/planning.puml:** Flujo de planificación de viajes
* **behavior/activities/suggestion.puml:** Flujo de generación de sugerencias

#### Casos de Uso

* **behavior/use-cases.puml:** Casos de uso completos del sistema

---

### UML - Contexto Alternativo

* **context/system-context.puml:** Contexto UML con actores y relaciones (alternativa al modelo C4)

---

### Arquitectura Empresarial

* **enterprise/archimate.puml:** Vista estratégica de arquitectura empresarial y gobernanza

---

### Atributos de Calidad

* **quality-attributes/scenarios.md:** Escenarios de atributos de calidad
* **quality-attributes/quality-attributes.qify:** Diagrama de atributos de calidad (Qify)

### Estándares Técnicos

#### Tecnologías Representadas

- **Frontend:** React + Vite, Kotlin + Jetpack Compose
- **Backend:** Java 17 + Spring Boot, Python 3.11 + FastAPI
- **Infraestructura:** AWS (EC2, RDS, S3, API Gateway, ALB, SQS, SNS, CloudWatch)
- **CI/CD:** GitHub Actions, Trivy, SonarCloud
- **Bases de Datos:** PostgreSQL, SQLite (desarrollo), Room (Android)

#### Patrones Arquitectónicos

- **Microservicios:** Backend + IA Service desacoplados
- **Clean Architecture:** MVVM en Android, capas en backend
- **Cloud-Native:** Auto Scaling Groups, balanceo de carga
- **Event-Driven:** SNS/SQS para comunicación asíncrona

### Convenciones de Nomenclatura

#### Sistema de Archivos

- **Numeración secuencial:** 01-16 para orden visual
- **Nomenclatura descriptiva:** `tipo-diagrama.plantuml`
- **Consistencia C4:** Prefijos `c4-` para diagramas del modelo

#### Elementos Visuales

- **Colores por capa:** Diferenciación visual entre frontend, backend, infraestructura
- **Iconos estándar:** Símbolos reconocibles para servicios AWS
- **Notación UML:** Sintaxis estándar PlantUML para diagramas técnicos

## Contributors

- Santiago Botero Garcia - [LePeanutButter](https://github.com/LePeanutButter)

---

**Esta colección de diagramas representa la documentación visual completa de la arquitectura del sistema, proporcionando múltiples perspectivas técnicas y de negocio para facilitar la comprensión y comunicación efectiva entre todos los stakeholders del proyecto.**
