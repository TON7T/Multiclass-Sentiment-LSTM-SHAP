# Multiclass-Sentiment-LSTM-SHAP
Deep learning para análisis de sentimientos multiclase en inglés, usando redes LSTM, embeddings FastText y explicaciones con SHAP. Incluye búsqueda de hiperparámetros exhaustiva y visualización de interpretabilidad.

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
├── data/                     # Conjuntos de datos (limpios y raw)
├── notebooks/                # Cuadernos de exploración y visualización
├── models/                   # Entrenamiento y arquitectura del modelo
├── shap_analysis/            # Resultados e interpretabilidad
├── utils/                    # Funciones auxiliares
├── results/                  # Reportes, gráficos y métricas finales
├── requirements.txt          # Dependencias del proyecto
├── README.md                 # Este archivo
└── LICENSE                   # Licencia (MIT por defecto)
