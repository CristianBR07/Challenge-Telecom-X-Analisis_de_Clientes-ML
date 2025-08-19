# 📊 Customer Churn Prediction

Este proyecto tiene como objetivo **predecir la cancelación de clientes (Churn)** en una empresa de telecomunicaciones utilizando **Machine Learning**.  
Se explora, procesa y modela el dataset para identificar los factores más relevantes que influyen en la decisión de un cliente de abandonar el servicio.

---

## 📂 Contenido del Proyecto

- **EDA (Exploratory Data Analysis)**  
  - Análisis de correlaciones.  
  - Relación de variables clave con la cancelación (tenure, total charges, contract type, etc.).  
  - Visualizaciones (boxplots, scatterplots, heatmaps).

- **Preprocesamiento de Datos**  
  - Codificación de variables categóricas con `get_dummies()`.  
  - Revisión y tratamiento de valores nulos.  
  - División en conjuntos de entrenamiento y prueba.  
  - (Opcional) Balanceo de clases con técnicas como SMOTE.

- **Modelos de Machine Learning**  
  - **Regresión Logística** (modelo interpretable y sensible a escala).  
  - **Random Forest** (modelo robusto, no sensible a escala).  

- **Evaluación de Modelos**  
  - Métricas utilizadas: Accuracy, Precision, Recall, F1-score y ROC-AUC.  
  - Comparación entre modelos para seleccionar el más adecuado.

---

## ⚙️ Tecnologías Utilizadas

- **Python 3**  
- Librerías principales:  
  - `pandas`, `numpy` → Manipulación de datos.  
  - `matplotlib`, `seaborn` → Visualización.  
  - `scikit-learn` → Modelado y métricas.

---

## 📈 Resultados

- **Random Forest**  
  - Accuracy: 0.75  
  - Recall (churners): 0.50  
  - ROC-AUC: 0.79  

- **Regresión Logística**  
  - Accuracy: 0.78  
  - Recall (churners): 0.57  
  - ROC-AUC: 0.82  

👉 La **Regresión Logística resultó ser el mejor modelo base**, ya que logra un mejor balance entre precisión y recall, además de un ROC-AUC superior.  

---

## ✅ Conclusiones

- Existe un **desbalance en las clases** (mayoría de clientes no cancelan).  
- La **Regresión Logística** es preferible como modelo inicial por su mejor desempeño en la detección de clientes con riesgo de cancelar.  
- Futuras mejoras:  
  1. Aplicar balanceo de clases (SMOTE, oversampling).  
  2. Optimizar hiperparámetros en Random Forest y probar con **XGBoost**.  
  3. Crear nuevas variables derivadas (feature engineering).

---
