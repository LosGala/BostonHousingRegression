# Predicción del Valor de Viviendas con Regresión Lineal (BostonHousing)

Este proyecto utiliza el conjunto de datos `BostonHousing` para entrenar un modelo de regresión lineal que predice el valor medio de las viviendas (variable `medv`). Se emplea el paquete `caret` de R para preparar los datos, entrenar el modelo y evaluar su desempeño.

---

## 📦 Librerías utilizadas

- `mlbench`: contiene el dataset BostonHousing.
- `caret`: proporciona funciones para entrenamiento y evaluación de modelos.
- `ggplot2` (opcional): para visualizaciones más detalladas.

---

## 🧪 Dataset

El dataset **BostonHousing** contiene información de diversas características de barrios en Boston. La variable objetivo `medv` representa el valor medio de las viviendas.

---

## ⚙️ Flujo del Proyecto

1. **Carga de datos**  
   Se importa el dataset y se verifica la presencia de datos faltantes.

2. **Preprocesamiento**  
   - División de los datos en conjunto de entrenamiento (80%) y prueba (20%) usando partición estratificada.  
   - Normalización de los datos (`center` y `scale`).

3. **Entrenamiento del Modelo**  
   - Se entrena un modelo de regresión lineal (`method = "lm"`).
   - No se usa validación cruzada en esta versión base.

4. **Predicción**  
   - Se hacen predicciones sobre el conjunto de entrenamiento y prueba.

5. **Evaluación del Modelo**  
   - Visualización mediante gráficos de dispersión.
   - (Se recomienda agregar métricas como RMSE, MAE y R² para mayor análisis).

---

## 📈 Resultados esperados

Gráficos de dispersión que muestran la relación entre los valores reales y los predichos por el modelo. Un buen modelo debería mostrar una distribución cercana a la línea de 45 grados.


