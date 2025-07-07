# Multiclass-Sentiment-LSTM-SHAP

Análisis de sentimientos multiclase en textos en inglés utilizando redes neuronales recurrentes (LSTM bidireccional), embeddings preentrenados (FastText) y técnicas de interpretabilidad como SHAP. Este repositorio contiene todo el flujo de trabajo, desde la preparación de datos hasta el análisis explicativo de los resultados.

---

## 📌 Descripción del proyecto

Este proyecto aborda la clasificación automática de sentimientos en seis categorías emocionales: **sadness**, **joy**, **love**, **anger**, **fear** y **surprise**. Se construyó un modelo profundo que combina:

- Embeddings preentrenados (FastText, 300 dimensiones)
- LSTM bidireccional para capturar contexto secuencial
- Búsqueda sistemática sobre 2 592 combinaciones de hiperparámetros
- Visualización de importancia por posición y tokens mediante SHAP

El modelo final alcanza una **precisión del 94 %** en el conjunto de prueba.

---

## 🗃️ Origen de los datos

El conjunto de datos utilizado en este proyecto proviene del repositorio de Kaggle:

> 📥 https://www.kaggle.com/datasets/nelgiriyewithana/emotions/data

Este dataset contiene textos en inglés etiquetados con seis categorías emocionales: sadness, joy, love, anger, fear y surprise.


## 🧠 Tecnologías utilizadas

- Python 3.10+
- TensorFlow 2.x
- NumPy / Pandas / Matplotlib
- Gensim (para FastText)
- SHAP (interpretabilidad)
- Scikit-learn (evaluación)

---

🧠 Aplicación interactiva de clasificación emocional

Se ha desarrollado una aplicación interactiva que permite al usuario ingresar una frase y obtener:

- La emoción detectada con su respectivo nivel de confianza.
- Una visualización de las probabilidades asignadas por el modelo a cada clase emocional.
- Una explicación detallada con valores SHAP que muestran la importancia de cada token en la predicción.
- Una simulación de atención basada en los valores SHAP, indicando qué palabras influyeron más.
- Una representación del espacio de embeddings del texto ingresado.

👉 En esta aplicación se encuentra embebido el modelo entrenado y todos los recursos necesarios para utilizarlo como un **intérprete de emociones transparente y explicable**.

🔗 Puedes acceder a la aplicación aquí:

---

## 📁 Estructura del repositorio

```plaintext

├── Trabajo_Titulacion/       # Entrenamiento y arquitectura del modelo
├── requirements.txt          # Dependencias del proyecto
├── README.md                 # Este archivo
├── data/                     # App para usarla en producción


