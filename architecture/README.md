# Documentación Arquitectónica

[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
[![Architecture Documentation](https://img.shields.io/badge/Architecture%20Documentation-2024-blue.svg)](https://github.com/RichardLitt/standard-readme)

Colección completa de diagramas arquitectónicos del sistema de turismo digital en formato PlantUML, incluyendo modelos C4, diagramas de despliegue AWS, integración continua y flujos de negocio.

## Table of Contents

- [Background](#background)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Documentation](#documentation)
- [Contributors](#contributors)

## Background

Este directorio contiene la documentación visual completa de la arquitectura del sistema de turismo digital inteligente. Los diagramas están organizados siguiendo el modelo C4 para proporcionar diferentes niveles de abstracción, desde el contexto de negocio hasta los detalles técnicos de implementación.

La colección incluye 16 diagramas especializados que cubren todos los aspectos arquitectónicos del sistema: desde la vista general del negocio hasta los detalles específicos de infraestructura AWS, pipelines de CI/CD y modelos de datos.

## Usage

### Exploración por Tipo de Diagrama

- **Diagramas C4 (Niveles 1-3):** `1-c4-context-diagram.plantuml`, `2-c4-container-diagram.plantuml`, `3-6-*component-diagram.plantuml`
- **Infraestructura AWS:** `7-deployment-diagram.plantuml`, `10-aws-diagram.plantuml`, `12-network-topology.plantuml`
- **Integración y Despliegue:** `8-component-diagram.plantuml`, `9-cicd-pipeline-diagram.plantuml`
- **Modelo de Negocio:** `11-context-diagram.plantuml`, `13-activity-diagram.plantuml`, `15-use-cases-diagram.plantuml`
- **Datos y Dominio:** `14-er-diagram.plantuml`
- **Arquitectura Empresarial:** `16-enterprise-architecture-and-gobernanze-diagram.plantuml`

### Herramientas de Visualización

- **PlantUML Online:** https://plantuml.com/online
- **VS Code Extension:** PlantUML
- **IntelliJ IDEA:** PlantUML integration
- **Miro/Draw.io:** Importación de PlantUML

## Project Structure

```
architecture-diagrams/
├── README.md                                          # Este archivo
├── 1-c4-context-diagram.plantuml                      # Contexto del sistema (C4 Nivel 1)
├── 2-c4-container-diagram.plantuml                    # Contenedores (C4 Nivel 2)
├── 3-c4-web-client-component-diagram.plantuml         # Componentes cliente web
├── 4-c4-android-app-component-diagram.plantuml       # Componentes app Android
├── 5-c4-backend-api-component-diagram.plantuml        # Componentes backend API
├── 6-c4-ai-microservice-component-diagram.plantuml    # Componentes microservicio IA
├── 7-deployment-diagram.plantuml                      # Diagrama de despliegue UML
├── 8-component-diagram.plantuml                       # Vista técnica integrada
├── 9-cicd-pipeline-diagram.plantuml                   # Pipelines CI/CD
├── 10-aws-diagram.plantuml                            # Servicios y comunicación AWS
├── 11-context-diagram.plantuml                       # Contexto UML alternativo
├── 12-network-topology.plantuml                       # Topología de red VPC
├── 13-activity-diagram.plantuml                       # Flujos principales
├── 14-er-diagram.plantuml                             # Modelo entidad-relación
├── 15-use-cases-diagram.plantuml                      # Casos de uso del sistema
└── 16-enterprise-architecture-and-gobernanze-diagram.plantuml # Arquitectura empresarial
```

## Documentation

### Modelos C4 - Arquitectura por Capas

#### Nivel 1 - Contexto del Sistema

- **1-c4-context-diagram.plantuml:** Vista general del sistema con actores principales (Viajeros, Operadores turísticos) y su relación con la plataforma y AWS Cloud.

#### Nivel 2 - Contenedores

- **2-c4-container-diagram.plantuml:** Aplicaciones principales del sistema (Web, Android, Backend, IA) y su interacción con servicios cloud.

#### Nivel 3 - Componentes

- **3-c4-web-client-component-diagram.plantuml:** Arquitectura interna del cliente React
- **4-c4-android-app-component-diagram.plantuml:** Clean Architecture de la app Android
- **5-c4-backend-api-component-diagram.plantuml:** Módulos del backend Spring Boot
- **6-c4-ai-microservice-component-diagram.plantuml:** Componentes del servicio FastAPI

### Infraestructura y Despliegue

#### Arquitectura Cloud

- **7-deployment-diagram.plantuml:** Despliegue UML en AWS Academy con nodos y artefactos
- **10-aws-diagram.plantuml:** Servicios AWS y flujos de comunicación
- **12-network-topology.plantuml:** Topología detallada de VPC, subredes y seguridad

#### Integración Continua

- **8-component-diagram.plantuml:** Vista técnica integrada de todos los componentes
- **9-cicd-pipeline-diagram.plantuml:** Flujo CI/CD por repositorio con GitHub Actions

### Modelo de Negocio y Dominio

#### Flujos y Casos de Uso

- **11-context-diagram.plantuml:** Contexto UML con actores y casos de uso
- **13-activity-diagram.plantuml:** Flujo principal de invocación API autenticada
- **15-use-cases-diagram.plantuml:** Casos de uso completos del sistema

#### Datos y Entidades

- **14-er-diagram.plantuml:** Modelo entidad-relación con entidades JPA y despliegue RDS

#### Arquitectura Empresarial

- **16-enterprise-architecture-and-gobernanze-diagram.plantuml:** Vista estratégica de arquitectura y gobernanza

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
