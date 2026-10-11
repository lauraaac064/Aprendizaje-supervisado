# Aprendizaje supervisado

**Creado por:** Laura Cortés Hoyos  

---

## Descripción del dataset:

Para este trabajo se utilizó la base de datos Breast Cancer Wisconsin (Diagnostic), obtenida de Kaggle. El conjunto contiene 569 observaciones y 30 variables predictoras numéricas relacionadas con las características de los núcleos celulares. La variable objetivo permite clasificar los tumores como benignos o malignos.

---

## Objetivo del trabajo: 

Comparar el rendimiento de tres modelos clásicos de clasificación supervisada: regresión logística, K vecinos más cercanos (KNN) y árbol de decisión. Para evaluar su desempeño, se utilizó la métrica ROC AUC y validación cruzada estratificada de cinco folds.

---

## Metodología: 

Los datos se dividieron en tres conjuntos: entrenamiento (60 %), validación (20 %) y prueba (20 %). Se aplicó estandarización mediante StandardScaler y se evaluaron los modelos utilizando sus hiperparámetros por defecto. Posteriormente, se compararon los resultados de entrenamiento, validación y validación cruzada para seleccionar el modelo con mejor desempeño.

---

## Principales resultados:

- Regresión logística: obtuvo un ROC AUC promedio de 0.9939 en validación cruzada, con una desviación estándar de 0.0074.

- KNN: alcanzó un ROC AUC promedio de 0.9775, con una desviación estándar de 0.0208.

- Árbol de decisión: obtuvo un ROC AUC promedio de 0.9092, mostrando un posible sobreajuste debido a su alto desempeño en entrenamiento y menor resultado en validación.

En la evaluación final, la regresión logística obtuvo un ROC AUC de 0.9940 en el conjunto de prueba.

---

## Conclusiones:

La regresión logística presentó el mejor desempeño y la mayor estabilidad entre los tres modelos evaluados. Además, su resultado en el conjunto de prueba fue muy similar al promedio de validación cruzada, lo que aporta evidencia favorable sobre su capacidad de generalización. Por tanto, fue el modelo seleccionado para este problema de clasificación.
