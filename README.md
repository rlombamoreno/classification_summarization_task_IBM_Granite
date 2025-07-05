# granite-nlp-lab

Este repositorio contiene ejercicios prácticos realizados en un laboratorio del curso de IBM relacionados con tareas de clasificación de texto y resumen automático, utilizando el modelo **IBM Granite 3.3-8B Instruct** a través de la integración con LangChain y Replicate.

## 🧪 Descripción

Se han desarrollado dos notebooks (`classification_lab1.ipynb` y `classification_lab2.ipynb`) en Google Colab que demuestran el uso de modelos de lenguaje de gran escala (LLMs) para resolver:

- Clasificación de reseñas de clientes (sentimiento y categorías como batería, pantalla, rendimiento)
- Resumen estructurado de reuniones de negocio (puntos clave, decisiones, acciones)

## 🧰 Tecnologías utilizadas

- 🧠 [IBM Granite 3.3-8B Instruct](https://huggingface.co/ibm-granite)
- 🔗 [LangChain Community](https://python.langchain.com/)
- 🧪 [Replicate API](https://replicate.com/)
- 🐍 Python 3 en [Google Colab](https://colab.research.google.com/)

## 📄 Archivos

| Archivo | Descripción |
|--------|-------------|
| `classification_lab1.ipynb` | Primer laboratorio. Ejemplos básicos de clasificación y resumen sin parámetros personalizados. |
| `classification_lab2.ipynb` | Segundo laboratorio. Incluye parametrización avanzada del modelo (top_k, top_p, max_tokens, etc.) para mejorar el control del output. |

## 🔐 Autenticación

Ambos notebooks requieren el uso de un token de Replicate, el cual debe almacenarse en las variables del entorno seguro de Google Colab (`userdata`).

```python
from google.colab import userdata
api_token = userdata.get('api_token')
