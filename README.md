# OverTheAir Docs - Proyecto Integral de **Turismo Digital Inteligente**

[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)

Repositorio central de documentación del proyecto integral de **Turismo Digital Inteligente**, desarrollado a través de múltiples asignaturas académicas. Contiene la investigación, desarrollo y análisis completo de una plataforma de transformación digital para el sector turístico, abordando todos los aspectos técnicos, de negocio, seguridad y financieros necesarios para su implementación.

## Table of Contents

- [Background](#background)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Documentation](#documentation)
- [Contributors](#contributors)

## Background

Este repositorio contiene la documentación completa del proyecto de **Turismo Digital Inteligente**, desarrollado por un equipo multidisciplinario a través de diferentes asignaturas de la Universidad Escuela Colombiana de Ingeniería Julio Garavito:

- **Transformación Digital y Soluciones Empresariales (TDSE)** - Arquitectura empresarial y modelo de negocio
- **Fundamentos de Seguridad de la Información (FDSI)** - Seguridad y DevSecOps
- **Innovación en Software y Tecnología (SWNT)** - Desarrollo técnico y arquitectura
- **Estructuración de Proyectos Financieros (EPRO)** - Viabilidad financiera y modelos de negocio

La documentación representa el trabajo integral del equipo aplicando conocimientos interdisciplinarios para desarrollar una solución completa de turismo digital con impacto empresarial real.

## Usage

### Explorar por Componente del Proyecto

- **[digital-transformation-business-solutions/](./digital-transformation-business-solutions/)** - Estrategia de transformación digital y arquitectura empresarial
- **[infosec-fundamentals/](./infosec-fundamentals/)** - Implementación de seguridad y análisis de vulnerabilidades
- **[tech-software-innovation/](./tech-software-innovation/)** - Desarrollo técnico, arquitectura de software e innovación
- **[project-structuring-finance/](./project-structuring-finance/)** - Análisis financiero, viabilidad y estructuración del proyecto

### Navegación Recomendada para el Proyecto Integral

1. **Paper académico principal**: `digital-transformation-business-solutions/transformacion-digital.tex`
2. **Análisis sistémico**: `systems/` para bucles causales y arquetipos
3. **Visión general del proyecto**: `tech-software-innovation/wiki.md`
4. **Estrategia y negocio**: `digital-transformation-business-solutions/README.md`
5. **Implementación técnica**: `tech-software-innovation/`
6. **Seguridad y DevSecOps**: `infosec-fundamentals/`
7. **Viabilidad financiera**: `project-structuring-finance/`

## Project Structure

```
overtheair-docs/
├── README.md                                          # Este archivo
├── digital-transformation-business-solutions/         # Estrategia y negocio
│   ├── README.md                                      # Visión de transformación digital
│   ├── transformacion-digital.tex                     # Paper académico principal (70+ páginas)
│   ├── figures/                                       # 38 diagramas técnicos integrados
│   │   ├── c4-model.level-*.pdf                      # Diagramas C4 (contexto, contenedores, componentes)
│   │   ├── uml.*.pdf                                 # Diagramas UML (casos de uso, despliegue, componentes)
│   │   ├── enterprise.archimate.pdf                  # Arquitectura empresarial
│   │   ├── quality-attributes.SmarTrip_*.pdf         # 13 atributos de calidad
│   │   └── systems.*.pdf                             # Análisis sistémico (bucles causales)
│   └── img/                                           # Imágenes legacy
├── infosec-fundamentals/                              # Seguridad
│   ├── README.md                                      # Fundamentos de seguridad implementados
│   ├── paper-escaneo-de-imagenes-de-contenedores.tex   # Análisis de vulnerabilidades CI/CD
│   └── presentacion-escaneo-de-imagenes-de-contenedores.pdf
├── tech-software-innovation/                          # Innovación y desarrollo técnico
│   ├── README.md                                      # Documentación técnica del proyecto
│   ├── wiki.md                                        # Arquitectura completa y diseño
│   ├── requerimientos-agiles.md                       # Especificaciones y user stories
│   └── checklist-de-calidad.md                        # Estándares de calidad aplicados
├── project-structuring-finance/                      # Viabilidad
│   ├── README.md                                      # Análisis financiero del proyecto
│   └── [documentos financieros]                       # Modelos y proyecciones económicas
└── systems/                                           # Análisis de pensamiento sistémico
    ├── README.md                                      # Fundamentos del análisis sistémico
    ├── cld-analysis.md                                # Análisis de bucles causales
    ├── systemic-analysis.md                           # Arquetipos y puntos de apalancamiento
    ├── atoms/                                          # Diagramas de bucles individuales
    └── maps/                                           # Modelo sistémico integrado
```

## Documentation

### Componentes del Proyecto Integral de Turismo Digital

#### Estrategia de Transformación Digital (TDSE)

- **Paper académico completo** de 70+ páginas con análisis integral de transformación digital
- **38 diagramas técnicos** integrados (C4 Model, UML, AWS, atributos de calidad, análisis sistémico)
- **Análisis sistémico innovador** con 5 bucles causales, 4 arquetipos y puntos de apalancamiento
- **Arquitectura empresarial cloud-native** verificable en AWS Academy con código reproducible
- **Inteligencia Artificial integrada** para matching social colaborativo y recomendaciones híbridas
- **Modelo de negocio digital** con monetización diversificada y efectos de red

#### Seguridad Informática y DevSecOps (FDSI)

- **Análisis de vulnerabilidades** en pipelines CI/CD del proyecto
- **Implementación de controles** de seguridad automatizados con GitHub Actions
- **Escaneo de imágenes** de contenedores con Trivy, Grype y CodeQL
- **Mejores prácticas** de seguridad aplicadas a la arquitectura del proyecto

#### Desarrollo Técnico e Innovación (SWNT)

- **Arquitectura completa** con microservicios (Spring Boot, FastAPI, React, Kotlin)
- **Infraestructura AWS** implementada (EC2, RDS, S3, API Gateway, SQS/SNS)
- **Inteligencia Artificial** para matching social y recomendaciones
- **Integración continua** y despliegue automatizado del proyecto

#### Viabilidad Financiera y Estructuración (EPRO)

- **Modelo de negocio** sostenible para la plataforma de turismo
- **Análisis de viabilidad** financiera y económica del proyecto
- **Estrategias de monetización** y captura de valor múltiple
- **Planificación estratégica** para escalado del negocio digital

#### Análisis de Pensamiento Sistémico

- **5 bucles causales fundamentales** que gobiernan el comportamiento del sistema turístico digital
- **4 arquetipos sistémicos identificados** (Límites del Crecimiento, Desplazamiento de la Carga, Erosión de Metas, Éxito a los Exitosos)
- **Puntos de apalancamiento estratégicos** para intervenciones de alto impacto
- **Modelo sistémico integrado** con interacciones complejas entre componentes
- **Recomendaciones priorizadas** para transformación digital sostenible

### Metodología de Trabajo

La documentación sigue una metodología estandarizada:

- **Investigación teórica**: Análisis de estado del arte y mejores prácticas
- **Desarrollo práctico**: Implementación de prototipos y soluciones
- **Validación empírica**: Pruebas y análisis de resultados
- **Documentación formal**: Papers técnicos y artículos académicos
- **Presentación ejecutiva**: Resúmenes y materiales de divulgación

## Contributors

Todos los miembros contribuyeron al desarrollo completo del proyecto de turismo digital:

- **Andrés Felipe Calderón Ramírez** - [AndresFelipeCalderonRamirez](https://github.com/AndresFelipeCalderonRamirez)
- **Daniel Esteban Rodríguez Suarez** - [ders14028-bit](https://github.com/ders14028-bit)
- **Juan Pablo Salamanca Mojica** - [juan-pablo-salamanca-mojica-017855382](https://www.linkedin.com/in/juan-pablo-salamanca-mojica-017855382/)
- **Juana Lozano Chaves** - [juanalch](https://github.com/juanalch)
- **Laura Natalia Perilla Quintero** - [Lanapequin](https://github.com/Lanapequin)
- **Laura Alejandra Venegas Piraban** - [LauraVenegas6](https://github.com/LauraVenegas6)
- **Ricardo Andres Ayala Garzon** - [lRicardol](https://github.com/lRicardol)
- **Santiago Amaya Zapata** - [SantiagoAmaya21](https://github.com/SantiagoAmaya21)
- **Santiago Botero Garcia** - [LePeanutButter](https://github.com/LePeanutButter)
- **Sofia Velandia Cifuentes** - [sofía-velandia-cifuentes-4b4aa51a4](https://www.linkedin.com/in/sof%C3%ADa-velandia-cifuentes-4b4aa51a4/)

---

## License

Este proyecto está licenciado bajo la Licencia Pública General GNU v3.0. Consulta el archivo [LICENSE](LICENSE) para más detalles.

### Resumen de la licencia

- **Uso comercial**: Sí
- **Modificación**: Sí
- **Distribución**: Sí
- **Uso privado**: Sí
- **Responsabilidad legal**: No
- **Garantía**: No

### Derechos de autor

© 2026 OverTheAir. Todos los derechos reservados.

---

**Esta documentación representa el desarrollo integral de un proyecto único de turismo digital inteligente, donde cada asignatura aportó conocimientos especializados para construir una solución completa y viable. El equipo colaborativo aplicó un enfoque interdisciplinario para crear una plataforma transformadora con impacto real en el sector turístico colombiano.**
