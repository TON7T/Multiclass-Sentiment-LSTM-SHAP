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

## 📁 Estructura del repositorio

```plaintext
.
├── Trabajo_Titulacion/       # Entrenamiento y arquitectura del modelo
├── requirements.txt          # Dependencias del proyecto
├── README.md                 # Este archivo
├── data/                     # App para usarla en producción


