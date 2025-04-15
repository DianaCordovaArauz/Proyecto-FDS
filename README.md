# Proyecto-FDS
Proyecto FDS
# Proyecto-FDS
Proyecto FDS
# 🔥 Análisis de Vulnerabilidad Habitacional ante una Erupción del Volcán Cotopaxi

Este proyecto analiza la **vulnerabilidad socioeconómica de hogares en seis provincias del Ecuador** frente a una posible erupción del volcán Cotopaxi, utilizando **modelos de clustering no supervisado** sobre datos del **Censo Nacional 2022**.

---

## 🎯 Objetivo

Desarrollar una herramienta que permita **segmentar hogares según su nivel de vulnerabilidad**, integrando factores como condiciones de vivienda, densidad habitacional y acceso a servicios básicos. Los resultados pueden ser utilizados por entidades públicas, ONGs y organismos internacionales para:

- Planificación territorial y gestión de riesgos
- Identificación de zonas prioritarias
- Adaptación climática en zonas de alta exposición

---

## 📊 Dataset

- Fuente: **Censo Nacional de Población y Vivienda 2022** (INEC - Ecuador)
- Formato: `.csv`, estructurado
- Tamaño: +3 millones de registros de hogares
- Variables: materiales de construcción, servicios básicos, tenencia, acceso a internet, número de personas, etc.

---

## ⚙️ Estructura del Proyecto


---

## 🧪 Metodología

- **Data Wrangling**: combinación de datos de vivienda y hogar, one-hot encoding, imputación con KNN, normalización.
- **Feature Engineering**: creación de índices de vulnerabilidad, personas por cuarto, hacinamiento.
- **Modelado**:
  - `KMeans`
  - `MiniBatchKMeans`
  - `Agglomerative Clustering`
- **Evaluación**:
  - Silhouette Score
  - Davies-Bouldin Index
  - Calinski-Harabasz Index

### 🥇 Resultados comparativos

| Modelo              | Silhouette ↑ | Davies ↓ | Calinski ↑ |
|---------------------|--------------|----------|-------------|
| KMeans              | 0.45         | 0.88     | 1320.0      |
| MiniBatchKMeans     | 0.42         | 0.92     | 1280.0      |

> KMeans tuvo un rendimiento ligeramente mejor, pero MiniBatchKMeans es más escalable.

---

## 🌍 Impacto Esperado

- Focalización precisa de recursos para políticas públicas
- Mejora de la resiliencia ante desastres
- Mayor eficiencia en programas sociales
- Apoyo en decisiones para adaptación al cambio climático

---

## 🚀 Próximos pasos

- Integración con capas geográficas para visualización
- Desarrollo de dashboard interactivo
- Incorporación de más variables (servicios públicos, percepción de riesgo)
- Despliegue mediante API (FastAPI/Flask)

---

## 🧾 Créditos

**Autora**: Diana Belén Córdova-Aráuz  
**Curso**: Fundamentos de Ciencias de Datos – USFQ  
**Fecha**: Abril 2025
