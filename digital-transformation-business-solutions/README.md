# Digital Transformation Business Solutions

[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
[![Digital Transformation](https://img.shields.io/badge/Digital%20Transformation-2026-blue.svg)](https://github.com/RichardLitt/standard-readme)
[![LaTeX](https://img.shields.io/badge/LaTeX-Document-green.svg)](https://www.latex-project.org/)
[![Systems Thinking](https://img.shields.io/badge/Systems%20Thinking-Analysis-orange.svg)](https://en.wikipedia.org/wiki/Systems_thinking)

Investigación académica completa sobre transformación digital en el sector turístico, presentada como paper científico con análisis sistémico integral, arquitectura empresarial cloud-native y 38 diagramas técnicos. El trabajo combina rigor académico con implementación práctica mediante IA, sistemas de recomendación y plataformas colaborativas.

El proyecto corresponde a la asignatura _Transformación Digital y Soluciones Empresariales (TDSE)_ de la Universidad Escuela Colombiana de Ingeniería Julio Garavito.

## Table of Contents

- [Background](#background)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Documentation](#documentation)
- [Contributors](#contributors)

## Background

Este repositorio contiene la investigación académica completa sobre transformación digital en el sector turístico, presentada como paper científico integral. El trabajo combina análisis estratégico, arquitectura empresarial cloud-native, inteligencia artificial y pensamiento sistémico para abordar los desafíos fundamentales del turismo digital.

### **Logros Principales**

- **Paper Académico Completo**: Documento LaTeX de 70+ páginas con análisis integral
- **38 Diagramas Técnicos**: C4 Model, UML, AWS, atributos de calidad y análisis sistémico
- **Análisis Sistémico Innovador**: 5 bucles causales, 4 arquetipos sistémicos y puntos de apalancamiento
- **Arquitectura Verificable**: Implementación cloud-native en AWS con código reproducible
- **Inteligencia Artificial Integrada**: Sistemas de recomendación híbridos y matching social colaborativo

El estudio aborda la transformación de experiencias individuales de viaje en ecosistemas colaborativos inteligentes, mediante arquitecturas escalables y análisis de dinámicas complejas del sistema turístico.

## Usage

### **Documento Principal**

**`digital-transformation.tex`** - Paper académico completo con:
- Abstract y resumen en español/inglés
- Marco teórico formal (PEAS, sistemas de recomendación, SARIMA)
- Modelo de negocio digital y propuesta de valor
- Arquitectura empresarial cloud-native (AWS)
- **Análisis sistémico del proceso de transformación digital**
- Atributos de calidad con diagramas detallados
- Metodología data-centric y métricas de evaluación
- 38 figuras integradas con formato optimizado

### **Navegación Recomendada**

1. **Visión General**: Lee el abstract y resumen (líneas 42-67)
2. **Problema y Objetivos**: Secciones 1-2 (líneas 100-140)
3. **Fundamento Teórico**: Sección 3 (líneas 142-188)
4. **Arquitectura**: Secciones 4-6 (líneas 190-460)
5. **Análisis Sistémico**: Sección 7 (líneas 738-960)
6. **Atributos de Calidad**: Sección 8 (líneas 962-1056)

### **Compilación LaTeX**

```bash
# Compilar el documento principal
pdflatex digital-transformation.tex
bibtex digital-transformation
pdflatex digital-transformation.tex
pdflatex digital-transformation.tex
```

## Project Structure

```
digital-transformation-business-solutions/
├── README.md                                           # Este archivo
├── digital-transformation.tex                          # Paper académico principal
├── figures/                                            # 38 diagramas técnicos
│   ├── c4-model.level-*.pdf                            # Diagramas C4 (contexto, contenedores, componentes)
│   ├── uml.*.pdf                                       # Diagramas UML (casos de uso, despliegue, componentes)
│   ├── enterprise.archimate.pdf                        # Arquitectura empresarial
│   ├── quality-attributes.SmarTrip_*.pdf               # 13 atributos de calidad
│   └── systems.*.pdf                                   # Análisis sistémico (bucles causales, modelo integrado)
├── img/                                                # Imágenes legacy (referenciadas en código)
└── ../systems/                                         # Análisis de pensamiento sistémico
    ├── README.md                                       # Fundamentos del análisis sistémico
    ├── cld-analysis.md                                 # Análisis de bucles causales
    ├── systemic-analysis.md                            # Arquetipos y puntos de apalancamiento
    ├── atoms/                                          # Diagramas de bucles individuales
    └── maps/                                           # Modelo sistémico integrado
```

## Documentation

### **Enfoque de la Investigación**

El paper aborda la transformación digital del turismo mediante:

- **Arquitectura Empresarial Cloud-Native**: Diseño verificable en AWS Academy con API Gateway, ALB, EC2, RDS, S3, SNS/SQS
- **Inteligencia Artificial Integrada**: Sistemas de recomendación híbridos, matching social colaborativo y modelos predictivos SARIMA
- **Análisis Sistémico**: Identificación de bucles causales, arquetipos sistémicos y puntos de apalancamiento estratégicos
- **Modelo de Negocio Digital**: Plataforma multisided con monetización diversificada y efectos de red
- **Atributos de Calidad**: 13 escenarios verificables covering disponibilidad, escalabilidad, seguridad y rendimiento

### **Metodología Científica**

- **Formalización Matemática**: Modelos PEAS, ecuaciones de recomendación híbrida y optimización lineal
- **Análisis de Pensamiento Sistémico**: Bucles de retroalimentación, arquetipos y leverage points
- **Diseño Data-Centric**: Dataset estructurado para contexto turístico colombiano
- **Métricas de Evaluación**: RMSE, MAE, Precision@K, Recall@K y análisis de significancia estadística
- **Validación Empírica**: Diseño experimental con validación cruzada y pruebas de hipótesis

### **Contribuciones Principales**

#### **1. Análisis Sistémico Innovador**
- **5 Bucles Causales**: R1 (Soledad), R2 (Fragmentación), R3 (Límites de Datos), B1 (Escalabilidad), R4 (Validación Social)
- **4 Arquetipos Sistémicos**: Límites del Crecimiento, Desplazamiento de la Carga, Erosión de Metas, Éxito a los Exitosos
- **Puntos de Apalancamiento**: Intervenciones estratégicas con máximo impacto sistémico

#### **2. Arquitectura Verificable**
- **Implementación AWS**: Topología completa con scripts de infraestructura reproducible
- **Separación de Responsabilidades**: Backend (Spring Boot), IA (FastAPI), clientes multiplataforma
- **Calidad Integrada**: 13 atributos de calidad con escenarios verificables y diagramas detallados

#### **3. Viaje Social Colaborativo**
- **Matching Multidimensional**: Algoritmos de compatibilidad basados en preferencias y comportamiento
- **Efectos de Red**: Plataforma que genera valor incremental con cada usuario adicional
- **Integración Continua**: Experiencias conectadas desde planificación hasta post-viaje

## Contributors

- Ricardo Andres Ayala Garzon - [lRicardol](https://github.com/lRicardol)
- Santiago Amaya Zapata - [SantiagoAmaya21](https://github.com/SantiagoAmaya21)
- Santiago Botero Garcia - [LePeanutButter](https://github.com/LePeanutButter)
