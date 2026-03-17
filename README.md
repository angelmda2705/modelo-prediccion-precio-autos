# modelo-prediccion-precio-autos
---

# 📊 Descripción del Proyecto

Rusty Bargain es un servicio de venta de autos usados que está desarrollando una aplicación para estimar **el valor de mercado de un vehículo** de forma rápida y precisa.

Este proyecto desarrolla varios modelos de **Machine Learning de regresión** para predecir el precio de autos usados utilizando características técnicas del vehículo.

La empresa está interesada en optimizar tres factores principales:

- **Calidad de la predicción**
- **Velocidad de predicción**
- **Tiempo de entrenamiento del modelo**

---

# 🎯 Objetivo del Proyecto

Construir y comparar diferentes modelos de Machine Learning capaces de predecir el precio de autos usados, evaluando su rendimiento mediante métricas de error y eficiencia computacional.

---

# 📂 Dataset

El dataset contiene información sobre vehículos usados incluyendo:

- Año de registro
- Potencia del motor
- Kilometraje
- Tipo de vehículo
- Marca
- Modelo
- Tipo de combustible
- Tipo de transmisión

Variable objetivo:

**Price → precio del automóvil**

---

# ⚙️ Metodología

El proyecto siguió las siguientes etapas de Ciencia de Datos:

1. Exploración y limpieza de datos  
2. Selección de variables relevantes  
3. Codificación de variables categóricas mediante **One Hot Encoding**  
4. División del dataset en entrenamiento y prueba  
5. Entrenamiento de múltiples modelos de regresión  
6. Evaluación y comparación de modelos  

---

# 🤖 Modelos Evaluados

Se entrenaron y compararon los siguientes modelos:

- Regresión Lineal
- Random Forest
- LightGBM
- Decision Tree

---

# 📈 Resultados

Comparación del desempeño de los modelos:

| Modelo | RMSE | MAE | R² | Tiempo |
|------|------|------|------|------|
| Regresión Lineal | 2340.60 | 1666.03 | 0.74 | 5.10 s |
| Random Forest (200) | **1547.14** | **967.97** | **0.89** | 28.0 min |
| LightGBM (300) | 1571.10 | 1028.77 | 0.88 | **5.57 s** |
| Decision Tree (15) | 1784.91 | 1144.26 | 0.85 | 10.27 s |

---

# 🧠 Conclusiones

El análisis muestra diferencias importantes entre los modelos evaluados:

- **Random Forest** obtuvo la mejor precisión con el menor RMSE y el mayor R², aunque con un tiempo de entrenamiento considerablemente alto.
- **LightGBM** logró un rendimiento muy cercano al de Random Forest, pero con un **tiempo de entrenamiento significativamente menor**, lo que lo convierte en una opción más eficiente para aplicaciones en producción.
- **Regresión Lineal** fue el modelo más rápido pero con menor precisión.
- **Decision Tree** mostró un rendimiento intermedio entre velocidad y precisión.

En general, **LightGBM representa el mejor equilibrio entre precisión y eficiencia computacional**, por lo que sería el modelo más adecuado para implementar en la aplicación de Rusty Bargain.

---

# 🛠️ Tecnologías Utilizadas

- Python
- Pandas
- NumPy
- Scikit-learn
- LightGBM
- Matplotlib
- Jupyter Notebook

---

# 👨‍💻 Autor

**Angel Mendiola Del Angel**

Ingeniero Industrial | Científico de Datos
