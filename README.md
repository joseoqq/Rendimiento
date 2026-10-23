# Rendimiento
Analisis del rendimiento academico
# 🎓 Predicción del Riesgo de Bajo Rendimiento Académico con Machine Learning
### *Caso de estudio: Estudiantes de Ingeniería de Minas (2020–2025)*

[![Python 3.11](https://img.shields.io/badge/Python-3.11-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.xxxxxx.svg)](https://doi.org/10.5281/zenodo.xxxxxx)

Repositorio oficial del trabajo de investigación de la **Maestría en Inteligencia Artificial** de la **Universidad César Vallejo (UCV)**. Este proyecto desarrolla un sistema predictivo para identificar tempranamente a estudiantes en riesgo académico, utilizando algoritmos de Machine Learning e Inteligencia Artificial Explicable (XAI).

---

## 🎯 Objetivo de la Tesis

Determinar en qué medida un modelo de Machine Learning permite predecir el rendimiento académico de los estudiantes de Ingeniería de Minas durante el periodo 2020–2025, mediante la implementación y evaluación de diferentes algoritmos de aprendizaje automático aplicados a datos educativos históricos.

El estudio busca no solo maximizar la precisión predictiva (superando el 80% de la hipótesis general), sino también garantizar la **interpretabilidad del modelo** mediante valores SHAP, permitiendo a las instituciones educativas diseñar intervenciones pedagógicas y de bienestar universitario oportunas y personalizadas.

### 🔑 Resultados clave
- **Modelo óptimo:** XGBoost (Accuracy: 96.41%, Recall clase "Bajo": 98.04%)
- **F1-Macro:** 0.9270 ± 0.0325
- **Predictores dominantes:** Tasa de aprobación, promedio mínimo semestral, ritmo de egreso
- **Alineación:** ODS 4 (Educación de Calidad) y RSU

---

##  Estructura del Repositorio
# 📄 README.md para tu Repositorio GitHub

A continuación te presento el archivo `README.md` completo, listo para copiar y pegar en tu repositorio. Está diseñado siguiendo las mejores prácticas de repositorios científicos (principios FAIR) y refleja fielmente la estructura de tu notebook.

---

## 📄 `README.md`

```markdown
# 🎓 Predicción del Riesgo de Bajo Rendimiento Académico con Machine Learning
### *Caso de estudio: Estudiantes de Ingeniería de Minas (2020–2025)*

[![Python 3.11](https://img.shields.io/badge/Python-3.11-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.xxxxxx.svg)](https://doi.org/10.5281/zenodo.xxxxxx)

Repositorio oficial del trabajo de investigación de la **Maestría en Inteligencia Artificial** de la **Universidad César Vallejo (UCV)**. Este proyecto desarrolla un sistema predictivo para identificar tempranamente a estudiantes en riesgo académico, utilizando algoritmos de Machine Learning e Inteligencia Artificial Explicable (XAI).

---

## 🎯 Objetivo de la Tesis

Determinar en qué medida un modelo de Machine Learning permite predecir el rendimiento académico de los estudiantes de Ingeniería de Minas durante el periodo 2020–2025, mediante la implementación y evaluación de diferentes algoritmos de aprendizaje automático aplicados a datos educativos históricos.

El estudio busca no solo maximizar la precisión predictiva (superando el 80% de la hipótesis general), sino también garantizar la **interpretabilidad del modelo** mediante valores SHAP, permitiendo a las instituciones educativas diseñar intervenciones pedagógicas y de bienestar universitario oportunas y personalizadas.

### 🔑 Resultados clave
- **Modelo óptimo:** XGBoost (Accuracy: 96.41%, Recall clase "Bajo": 98.04%)
- **F1-Macro:** 0.9270 ± 0.0325
- **Predictores dominantes:** Tasa de aprobación, promedio mínimo semestral, ritmo de egreso
- **Alineación:** ODS 4 (Educación de Calidad) y RSU

---

##  Estructura del Repositorio

```
.
├── README.md                                    # Documentación principal
├── requirements.txt                             # Dependencias de Python
├── LICENSE                                      # Licencia MIT
├── MITESIS_RENDIMIENTO_ACADEMICO.ipynb          # Notebook principal con el pipeline completo
├── data/                                        # Directorio de datos (NO incluido por privacidad)
│   ├── raw/                                     # Datos originales (bajo solicitud)
│   │   ├── MINAS_2020_2025_AGGREGATED123.csv
│   │   └── reporte Socioeconomico - FICHAS 20201 AL 20252 ING MINAS ACT1123.csv
│   ── processed/                               # Dataset anonimizado final
│       └── MINAS_LIMPIO_IMPUTADO_RIGUROSO_v3.csv
── notebooks/                                   # Notebooks modulares (opcional)
│   ├── 00_diagnostico_fusion.ipynb              # Script 0 y 0v3: Análisis y fusión
│   ├── 01_limpieza_preparacion.ipynb            # Script 1v3: Limpieza y feature engineering
│   ├── 02_analisis_estadistico.ipynb            # Script 2v3: Estadística descriptiva e inferencial
│   ├── 03_pipeline_ml.ipynb                     # Script 3v3: Modelado, SHAP, ROC, LIME
│   └── 04_analisis_complementarios.ipynb        # Scripts adicionales de frecuencia
├── outputs/                                     # Resultados generados
│   ├── tablas/                                  # Tablas en formato CSV
│   │   ├── tabla_01_estadistica_descriptiva_v3.csv
│   │   ├── tabla_05_resultados_validacion_cruzada_v3.csv
│   │   └── tabla_06_reporte_clasificacion_v3.txt
│   └── figuras/                                 # Visualizaciones
│       ├── figura_01_distribucion_promedio_v3.png
│       ├── figura_04_heatmap_correlacion_v3.png
│       ├── figura_06_matriz_confusion_v3.png
│       ├── figura_07_shap_summary_v3.png
│       ├── figura_08_shap_importance_bar_v3.png
│       ├── figura_09_curva_roc_multiclase_v3.png
│       └── figura_10_*_lime_explicacion_v3.png
└── docs/                                        # Documentación adicional
    └── manual_tecnico.pdf
```

---

## 🚀 Instrucciones para Ejecutar el Notebook

### 1. Clonar el repositorio

```bash
git clone https://github.com/tu_usuario/tu_repositorio.git
cd tu_repositorio
```

### 2. Crear y activar un entorno virtual

```bash
# Con venv (Python estándar)
python -m venv venv
source venv/bin/activate    # Linux/Mac
venv\Scripts\activate       # Windows

# O con conda
conda create -n rendimiento_ml python=3.11 -y
conda activate rendimiento_ml
```

### 3. Instalar dependencias

```bash
pip install -r requirements.txt
```

### 4. Colocar los datos

Coloca los archivos CSV en la carpeta `data/raw/`:
- `MINAS_2020_2025_AGGREGATED123.csv`
- `reporte Socioeconomico - FICHAS 20201 AL 20252 ING MINAS ACT1123.csv`

> ⚠️ **Importante:** Los datos reales **no están incluidos** en este repositorio por razones de privacidad. Consulta la sección *Datos* más abajo para solicitar acceso.

### 5. Ejecutar el notebook

```bash
jupyter notebook MITESIS_RENDIMIENTO_ACADEMICO.ipynb
```

Ejecuta las celdas en orden secuencial. El pipeline está organizado en 11 pasos:

| Paso | Descripción |
|------|-------------|
| 0–0v3 | Diagnóstico y fusión de datasets (INNER JOIN) |
| 1v3 | Limpieza, codificación y feature engineering |
| 2v3 | Estadística descriptiva e inferencial (Kruskal-Wallis, Chi-cuadrado, Spearman) |
| 3v3 | Pipeline ML: 6 algoritmos, validación cruzada con SMOTE, SHAP, ROC, LIME |
| Adicional | Análisis de frecuencia y variables socioeconómicas |

### 6. Resultados esperados

Al finalizar, se generarán automáticamente:
- 6 tablas CSV con resultados estadísticos
- 10+ figuras PNG de alta resolución (300 DPI)
- Archivos HTML interactivos de LIME
- Dataset limpio `MINAS_LIMPIO_IMPUTADO_RIGUROSO_v3.csv`

---

## 📦 Dependencias (`requirements.txt`)

```txt
# Core
python==3.11
pandas==2.1.4
numpy==1.26.2
scipy==1.12.0

# Machine Learning
scikit-learn==1.4.0
xgboost==2.0.3
imbalanced-learn==0.12.0

# Explainable AI
shap==0.44.0
lime==0.2.0.1

# Visualización
matplotlib==3.8.2
seaborn==0.13.1

# Entorno
jupyter==1.0.0
ipykernel==6.29.0
```

### Alternativa con Conda (`environment.yml`)

```yaml
name: rendimiento_ml
channels:
  - defaults
  - conda-forge
dependencies:
  - python=3.11
  - pandas=2.1.4
  - numpy=1.26.2
  - scipy=1.12.0
  - scikit-learn=1.4.0
  - matplotlib=3.8.2
  - seaborn=0.13.1
  - jupyter=1.0.0
  - pip:
    - xgboost==2.0.3
    - imbalanced-learn==0.12.0
    - shap==0.44.0
    - lime==0.2.0.1
```

---

## 📊 Nota sobre la Procedencia y Uso Permitido de los Datos

### ⚠️ Privacidad y Ética de los Datos

Los datos utilizados en esta investigación provienen de **registros académicos y socioeconómicos institucionales** de una universidad pública del sur del Perú (Periodo 2020–2025), correspondientes a 833 estudiantes de la Escuela Profesional de Ingeniería de Minas.

- **Anonimización:** En cumplimiento con la **Ley N° 29733** (Ley de Protección de Datos Personales del Perú) y el **Código de Ética en Investigación de la UCV (RCU N° 0157-2025)**, todos los identificadores directos (DNI, nombres, códigos de estudiante) han sido eliminados.
- **Acceso:** El dataset anonimizado **no se incluye directamente** en este repositorio público para prevenir cualquier riesgo de re-identificación.
- **Solicitud de datos:** Los investigadores interesados en replicar los resultados pueden solicitar el dataset anonimizado contactando al autor principal, quienes deberán firmar un **acuerdo de uso de datos** con fines estrictamente académicos y de investigación.
- **Reproducibilidad:** Se incluye un script en la carpeta `notebooks/` para generar un **dataset sintético** con la misma estructura y distribuciones estadísticas, permitiendo probar el pipeline de código sin necesidad de los datos reales.

### 🔓 Uso permitido
- ✅ Investigación académica y científica
- ✅ Replicación y validación de resultados
- ✅ Enseñanza y docencia (con citación adecuada)
- ❌ Uso comercial sin autorización expresa
- ❌ Intentos de re-identificación de sujetos
- ❌ Redistribución de los datos originales

---

## 📝 Cómo Citar este Trabajo

Si utilizas este código, metodología o resultados en tu propia investigación, por favor cita el trabajo de la siguiente manera:

### Formato APA 7ª edición

> Quintana Quispe, J. O. (2026). *Predicción del riesgo de bajo rendimiento académico mediante algoritmos de Machine Learning en estudiantes de Ingeniería de Minas, 2020–2025* [Tesis de Maestría, Universidad César Vallejo]. Repositorio GitHub. https://doi.org/10.5281/zenodo.xxxxxx

### Formato BibTeX

```bibtex
@mastersthesis{quintana2026prediccion,
  title={Predicción del riesgo de bajo rendimiento académico mediante algoritmos de Machine Learning en estudiantes de Ingeniería de Minas, 2020–2025},
  author={Quintana Quispe, José Orlando},
  year={2026},
  school={Universidad César Vallejo},
  address={Lima, Perú},
  note={Repositorio GitHub: https://github.com/tu_usuario/tu_repositorio}
}
```

### Citar el software

```bibtex
@software{quintana2026ml_rendimiento,
  author = {Quintana Quispe, José Orlando},
  title = {ML Rendimiento Académico - Ingeniería de Minas},
  year = {2026},
  url = {https://github.com/tu_usuario/tu_repositorio},
  version = {1.0.0}
}
```

---

## 📄 Licencia

- **Código fuente:** Este proyecto está licenciado bajo la [Licencia MIT](LICENSE). Eres libre de usar, copiar, modificar y distribuir el código, siempre que se mantenga el aviso de copyright original.
- **Documentación y textos:** Licenciados bajo [Creative Commons Attribution 4.0 (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
- **Datos:** El acceso a los datos está sujeto a un acuerdo de uso específico que prohíbe su uso comercial o la intentona de re-identificación de sujetos.

---

##  Agradecimientos

Se agradece a la **Universidad Nacional de Moquegua** por facilitar el acceso a los registros académicos y socioeconómicos para materializar este estudio. Agradezco también al asesor de tesis, **MSc. Rubén Quispe Llacctarimay**, por su orientación rigurosa y observaciones precisas en cada etapa del proceso. Finalmente, extiendo mi gratitud a la **Universidad César Vallejo** y a su programa de Maestría en Inteligencia Artificial por brindar el espacio formativo que hizo posible esta investigación.

---

## 📬 Contacto

**José Orlando Quintana Quispe**  
Maestría en Inteligencia Artificial — Universidad César Vallejo  
 jose.quintana@ucv.edu.pe  
🆔 ORCID: [0000-0001-6487-1313](https://orcid.org/0000-0001-6487-1313)

---

*Desarrollado con ❤️ para la comunidad académica peruana | 2026*
```

---

## 📄 `requirements.txt` (archivo independiente)

```txt
# Core data science
pandas==2.1.4
numpy==1.26.2
scipy==1.12.0

# Machine Learning
scikit-learn==1.4.0
xgboost==2.0.3
imbalanced-learn==0.12.0

# Explainable AI (XAI)
shap==0.44.0
lime==0.2.0.1

# Visualization
matplotlib==3.8.2
seaborn==0.13.1

# Jupyter environment
jupyter==1.0.0
ipykernel==6.29.0
```

---

##  `LICENSE` (Licencia MIT)

Crea un archivo llamado `LICENSE` en la raíz del repositorio con este contenido:

```
MIT License

Copyright (c) 2026 José Orlando Quintana Quispe

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 💡 Tips adicionales para tu repositorio

1. **DOI de Zenodo:** Vincula tu repositorio GitHub con [Zenodo](https://zenodo.org) desde *Settings → Archives*. Zenodo te dará un DOI real (ej. `10.5281/zenodo.1234567`) que reemplazará `xxxxxx` en el README. Esto le da **validez científica** a tu código.

2. **Dataset sintético:** Crea un script `generate_synthetic_data.py` que genere un CSV con ~100 filas aleatorias respetando las mismas columnas y rangos de tu tesis. Esto permitirá que cualquier persona que clone tu repo pueda ejecutar los notebooks sin errores de `FileNotFoundError`.

3. **`.gitignore` recomendado:**
   ```gitignore
   # Datos sensibles
   data/raw/*.csv
   *.csv
   !requirements.txt
   
   # Outputs grandes
   outputs/figuras/*.png
   outputs/tablas/*.csv
   
   # Entornos
   venv/
   .conda/
   __pycache__/
   .ipynb_checkpoints/
   
   # Sistema
   .DS_Store
   Thumbs.db
   ```

4. **GitHub Topics:** Añade estos topics a tu repositorio para mejorar su descubribilidad: `machine-learning`, `educational-data-mining`, `xgboost`, `shap`, `explainable-ai`, `academic-performance`, `peru`, `mining-engineering`.

5. **GitHub Actions (opcional):** Puedes añadir un workflow que ejecute automáticamente los notebooks al hacer push para verificar que el pipeline sigue funcionando.

Con este README tu repositorio quedará profesional, reproducible y alineado con los estándares de ciencia abierta. 🚀
