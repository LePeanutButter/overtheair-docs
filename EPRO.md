# OverTheAir - Montaje de una empresa de reservas con planificación de viaje a través de una aplicación en Colombia

[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
[![LaTeX](https://img.shields.io/badge/LaTeX-2024-blue.svg)](https://www.latex-project.org/)

El proyecto corresponde a la asignatura _Estructuración de Proyectos: Formulación y Evaluación Financiera (EPRO)_ de la Universidad Escuela Colombiana de Ingeniería Julio Garavito.

## Table of Contents

- [OverTheAir](#overtheair---montaje-de-una-empresa-de-reservas-con-planificación-de-viaje-a-través-de-una-aplicación-en-colombia)
	- [Table of Contents](#table-of-contents)
	- [Background](#background)
	- [Install](#install)
	- [Usage](#usage)
		- [Compilación de Documentos](#compilación-de-documentos)
		- [Estructura del Proyecto](#estructura-del-proyecto)
	- [Documentos Generados](#documentos-generados)
	- [Características Técnicas](#características-técnicas)
	- [Contributors](#contributors)

## Background

Este proyecto corresponde al desarrollo de la asignatura y se basa en **"Montaje de una empresa de reservas con planificación de viaje a través de una aplicación en Colombia"**. El proyecto ha sido completamente reestructurado para cumplir con los estándares académicos de la Universidad Escuela Colombiana de Ingeniería Julio Garavito.

### Objetivo del Proyecto

Desarrollar una aplicación móvil única en el mercado colombiano que integre:
- Sistema de reservas turísticas
- Planificación algorítmica de viajes
- Red social de viajeros
- Conexión directa con prestadores de servicios locales

### Mejoras Implementadas

- **Reorganización de imágenes**: Todas las imágenes optimizadas en directorio `img/`
- **Corrección de tablas**: Formato profesional sin errores de compilación
- **Optimización tipográfica**: Mejoras en legibilidad y formato académico
- **Estructura consistente**: Formato unificado para todos los documentos
- **Compilación sin errores**: Todos los documentos generan PDF correctamente

## Install

### Prerrequisitos

- **MiKTeX** o distribución LaTeX completa
- **Windows** (sistema operativo principal)
- **Editor de texto**: VS Code, TeXstudio, o similar

### Instalación de Dependencias LaTeX

```bash
# Instalar paquetes necesarios (en MiKTeX Package Manager)
# - geometry
# - fancyhdr  
# - titlesec
# - microtype
# - booktabs
# - enumitem
# - hyperref
# - tikz
# - adjustbox
# - array
# - multirow
# - tabularx
# - longtable
```

## Usage

### Compilación de Documentos

Para compilar cada documento individualmente:

```bash
# Compilar documento de planteamiento del proyecto
pdflatex -interaction=nonstopmode planteamiento-proyecto.tex

# Compilar estudio técnico
pdflatex -interaction=nonstopmode estudio-tecnico.tex

# Compilar estudio de mercados
pdflatex -interaction=nonstopmode estudio-mercado.tex

# Compilar análisis DOFA
pdflatex -interaction=nonstopmode analisis-dofa.tex
```

Para compilar todos los documentos secuencialmente:

```bash
for file in *.tex; do
    pdflatex -interaction=nonstopmode "$file"
done
```

### Estructura del Proyecto

```
project-structuring-finance/
├── README.md                    # Este archivo
├── img/                         # Directorio de imágenes
├── planteamiento-proyecto.tex    # Documento principal del proyecto
├── estudio-tecnico.tex          # Análisis técnico y tecnológico
├── estudio-mercado.tex          # Estudio de mercado y competitividad
└── analisis-dofa.tex            # Matriz DOFA y análisis estratégico
```

## Documentos Generados

### 1. Planteamiento del Proyecto
- **Archivo**: `planteamiento-proyecto.pdf`
- **Contenido**: Visión general, objetivos, alcance, stakeholders, cronograma y presupuesto
- **Páginas**: ~13 páginas
- **Imágenes**: 4 imágenes estratégicas incluidas

### 2. Estudio Técnico
- **Archivo**: `estudio-tecnico.pdf`
- **Contenido**: Análisis de ingeniería, tecnología, infraestructura y viabilidad técnica
- **Páginas**: ~15 páginas
- **Tablas**: Matrices de decisión y análisis técnico

### 3. Estudio de Mercados
- **Archivo**: `estudio-mercado.pdf`
- **Contenido**: Análisis de mercado, competencia, demanda y estrategias comerciales
- **Páginas**: ~10 páginas
- **Gráficos**: Análisis de tendencias del mercado

### 4. Análisis DOFA
- **Archivo**: `analisis-dofa.pdf`
- **Contenido**: Matriz DOFA completa con estrategias FO, FA, DO, DA
- **Páginas**: ~7 páginas
- **Matriz**: Formato optimizado con todas las estrategias visibles

## Características Técnicas

### Formato Académico
- **Tipografía**: Latin Modern para máxima legibilidad
- **Márgenes**: 2.5cm estándar académico
- **Interlineado**: 1.3 para mejor lectura
- **Encabezados**: Formato consistente con información institucional

### Optimizaciones Realizadas
- **Tablas**: Convertidas a formato `tabular` con anchos fijos
- **Imágenes**: Rutas relativas y optimización de tamaño
- **Símbolos matemáticos**: Uso correcto de modo matemático
- **Hiperenlaces**: Configurados para navegación en PDF
- **Metadatos**: Información completa del documento

### Calidad de Compilación
- **Sin errores**: Todos los documentos compilan sin warnings críticos
- **PDF optimizados**: Tamaños de archivo balanceados
- **Navegación**: Tabla de contenidos automática
- **Referencias**: Enlaces cruzados funcionales

## Contributors

- **Santiago Botero García** - [LePeanutButter](https://github.com/LePeanutButter)
- **Juana Lozano Chaves** - [juanalch](https://github.com/juanalch)
- **Juan Pablo Salamanca Mojica** - [juan-pablo-salamanca-mojica-017855382](https://www.linkedin.com/in/juan-pablo-salamanca-mojica-017855382/)
- **Sofia Velandia Cifuentes** - [sofía-velandia-cifuentes-4b4aa51a4](https://www.linkedin.com/in/sof%C3%ADa-velandia-cifuentes-4b4aa51a4/)
- **Laura Alejandra Venegas Piraban** - [LauraVenegas6](https://github.com/LauraVenegas6)

---

Proyecto desarrollado por **OverTheAir**
