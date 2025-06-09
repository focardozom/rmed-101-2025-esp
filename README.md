# R Medicine 101 2025 - Español

**Taller introductorio de R para Bioestadística y Ciencia de Datos en el ámbito de la salud**

## 📖 Descripción

Este taller está diseñado para introducir a profesionales de la salud, investigadores y estudiantes al uso de R para el análisis de datos biomédicos y epidemiológicos. A través de ejemplos prácticos y datos reales del sector salud colombiano, los participantes aprenderán los fundamentos de R y su aplicación en bioestadística.

## 🎯 Objetivos

- Introducir los conceptos fundamentales de programación en R
- Enseñar el manejo y manipulación de datos en el contexto de salud pública
- Aplicar técnicas de análisis exploratorio de datos biomédicos
- Desarrollar habilidades para crear visualizaciones informativas de datos de salud
- Fomentar buenas prácticas en la gestión y análisis reproducible de datos

## 📚 Contenido del Taller

### Módulo 1: Introducción a R
- **Archivo**: `scripts/R-MED-INTRO-A-R.qmd`
- **Contenido**:
  - Tipos de datos y variables en R
  - Objetos fundamentales: vectores, matrices, data frames y listas
  - Ejercicios prácticos con ejemplos biomédicos

### Módulo 2: Análisis de Datos de Migración y Salud
- **Archivo**: `scripts/R-MED-MIGRACION.qmd`
- **Contenido**:
  - Análisis de atenciones en salud a población migrante
  - Limpieza y organización de datos reales
  - Visualización de tendencias temporales (2017-2021)
  - Caso de estudio: Bucaramanga, Colombia

## 🗂️ Estructura del Proyecto

```
rmed-101-2025-esp/
├── README.md                    # Este archivo
├── rmed-101-2025-esp.Rproj     # Proyecto de RStudio
├── scripts/                     # Scripts del taller
│   ├── R-MED-INTRO-A-R.qmd     # Introducción a R
│   ├── R-MED-MIGRACION.qmd     # Análisis de datos de migración
│   ├── prompts.qmd             # Ejercicios y prompts
│   └── style.css               # Estilos para documentos
├── data/                        # Datos para el análisis
│   └── atenciones_migrantes.parquet
└── img/                         # Imágenes generadas
    └── atenciones_por_servicio.png
```

## 🛠️ Requisitos Previos

### Software Necesario
- **R** (versión 4.0 o superior) - [Descargar aquí](https://cran.r-project.org/)
- **RStudio** - [Descargar aquí](https://posit.co/download/rstudio-desktop/)

### Conocimientos
- Conocimientos básicos de estadística descriptiva
- Familiaridad con conceptos de epidemiología (recomendado)
- No se requiere experiencia previa en programación

## 📦 Instalación de Paquetes

Antes de comenzar el taller, instala los siguientes paquetes ejecutando este código en R:

```r
# Instalar paquetes necesarios
install.packages(c(
  "pak",        # Gestión de paquetes
  "here",       # Gestión de rutas de archivos
  "tidyverse",  # Análisis de datos
  "janitor",    # Limpieza de datos
  "readxl",     # Lectura de archivos Excel
  "leaflet"     # Mapas interactivos
))

# Instalar arrow para archivos Parquet
pak::pak("arrow")
```

## 🚀 Cómo Usar Este Material

1. **Clonar o descargar** este repositorio
2. **Abrir** el proyecto en RStudio (`rmed-101-2025-esp.Rproj`)
3. **Instalar** los paquetes necesarios (ver sección anterior)
4. **Seguir** los módulos en orden:
   - Comenzar con `R-MED-INTRO-A-R.qmd`
   - Continuar con `R-MED-MIGRACION.qmd`
5. **Ejecutar** el código chunk por chunk usando `Ctrl+Enter` (Windows) o `Cmd+Enter` (Mac)

## 📊 Datos Utilizados

El taller utiliza datos reales de **atenciones en salud a población migrante** en Bucaramanga, Colombia, obtenidos de:
- **Fuente**: [Datos Abiertos del Gobierno de Colombia](https://www.datos.gov.co/Salud-y-Protecci-n-Social/Atenciones-en-Salud-a-Poblaci-n-Migrante/xbwb-yz9d/about_data)
- **Periodo**: 2014-2022
- **Registros**: >200,000 atenciones
- **Formato**: Parquet (optimizado para análisis de datos grandes)

## 👥 Instructores

- **Francisco Cardozo**
- **Catalina Cañizares**

## 🤝 Contribuciones

Este material está en desarrollo activo. Si encuentras errores o tienes sugerencias de mejora, por favor:
1. Abre un issue en el repositorio
2. Envía un pull request con tus mejoras
3. Contacta a los instructores

## 📄 Licencia

Este material educativo está disponible para uso académico y educativo. Por favor, cita apropiadamente si utilizas este contenido en tus propios proyectos o enseñanza.

## 🏥 Acerca de R Medicine

Este taller forma parte de la iniciativa **R Medicine**, que promueve el uso de R en investigación médica y ciencias de la salud. Para más información, visita [r-medicine.org](https://r-medicine.org/).

---

**¡Esperamos que disfrutes aprendiendo R para aplicaciones biomédicas!** 🩺📊
