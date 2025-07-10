# Beta-Bank

# 🏦 Predicción de Pérdida de Clientes en Beta Bank

En este proyecto se desarrolla un modelo de machine learning para predecir qué clientes del **Beta Bank** están en riesgo de abandonar el servicio. Este tipo de análisis es clave para implementar estrategias de retención, ya que conservar a un cliente existente resulta significativamente más económico que adquirir uno nuevo.

---

## 📌 Objetivo

El objetivo principal es construir un modelo predictivo con un valor **F1 Score ≥ 0.59**, que permita identificar clientes propensos a cancelar su contrato, utilizando datos históricos del banco.

---

## 🧰 Herramientas y tecnologías

- **Python**
- `pandas`, `numpy`
- `scikit-learn`
- `matplotlib`, `seaborn`
- Modelos: Árboles de decisión, Random Forest, Regresión logística
- Métricas: F1 Score, AUC-ROC

---

## 🔍 Metodología

1. **Exploración y limpieza de datos**  
   - Análisis de valores faltantes y tipos de variables  
   - Distribución de la variable objetivo

2. **Tratamiento del desbalance de clases**  
   - Modelo base (sin ajuste)  
   - `class_weight='balanced'`  
   - Submuestreo manual de la clase mayoritaria  

3. **Entrenamiento y validación de modelos**  
   - Evaluación con F1 Score y curva AUC-ROC  
   - Selección del modelo con mejor balance entre precisión y recall  

---

## 📊 Resultados

- 🔎 **Modelo seleccionado**: Submuestreo + Random Forest  
- ✅ **F1 Score (validación)**: 0.600  
- ✅ **AUC-ROC (validación)**: 0.854  
- 🧪 **F1 Score (prueba)**: 0.605  
- 🧪 **AUC-ROC (prueba)**: 0.868  

---

## ✅ Conclusiones

> En este proyecto se desarrolló un modelo eficaz para anticipar la pérdida de clientes en Beta Bank. A través del análisis exploratorio y el tratamiento del desbalance de clases, se logró construir una solución robusta con alto poder predictivo.

El modelo final no solo **supera el umbral mínimo de F1 requerido**, sino que también mantiene una buena capacidad de generalización, permitiendo al banco tomar decisiones informadas y proactivas. Esta herramienta puede ser integrada en campañas de retención y alertas tempranas para reducir el churn.

---

📁 *Proyecto realizado como parte de mi formación en científica de datos con enfoque en modelado supervisado.*
