# Healthcare Tariff Analysis - Data Cleaning & Exploratory Data Analysis

**Autor:** Juan Manuel Erazo  
**Fecha:** Enero 2026  
**Objetivo:** Análisis exploratorio y limpieza de nomenclador de procedimientos médicos

## 📊 Descripción

Este proyecto analiza un nomenclador de procedimientos médicos de una clínica peruana con **3,878 registros**. Incluye:
- Limpieza de datos (registros vacíos, valores faltantes)
- Análisis exploratorio (distribución de procedimientos, grupos contables)
- Identificación de patrones y anomalías en la data

## 📈 Hallazgos Clave

| Métrica | Valor |
|---------|-------|
| **Registros totales** | 3,878 |
| **Registros limpios después de EDA** | 3,876 |
| **Grupos contables identificados** | 7 categorías |
| **Datos faltantes detectados** | 100% en 1 columna, 71% en otra |
| **Registros únicos (por código)** | 3,876 |

### Top 3 Grupos Contables por frecuencia:
1. **Honorarios y Procedimientos Médicos y Quirúrgicos** - 1,853 registros (48%)
2. **Exámenes Auxiliares de Laboratorio** - 901 registros (23%)
3. **Diagnóstico X Imágenes** - 896 registros (23%)

## 🛠️ Tecnologías Utilizadas

- **Python 3.9+**
- **Pandas** - Manipulación de datos
- **NumPy** - Operaciones numéricas
- **Matplotlib / Seaborn** - Visualización
- **Jupyter Notebook** - Análisis interactivo

## 📁 Estructura del Proyecto

```
healthcare-tariff-analysis/
├── README.md
├── data/
│   └── nomenclador_procedimientos.xlsx (datos reales)
├── notebooks/
│   ├── 01_data_loading_and_cleaning.ipynb
│   └── 02_exploratory_data_analysis.ipynb
├── scripts/
│   └── data_quality_check.py
└── requirements.txt
```

## 🚀 Cómo Usar

### 1. Clonar el repositorio
```bash
git clone https://github.com/juanerazo/healthcare-tariff-analysis.git
cd healthcare-tariff-analysis
```

### 2. Instalar dependencias
```bash
pip install -r requirements.txt
```

### 3. Ejecutar análisis
```bash
jupyter notebook notebooks/01_data_loading_and_cleaning.ipynb
```

## 📋 Pasos de Análisis

### Paso 1: Carga y Limpieza de Datos
- ✓ Identificar y eliminar registros vacíos
- ✓ Validar tipos de datos
- ✓ Documentar datos faltantes por columna

### Paso 2: Análisis Exploratorio (EDA)
- ✓ Distribución de procedimientos por categoría
- ✓ Análisis de estados (Activo/Inactivo)
- ✓ Identificación de procedimientos únicos vs duplicados
- ✓ Visualización de patrones

### Paso 3: Validación de Integridad
- ✓ Verificar completitud de datos críticos
- ✓ Detectar anomalías o inconsistencias
- ✓ Generar reporte de calidad

## 💡 Insights Generados

1. **Calidad de datos: 99.9%** - Solo 2 registros completamente vacíos de 3,878
2. **Columnas problemáticas:** 
   - `DE_DETALLE_VALIDACION`: 100% faltante (columna candidata para eliminación)
   - `DE_UNIDAD`: 71% faltante
3. **Data limpia:** 99% de procedimientos tiene código y descripción
4. **Segmentación clara:** 7 grupos contables bien definidos

## 🔍 Casos de Uso

Este análisis es aplicable a:
- Auditoría de nomencladores médicos
- Validación de tarifarios clínicos
- Gestión de integridad de datos en sistemas de salud
- Preparación de datos para reportes gerenciales

## 👤 Autor

**Juan Manuel Erazo Huarache**
- Data Analyst & Backend Developer
- Especialización en SQL Server, Python, análisis de datos
- Contacto: juanm.erazoh@hotmail.com | (+51) 972 712 543

## 📜 Licencia

Este proyecto utiliza datos anonimizados de una clínica peruana. Uso educativo solamente.

---

**Última actualización:** 24 de enero de 2026
