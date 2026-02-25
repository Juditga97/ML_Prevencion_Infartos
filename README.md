### **ML_Prevencion_infartos** **SPA**

**Descripción del problema:** ¿Qué problema de negocio se quiere resolver?

Las enfermedades cardíacas son una de las principales causas de mortalidad a nivel mundial. La detección temprana de pacientes con alto riesgo cardiovascular es clave para aplicar medidas preventivas y mejorar los resultados clínicos.

El objetivo de este proyecto es desarrollar un modelo de Machine Learning capaz de predecir si una persona tiene riesgo de sufrir un ataque cardíaco, utilizando variables relacionadas con su salud, estilo de vida y antecedentes médicos.

- **Dataset utilizado:** Descripción breve, si es público o privado, y cómo acceder a él
Se ha utilizado un dataset público que contiene información sobre el estado de salud de pacientes, incluyendo:

- Variables demográficas (edad, sexo)
- Indicadores físicos (BMI, peso, altura)
- Hábitos de vida (actividad física, tabaquismo)
- Condiciones médicas previas (diabetes, enfermedad renal, angina, etc.)
- Estado general de salud

Variable objetivo:

- `HadHeartAttack` → indica si el paciente ha sufrido un ataque cardíaco o no.

El dataset es público y puede encontrarse en la plataforma Kaggle en el siguiente enlace: https://www.kaggle.com/datasets/kamilpytlak/personal-key-indicators-of-heart-disease 

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

- **Estructura del repositorio:** Breve explicación de la organización de carpetas


- **Tecnologías utilizadas:** Librerías, herramientas, lenguajes
Lenguaje:

- Python

Librerías principales:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

Herramientas:

- Jupyter Notebook
- Git
- GitHub

- **Instrucciones de reproducción:** Cómo ejecutar el código
- **Principales resultados:** Resumen de las métricas y conclusiones
- **Autores:** Nombres y enlaces a perfiles de GitHub



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
