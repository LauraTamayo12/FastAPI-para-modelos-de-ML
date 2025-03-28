# FastAPI-para-modelos-de-ML
Despliegue de un Modelo de Clasificación con FastAPI usando el Dataset de Vinos

Este proyecto implementa el despliegue de un modelo de clasificación (`RandomForestClassifier`) entrenado con el dataset `wine` de Scikit-learn. El modelo predice el tipo de vino en base a 13 características químicas.

## Tecnologías usadas

- Python
- Scikit-learn
- FastAPI
- Uvicorn
- Pyngrok
- Google Colab

## 🎯 Objetivo
Convertir un modelo de Machine Learning en un **servicio web accesible** mediante una **API REST** usando FastAPI.

## 🔧 Problema y solución
Se utilizó **`pyngrok`** para crear un **túnel público** que expone la API de forma segura y accesible desde cualquier navegador o herramienta como Postman.

## 🌐 API Endpoint
Una vez desplegada, la API se pudo probar en: https://d641-34-150-163-63.ngrok-free.app/pedecir/

## 🛠️ Flujo de trabajo
1. Preprocesamiento y escalado de datos
3. Entrenamiento del modelo Random Forest
4. Guardado del modelo y el escalador
5. Implementación de una API REST con FastAPI
6. Exposición pública de la API usando pyngrok
![image](https://github.com/user-attachments/assets/3223ece9-bdd5-44d4-b903-e8d64250ec10)
8. Pruebas con Postman y documentación Swagger
![image](https://github.com/user-attachments/assets/b1fd52fb-efe1-4b97-ad07-db5a213924fc)



---

## 📂 Estructura del repositorio


