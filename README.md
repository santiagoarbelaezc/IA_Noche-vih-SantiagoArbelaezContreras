<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:667eea,100:764ba2&height=120&section=header&animation=fadeIn" />
</div>

<h1 align="center">🚀 IA_Noche — Análisis VIH vs Sano</h1>
<h3 align="center">📊 EDA & preprocesamiento — `codigo.ipynb`</h3>

<p align="center">
  Notebook de análisis exploratorio y preprocesamiento para el dataset <strong>`Dataset_VIH_vs_Sano_v3.csv`</strong>.<br>
  Incluye carga local del CSV, inspección de datos, detección de nulos/duplicados, visualizaciones y recomendaciones para modelado.  
</p>

---

## 🎯 Descripción general

Repositorio con un notebook Jupyter que realiza un análisis exploratorio completo del dataset VIH vs Sano: limpieza básica, verificación de consistencia, estadísticas descriptivas y visualizaciones listas para preparar modelos de clasificación.

---

## ✨ Características principales

- ✅ Lectura local de `Dataset_VIH_vs_Sano_v3.csv` (sin Google Drive)  
- ✅ Resumen general: forma, memoria, vista previa  
- ✅ Detección y visualización de nulos por columna  
- ✅ Detección de duplicados y registros inconsistentes  
- ✅ Análisis de tipos de variables (numéricas / categóricas / booleanas)  
- ✅ Estadísticas descriptivas y boxplots para numéricas  
- ✅ Distribución y balanceo de la variable objetivo (`Clase`)  
- ✅ Gráficas limpias (Seaborn / Matplotlib) y tablas `display()`  
- ✅ Recomendaciones para preprocesamiento y modelado

---

## 📋 Qué hace `codigo.ipynb`

1. Carga y validación del CSV local  
2. Muestra resumen, head/tail, tipos y ejemplos de columnas  
3. Informe y gráfico de valores nulos por columna  
4. Detección de duplicados y filas con inconsistencias lógicas  
5. Análisis de variables categóricas (frecuencias + pie charts)  
6. Estadísticas y boxplots para variables numéricas  
7. Análisis detallado de la variable objetivo `Clase`  
8. Tabla resumen + recomendaciones reproducibles

---

## 🗂️ Estructura del proyecto

```
IA_Noche-vih-SantiagoArbelaezContreras/
├── codigo.ipynb
├── Dataset_VIH_vs_Sano_v3.csv
└── README.md
```

---

## 🛠️ Stack tecnológico

<div align="center">
  <img src="https://img.shields.io/badge/Python-3.11%2B-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img width="8" />
  <img src="https://img.shields.io/badge/Pandas-2.x-150458?style=for-the-badge&logo=pandas&logoColor=white" />
  <img width="8" />
  <img src="https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white" />
  <img width="8" />
  <img src="https://img.shields.io/badge/Matplotlib%20%7C%20Seaborn-visuals-0A0A0A?style=for-the-badge" />
</div>

---

## 🚀 Cómo ejecutar

### Opción A — VS Code / Jupyter (recomendado)
1. Abrir el repo en VS Code o JupyterLab.  
2. Abrir `codigo.ipynb`.  
3. Ejecutar las celdas (ejecutar secuencialmente).

### Opción B — Instalar dependencias
```bash
python -m pip install --upgrade pip
pip install pandas numpy matplotlib seaborn jupyterlab
```

### Opción C — Ejecutar notebook desde terminal
```bash
jupyter notebook codigo.ipynb
# o
jupyter lab
```

---

## 📊 Salida de ejemplo (extracto)
```
================================================================================
✅ ARCHIVO CARGADO EXITOSAMENTE
================================================================================

📊 INFORMACIÓN GENERAL:
   • Dimensiones: 1200 filas × 32 columnas
   • Memoria utilizada: 12.34 MB

🔍 VALORES NULOS POR COLUMNA:
  Columna                 Valores Nulos  Porcentaje
  Sexo                          5           0.42
  CD4                         120          10.00

🎯 DISTRIBUCIÓN DE LA VARIABLE OBJETIVO 'Clase':
Sano    840
VIH     360
Porcentajes:
Sano    70.00
VIH     30.00
```
(La salida real depende del contenido de `Dataset_VIH_vs_Sano_v3.csv`.)

---

## 💡 Recomendaciones rápidas
- Imputar o eliminar columnas con alto % de nulos.  
- Revisar duplicados que cambian `Clase`.  
- Normalizar/estandarizar variables numéricas antes de modelar.  
- Si la clase está desbalanceada, usar re-muestreo o ajustar pesos.

> ⚠️ Este dataset contiene información clínica — maneja con responsabilidad y siguiendo reglas de privacidad.

---

## 📚 Referencias y próximos pasos
- Añadir pipeline de preprocesamiento (scikit-learn).  
- Crear notebook separado para entrenamiento (train / eval / ROC).  
- Exportar reportes en HTML con `nbconvert`.

---

## 👨‍💻 Autor / Contacto
**Santiago Arbelaez Contreras** — Estudiante / Developer  
GitHub: https://github.com/santiagoarbelaezc

---

## 📜 Licencia
MIT — usa y modifica con atribución.

---

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:667eea,100:764ba2&height=90&section=footer&animation=fadeIn" />
</div>