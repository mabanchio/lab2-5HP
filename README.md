# Laboratorio 2: NumPy y Pandas con Datos de Argentina

## Universidad de la Ciudad de Buenos Aires
**Materia:** ASIG00202 - Programación Avanzada para Ciencia de Datos - 2/2025  
**Profesor:** Juan Carlos Cifuentes Duran

## Integrantes del Equipo
- MATIAS ALEJANDRO BANCHIO
- PABLO GABRIEL CIOCIANO  
- PAULA GISELA COCHIMANO
- ANTONIO LUIS EMILIO MARTINEZ
- ENRIQUE IGNACIO VAZQUEZ

## Descripción del Proyecto

Este proyecto implementa un laboratorio práctico de análisis de datos utilizando las librerías **NumPy** y **Pandas** de Python. El laboratorio trabaja con un dataset de ciudades argentinas para demostrar operaciones fundamentales de ciencia de datos.

## Dataset Utilizado

El laboratorio utiliza un dataset con información de 5 ciudades principales de Argentina:

| Ciudad | Provincia | Población (miles) | Año Fundación |
|--------|-----------|-------------------|---------------|
| Buenos Aires | CABA | 3,070 | 1580 |
| Córdoba | Córdoba | 1,390 | 1573 |
| Rosario | Santa Fe | 1,170 | 1689 |
| Mendoza | Mendoza | 937 | 1561 |
| La Plata | Buenos Aires | 740 | 1882 |

## Funcionalidades Implementadas

### Parte 1: NumPy
- ✅ Creación de arrays con datos de población
- ✅ Cálculo de estadísticas descriptivas (media, mediana, desviación estándar)
- ✅ Análisis de años de fundación
- ✅ Identificación de ciudades más antigua y más reciente

### Parte 2: Pandas
- ✅ Manipulación de DataFrames
- ✅ Cálculo de población total
- ✅ Ordenamiento de datos por población
- ✅ Filtrado de datos (ciudades fundadas antes de 1600)
- ✅ Exportación de resultados a CSV

## Estructura del Proyecto

```
laboratorio-2/
│
├── README.md                           # Este archivo
├── INSTRUCTIVO_INSTALACION.md          # Guía de instalación
├── DOCUMENTO_EJECUTIVO.md              # Resumen ejecutivo
├── laboratorio_numpy_pandas.ipynb      # Notebook principal
└── ciudades_arg.csv                    # Archivo generado por el análisis
```

## Resultados Principales

- **Población total analizada:** 7,307 miles de habitantes
- **Ciudad más poblada:** Buenos Aires (3,070 miles)
- **Ciudad más antigua:** Mendoza (fundada en 1561)
- **Ciudad más reciente:** La Plata (fundada en 1882)
- **Promedio poblacional:** 1,461.4 miles de habitantes

## Tecnologías Utilizadas

- **Python 3.11.2**
- **NumPy:** Para operaciones matemáticas y estadísticas
- **Pandas:** Para manipulación y análisis de datos
- **Jupyter Notebook:** Para desarrollo interactivo

## Cómo Ejecutar

1. Sigue las instrucciones del `INSTRUCTIVO_INSTALACION.md`
2. Abre el notebook `laboratorio_numpy_pandas.ipynb`
3. Ejecuta todas las celdas secuencialmente
4. Los resultados se mostrarán inline y se generará `ciudades_arg.csv`

## Notas Técnicas

- El notebook incluye visualización de datos en formato HTML
- Todos los cálculos están documentados paso a paso
- El código es reproducible y está optimizado para aprendizaje

## Contacto

Para consultas sobre este laboratorio, contactar a cualquiera de los integrantes del equipo a través de los canales oficiales de la Universidad de la Ciudad de Buenos Aires.