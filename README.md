# 🏘️ Pricing sector inmobiliario CABA-AR

Este proyecto fue realizado como trabajo final de la materia **Ciencia de Datos para Economía y Negocios** (FCE – UBA, 2025). El objetivo fue aplicar técnicas de machine learning para estimar el precio de publicación de propiedades inmobiliarias en la Ciudad Autónoma de Buenos Aires, utilizando datos reales del portal Properati.

## 📌 Objetivo

Desarrollar un modelo de pricing que permita predecir el valor de publicación de propiedades, a partir de variables estructurales como m², cantidad de baños, ambientes, tipo de propiedad y barrio.

---

## 🔍 Análisis realizado

- Análisis exploratorio de datos (EDA) y tratamiento de outliers
- Ingeniería de variables (conversión de fechas, superficies, etc.)
- División train/test con semilla
- Modelos implementados:
  - Regresión Lineal (OLS)
  - Lasso (con tuning de alpha)
  - Random Forest
  - Gradient Boosting
  - XGBoost (Bonus)
- Evaluación con métricas: **R², RMSE, MAE**
- Comparación de performance entre modelos

---

## 🧠 Principales resultados

| Modelo             | R²     | RMSE       | MAE        |
|--------------------|--------|------------|------------|
| Regresión Lineal   | 0.6237 | 57222.31   | 40239.37   |
| Lasso              | 0.6236 | 57231.11   | 40247.20   |
| Random Forest      | 0.7875 | 42998.87   | 29477.19   |
| Gradient Boosting  | 0.7669 | 45088.36   | 31928.02   |
| XGBoost            | 0.7741 | 43441.71   | 31154.73   |

📌 **Modelo seleccionado:** Random Forest, por su mejor precisión y menor dispersión de errores.

---

## 🏁 Conclusiones

- El precio puede predecirse con alta precisión incluso en mercados tan heterogéneos como el inmobiliario.
- Los modelos de árboles (RF, XGB) superan ampliamente a los modelos lineales clásicos en este contexto.
- Esta lógica de pricing es extensible a sectores como telecomunicaciones, hotelería, riesgo crediticio y más.

---

## 🛠️ Herramientas utilizadas

- Python
- pandas, numpy, seaborn, matplotlib
- scikit-learn
- xgboost

---

## 👥 Autores

**Mijael Castro Lozano**  
[LinkedIn](https://www.linkedin.com/in/mijaelcastro) | [GitHub](https://github.com/mijaelcastro)

