# Documento Ejecutivo - Laboratorio Nro. 2
## Análisis de Datos con NumPy y Pandas

---

**Universidad de la Ciudad de Buenos Aires**  
**Materia:** ASIG00202 - Programación Avanzada para Ciencia de Datos - 2/2025  
**Profesor:** Juan Carlos Cifuentes Duran  
**Fecha de Entrega:** Septiembre 2025

---

## Equipo de Trabajo

| Integrante | Rol en el Proyecto |
|------------|-------------------|
| MATIAS ALEJANDRO BANCHIO | Análisis NumPy y Documentación |
| PABLO GABRIEL CIOCIANO | Implementación Pandas y Testing |
| PAULA GISELA COCHIMANO | Validación de Datos y Control de Calidad |
| ANTONIO LUIS EMILIO MARTINEZ | Estructura del Proyecto y README |
| ENRIQUE IGNACIO VAZQUEZ | Coordinación General y Documento Ejecutivo |

---

## Resumen Ejecutivo

El presente laboratorio implementa un análisis integral de datos demográficos argentinos utilizando las librerías fundamentales de ciencia de datos en Python: **NumPy** y **Pandas**. El proyecto demuestra competencias en manipulación de arrays multidimensionales, cálculos estadísticos, análisis exploratorio de datos y exportación de resultados.

### Objetivos Cumplidos

✅ **Objetivo Principal:** Demostrar dominio técnico en NumPy y Pandas  
✅ **Objetivo Secundario:** Aplicar conceptos teóricos a datos reales argentinos  
✅ **Objetivo Metodológico:** Implementar flujo completo de análisis de datos  

---

## Metodología Aplicada

### Dataset de Trabajo
Se utilizó un conjunto de datos estructurado con información de 5 ciudades principales de Argentina:

| Variable | Tipo | Descripción |
|----------|------|-------------|
| Ciudad | String | Nombre de la ciudad |
| Provincia | String | Provincia de ubicación |
| Poblacion_miles | Integer | Población en miles de habitantes |
| Año_fundacion | Integer | Año de fundación histórica |

### Tecnologías Implementadas

**NumPy v1.24+**
- Arrays unidimensionales para cálculos vectorizados
- Funciones estadísticas: `mean()`, `median()`, `std()`
- Búsqueda de índices: `argmin()`, `argmax()`

**Pandas v2.0+**
- DataFrames para manipulación estructurada
- Operaciones de agregación: `sum()`
- Ordenamiento y filtrado de datos
- Exportación a formatos estándar (CSV)

---

## Resultados Obtenidos

### Análisis Estadístico (NumPy)

| Métrica | Valor | Unidad |
|---------|-------|--------|
| **Población Media** | 1,461.4 | miles de hab. |
| **Población Mediana** | 1,170.0 | miles de hab. |
| **Desviación Estándar** | 833.4 | miles de hab. |

### Análisis Histórico

| Categoría | Ciudad | Año |
|-----------|--------|-----|
| **Más Antigua** | Mendoza | 1561 |
| **Más Reciente** | La Plata | 1882 |
| **Diferencia Temporal** | - | 321 años |

### Análisis Demográfico (Pandas)

**Población Total Analizada:** 7,307 miles de habitantes

**Ranking Poblacional:**
1. Buenos Aires: 3,070 miles (42.0% del total)
2. Córdoba: 1,390 miles (19.0% del total)
3. Rosario: 1,170 miles (16.0% del total)
4. Mendoza: 937 miles (12.8% del total)
5. La Plata: 740 miles (10.1% del total)

**Análisis Temporal:**
- Ciudades fundadas antes de 1600: 3 (60% del dataset)
- Concentración fundacional: Siglo XVI (época colonial)

---

## Implementación Técnica

### Estructura del Código

```python
# Ejemplo de implementación NumPy
poblaciones = np.array(df["Poblacion_miles"])
media = np.mean(poblaciones)
mediana = np.median(poblaciones)
desv = np.std(poblaciones)

# Ejemplo de implementación Pandas
poblacion_total = df["Poblacion_miles"].sum()
df_ordenado = df.sort_values(by="Poblacion_miles", ascending=False)
ciudades_antiguas = df[df["Año_fundacion"] < 1600]
```

### Validaciones Implementadas

✅ **Integridad de Datos:** Verificación de tipos y valores nulos  
✅ **Consistencia Temporal:** Validación de años de fundación  
✅ **Precisión Numérica:** Control de decimales en cálculos estadísticos  
✅ **Formato de Salida:** Exportación correcta a CSV con encoding UTF-8  

---

## Análisis Crítico y Observaciones

### Fortalezas del Proyecto

1. **Completitud Metodológica:** Se cubrieron todos los aspectos solicitados del laboratorio
2. **Precisión Técnica:** Implementación correcta de funciones NumPy y Pandas
3. **Documentación Integral:** Código autodocumentado con outputs visibles
4. **Reproducibilidad:** Entorno controlado y dependencias especificadas

### Limitaciones Identificadas

1. **Tamaño del Dataset:** Muestra pequeña (5 ciudades) limita análisis estadístico robusto
2. **Encoding de Caracteres:** Problemas menores de codificación en nombres (Ã³ → ó)
3. **Validación Externa:** No se contrastaron datos con fuentes oficiales (INDEC)

### Recomendaciones para Mejoras Futuras

- Expandir dataset con más ciudades argentinas
- Implementar visualizaciones con matplotlib/seaborn
- Agregar análisis de correlación entre variables
- Incluir datos temporales (series de tiempo poblacional)

---

## Conclusiones Académicas

### Competencias Demostradas

**Técnicas:**
- Dominio de operaciones NumPy para cálculos científicos
- Competencia en manipulación de DataFrames con Pandas
- Implementación de flujos ETL básicos (Extract-Transform-Load)

**Metodológicas:**
- Aplicación de pensamiento analítico a datos reales
- Documentación profesional de procesos de análisis
- Trabajo colaborativo en equipo técnico

### Impacto del Aprendizaje

El laboratorio consolidó conocimientos fundamentales en ciencia de datos, preparando al equipo para análisis más complejos en proyectos futuros. La experiencia práctica con datos argentinos añadió contexto local relevante al aprendizaje técnico.

### Alineación Curricular

El proyecto cumple plenamente con los objetivos de la materia **ASIG00202**, demostrando:
- Programación avanzada en Python
- Manejo de librerías especializadas en ciencia de datos
- Análisis exploratorio de datos estructurados
- Documentación técnica profesional

---

## Entregables del Proyecto

| Archivo | Descripción | Estado |
|---------|-------------|--------|
| `laboratorio_numpy_pandas.ipynb` | Notebook principal con análisis completo | ✅ Completado |
| `ciudades_arg.csv` | Dataset exportado post-análisis | ✅ Generado |
| `README.md` | Documentación del proyecto | ✅ Completado |
| `INSTRUCTIVO_INSTALACION.md` | Guía técnica de setup | ✅ Completado |
| `DOCUMENTO_EJECUTIVO.md` | Este documento de presentación | ✅ Completado |

---

## Declaración de Autoría

El equipo declara que este laboratorio fue desarrollado completamente por los integrantes listados, utilizando únicamente recursos académicos autorizados y herramientas de software libre. Todo el código es original y está disponible para revisión académica.

---

**Firma Digital del Equipo**  
*Laboratorio 2 - Programación Avanzada para Ciencia de Datos*  
*Universidad de la Ciudad de Buenos Aires - Septiembre 2025*