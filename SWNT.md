# SmarTrip - Tech Software Innovation Documentation

[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
[![LaTeX](https://img.shields.io/badge/LaTeX-2024-blue.svg)](https://www.latex-project.org/)

Documentación técnica y de innovación para SmarTrip, una plataforma social de turismo inteligente que revoluciona la forma en que los viajeros se conectan entre sí y descubren experiencias auténticas mediante Inteligencia Artificial avanzada y matching social. El proyecto corresponde a la asignatura _Innovación Software apoyada en Nuevas Tecnologías (SWNT)_ de la Universidad Escuela Colombiana de Ingeniería Julio Garavito.

## Table of Contents

- [Background](#background)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Documentation](#documentation)
- [Contributing](#contributing)

## Background

SmarTrip es un **ecosistema digital centrado en**:

- **Asistente IA Personalizado**: Companion inteligente que aprende y adapta recomendaciones
- **Conexiones Sociales Inteligentes**: Sistema de matching entre viajeros compatibles
- **Planificación Colaborativa**: Herramientas para crear itinerarios compartidos
- **Descubrimiento Contextual**: Recomendaciones basadas en ubicación, preferencias y comportamiento

Este repositorio contiene la documentación técnica del proyecto, incluyendo especificaciones ágiles, checklists de calidad, y el modelo de negocio.

## Usage

### Explorar la Documentación

- **wiki.md**: Documentación completa del proyecto con arquitectura, características y visión general
- **requerimientos-agiles.md**: Especificaciones técnicas detalladas con user stories y criterios de aceptación
- **checklist-de-calidad.md**: Estándares de calidad y procesos de desarrollo
- **business-model-canvas.pdf**: Modelo de negocio estratégico

### Navegación Recomendada

1. **Para entender el proyecto**: Comienza con `wiki.md`
2. **Para desarrollo técnico**: Revisa `requerimientos-agiles.md`
3. **Para estándares de calidad**: Consulta `checklist-de-calidad.md`
4. **Para perspectiva de negocio**: Analiza el Business Model Canvas

## Project Structure

```
tech-software-innovation/
├── README.md                    # Este archivo
├── wiki.md                      # Documentación completa del proyecto
├── requerimientos-agiles.md      # Especificaciones técnicas y user stories
├── checklist-de-calidad.md      # Estándares de calidad y procesos
└── business-model-canvas.tex     # Fuente LaTeX del Business Model Canvas
```

## Documentation

### Arquitectura Técnica

El proyecto utiliza un ecosistema multi-plataforma:

| Componente | Tecnología | Propósito |
| ----------- | ---------- | --------- |
| **Aplicación Móvil** | Kotlin + Jetpack Compose | Experiencia nativa Android con Clean Architecture |
| **Backend Core** | Java 17 + Spring Boot 3.2 | API RESTful con JWT, PostgreSQL y microservicios |
| **Plataforma Web** | React 18 + Vite | Dashboard de gestión y planificación detallada |
| **Servicio IA** | Python + FastAPI | Motor de recomendaciones y matching social |
| **Infraestructura** | AWS Academy | Cloud computing con auto-scaling y monitoring |

### Metodología de Desarrollo

- **Sprints Ágiles**: Desarrollo iterativo con entregas incrementales
- **User Stories**: Especificaciones centradas en el usuario
- **Clean Architecture**: Separación de responsabilidades y mantenibilidad
- **CI/CD**: Integración continua con GitHub Actions

### Características Principales

- **Matching Social Inteligente**: Algoritmos de IA que conectan viajeros con alta compatibilidad
- **Recomendaciones Contextuales**: Sugiere experiencias basadas en ubicación, tiempo y preferencias grupales
- **Planificación Colaborativa**: Herramientas para co-crear itinerarios con conexiones compatibles
- **Social Intelligence**: Análisis de patrones de comportamiento para optimizar conexiones
- **Aprendizaje Adaptativo**: Sistema que mejora con cada interacción y conexión exitosa

## Contributors

- Andrés Felipe Calderón Ramírez - [AndresFelipeCalderonRamirez](https://github.com/AndresFelipeCalderonRamirez)
- Laura Natalia Perilla Quintero - [Lanapequin](https://github.com/Lanapequin)
- Ricardo Andres Ayala Garzon - [lRicardol](https://github.com/lRicardol)
- Santiago Amaya Zapata - [SantiagoAmaya21](https://github.com/SantiagoAmaya21)
- Santiago Botero Garcia - [LePeanutButter](https://github.com/LePeanutButter)

---

Proyecto desarrollado por **Voyager Team**
