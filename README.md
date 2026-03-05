### **ML_Prevencion_infartos** **SPA**

**Descripción del problema:** ¿Qué problema de negocio se quiere resolver?

Las enfermedades cardíacas son una de las principales causas de mortalidad a nivel mundial. La detección temprana de pacientes con alto riesgo cardiovascular es clave para aplicar medidas preventivas y mejorar los resultados clínicos.


El objetivo de este proyecto es desarrollar un modelo de Machine Learning capaz de predecir si una persona tiene riesgo de sufrir un ataque cardíaco, utilizando variables relacionadas con su salud, estilo de vida y antecedentes médicos.

---

- **Dataset utilizado:** Descripción breve, si es público o privado, y cómo acceder a él

Se ha utilizado un dataset público que contiene información sobre el estado de salud de pacientes, incluyendo:

- Variables demográficas (edad, sexo)
- Indicadores físicos (BMI, peso, altura)
- Hábitos de vida (actividad física, tabaquismo)
- Condiciones médicas previas (diabetes, angina, etc.)
- Estado general de salud

Variable objetivo:

- `HadHeartAttack` → indica si el paciente ha sufrido un ataque cardíaco o no.

El dataset es público y puede encontrarse en la plataforma Kaggle en el siguiente enlace: https://www.kaggle.com/datasets/kamilpytlak/personal-key-indicators-of-heart-disease 

---

- **Solución adoptada:** Descripción breve de la aproximación de ML utilizada
Se ha seguido un enfoque supervisado de clasificación utilizando Machine Learning.

Las principales etapas han sido:

1. Análisis exploratorio de datos (EDA)
2. Limpieza e imputación de valores faltantes
3. Selección de variables relevantes
4. Preparación de datos para modelado
5. División en conjunto de entrenamiento y test
6. Entrenamiento y evaluación de modelos de clasificación

Se han identificado las variables con mayor capacidad predictiva, como:

- HadAngina
- HadStroke
- GeneralHealth
- AgeCategory
- HadDiabetes

---

- **Estructura del repositorio:** Breve explicación de la organización de carpetas
1. **`src/data_sample/`** - Muestra del dataset utilizado

2. **`src/img/`** - Imágenes necesarias o generadas para el proyecto

3. **`src/models/`** - Modelos entrenados guardados

4. **`src/notebooks/`** - Notebooks de desarrollo y pruebas
   
5. **`src/utils/`** - Código auxiliar reutilizable
     
---

- **Tecnologías utilizadas:** Librerías, herramientas, lenguajes

Lenguaje:

- Python

Librerías principales:

- Pandas
- Numpy
- Matplotlib
- Seaborn
- Scikit-learn

Herramientas:

- Jupyter Notebook
- Git
- GitHub

---

- **Instrucciones de reproducción:** Cómo ejecutar el código

Para reproducir el análisis y los resultados del proyecto, se debe ejecutar el archivo **main.ipynb**, ubicado en la rama main del repositorio. Este notebook contiene todo el flujo de trabajo del proyecto, incluyendo la exploración de datos, el preprocesamiento, el entrenamiento de los modelos y la evaluación de resultados.

Para garantizar su correcta ejecución, es necesario ejecutar las celdas en el orden en el que aparecen dentro del notebook. Cada bloque de código está acompañado de explicaciones que describen el proceso realizado y los resultados obtenidos en cada etapa del análisis.

De este modo, siguiendo el orden secuencial del notebook, es posible reproducir todo el proceso de análisis y modelado desarrollado en el proyecto.


---

- **Principales resultados:** Resumen de las métricas y conclusiones

El objetivo del proyecto fue desarrollar un modelo de machine learning capaz de predecir el riesgo de ataque cardíaco a partir de variables médicas y de estilo de vida. 

Tras el análisis exploratorio, se identificaron como variables más relevantes la edad, el estado general de salud, los días de mala salud física, el peso corporal y antecedentes médicos como angina o ictus. Estas variables mostraron mayor relación con la probabilidad de sufrir un ataque cardíaco. 

Se entrenaron y compararon varios modelos de clasificación utilizando ROC-AUC como métrica principal para evaluar su capacidad discriminativa. Los modelos evaluados fueron:

* **Regresión Logística (baseline)**

* **Random Forest**

* **Gradient Boosting**

* **XGBoost**

En el conjunto de test, los resultados fueron:

- **XGBoost: ROC-AUC ≈ 0.884**

- **Gradient Boosting: ROC-AUC ≈ 0.884**

- **Regresión Logística: ROC-AUC ≈ 0.883**

- **Random Forest: ROC-AUC ≈ 0.865**

Debido a su mejor rendimiento, **XGBoost** fue seleccionado como modelo final. Tras la optimización de hiperparámetros y la validación cruzada, el modelo alcanzó en el conjunto de test:

- **ROC-AUC: ~ 0.878**

- **Accuracy: ~ 88%**

*Estos resultados indican que el modelo tiene buena capacidad para discriminar entre pacientes con mayor o menor riesgo de ataque cardíaco, lo que podría ser útil como herramienta de apoyo en contextos de prevención clínica.*

---

- **Autores:** Nombres y enlaces a perfiles de GitHub

1. Alejandro Arbide: https://github.com/alejandroarbide | https://www.linkedin.com/in/alejandro-arbide/
2. Camila Fiore: https://github.com/cflorenciafiore | https://www.linkedin.com/in/camilafiore/
3. Judit García: https://github.com/Juditga97 | https://www.linkedin.com/in/judit-garcia-aguilar/

---

### **ML_Heart_Attack_Prevention** **ENG**


**Problem Description:** What business problem is being addressed?

Heart disease is one of the leading causes of mortality worldwide. Early detection of patients at high cardiovascular risk is crucial to enable preventive measures and improve clinical outcomes.

The objective of this project is to develop a Machine Learning model capable of predicting whether a person is at risk of suffering a heart attack, using variables related to their health, lifestyle, and medical history.

---

**Dataset:** Brief description, whether it is public or private, and how to access it

A public dataset has been used containing information about patients’ health status, including:

- Demographic variables (age, sex)
- Physical indicators (BMI, weight, height)
- Lifestyle habits (physical activity, smoking)
- Previous medical conditions (diabetes, kidney disease, angina, etc.)
- General health status

Target variable:

- `HadHeartAttack` → indicates whether the patient has suffered a heart attack or not.

The dataset is public and can be accessed on Kaggle at the following link:  
https://www.kaggle.com/datasets/kamilpytlak/personal-key-indicators-of-heart-disease 

---

**Solution:** Brief description of the Machine Learning approach used

A supervised Machine Learning classification approach has been followed.

The main stages were:

1. Exploratory Data Analysis (EDA)
2. Data cleaning and missing value imputation
3. Relevant feature selection
4. Data preparation for modeling
5. Train-test split
6. Training and evaluation of classification models

The variables with the highest predictive power identified include:

- HadAngina
- HadStroke
- GeneralHealth
- AgeCategory
- HadDiabetes

---

**Repository Structure:** Brief explanation of folder organization
1. **`src/data_sample/`** - Sample of the dataset used (only if it is public)

2. **`src/img/`** - Images required or generated for the project

3. **`src/models/`** - Saved trained models

4. **`src/notebooks/`** - Development and experimentation notebooks

5. **`src/utils/`** - Reusable auxiliary code

---

**Technologies Used:** Libraries, tools, and languages

Language:

- Python

Main libraries:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

Tools:

- Jupyter Notebook
- Git
- GitHub

---

- **Instructions to reproduce:** How to run the code

To reproduce the analysis and results of this project, the file **main.ipynb** must be executed. This notebook is located in the main branch of the repository and contains the complete workflow of the project, including data exploration, preprocessing, model training, and evaluation of the results.

For the notebook to run correctly, the cells should be executed in the same order in which they appear. Each code block is accompanied by explanations that describe the steps performed and the results obtained throughout the analysis.

By following the notebook sequentially, it is possible to reproduce the entire analysis and modeling process developed in this project.

---

- **Main Results:** Summary of metrics and conclusions

The objective of this project was to develop a machine learning model capable of predicting the risk of heart attack using medical and lifestyle data. 

During the exploratory data analysis, several variables showed a stronger relationship with the target variable. The most relevant predictors included age, general health condition, number of days with poor physical health, body weight, and medical history such as angina or stroke. 

To evaluate predictive performance, ROC-AUC was selected as the main evaluation metric, as it measures the model’s ability to correctly distinguish between patients with and without heart attack risk. Four classification models were trained and compared:

- **Logistic Regression (baseline)**

- **Random Forest**

- **Gradient Boosting**

- **XGBoost**

On the test dataset, the models achieved the following results:

- **XGBoost: ROC-AUC ≈ 0.884**

- **Gradient Boosting: ROC-AUC ≈ 0.884**

- **Logistic Regression: ROC-AUC ≈ 0.883**

- **Random Forest: ROC-AUC ≈ 0.865**

Among them, XGBoost showed the best predictive performance and was selected as the final model. After hyperparameter optimization and cross-validation, the final model achieved:

- **ROC-AUC: ~ 0.878**

- **Accuracy: ~ 88% on the independent test set.**

*These results indicate that the model has a strong ability to identify patterns associated with heart attack risk, making it a potential tool for supporting preventive decision-making in healthcare contexts.*

---

- **Authors:** Names and links to GitHub profiles

1. Alejandro Arbide: https://github.com/alejandroarbide | https://www.linkedin.com/in/alejandro-arbide/
2. Camila Fiore: https://github.com/cflorenciafiore | https://www.linkedin.com/in/camilafiore/
3. Judit García: https://github.com/Juditga97 | https://www.linkedin.com/in/judit-garcia-aguilar/
