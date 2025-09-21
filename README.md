**Análisis y Reporte sobre el desempeño de un modelo de Clasificación**
---

En este proyecto se implementa y evalúa un Árbol de Decisión utilizando el dataset de cáncer de mama de scikit-learn.
El objetivo es analizar el desempeño del modelo antes y después de aplicar técnicas de regularización para mejorar su capacidad de generalización.

**Flujo del proyecto**
---

Carga de datos
- Se utiliza el dataset breast_cancer de sklearn.datasets.
- Se separan los datos en Train (60%), Validación (20%) y Test (20%).

Entrenamiento de modelo base
- Se entrena un DecisionTreeClassifier sin restricciones.
- Se miden las métricas de desempeño (accuracy en train, validación y test).
- Se genera un reporte de clasificación y una matriz de confusión.


Regularización del modelo
- Se limitó la profundidad (max_depth=5).
- Se agregaron restricciones de división (min_samples_split=20, min_samples_leaf=10).



Se evalúa la regularización
- Accuracy en validación y test mejora y se vuelven más consistentes.
- Se muestra una comparación gráfica de los resultados.

**Resultados**
---

Modelo base:
- Accuracy Train = 1.00
- Accuracy Validación = 0.95
- Accuracy Test = 0.90

Modelo regularizado:
- Accuracy Validación = 0.94
- Accuracy Test = 0.92


**Tecnologías utilizadas**
---

Python 3
scikit-learn

matplotlib

seaborn
