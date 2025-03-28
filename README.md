# FastAPI-para-modelos-de-ML
Despliegue de un Modelo de Clasificación con FastAPI usando el Dataset de Vinos

Este proyecto implementa el despliegue de un modelo de clasificación (`RandomForestClassifier`) entrenado con el dataset `wine` de Scikit-learn. El modelo predice el tipo de vino en base a 13 características químicas. Cabe resaltar que para nuestro dataset existen 3 tipos de vino, o 3 categorías (0, 1, 2) que representan diferentes tipos de cepas de uva (cultivares), y no marcas comerciales. El objetivo es predecir la cepa del vino a partir de mediciones químicas como alcohol, acidez málica, intensidad del color, flavonoides, entre otras.

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
Una vez desplegada, la API se pudo probar en: [https://fe6b-34-150-163-63.ngrok-free.app/predecir/](https://b4cd-34-150-163-63.ngrok-free.app/predecir/)

## 🛠️ Flujo de trabajo
1. Preprocesamiento y escalado de datos
3. Entrenamiento del modelo Random Forest
4. Guardado del modelo y el escalador

![image](https://github.com/user-attachments/assets/049191dc-a8ab-4938-b174-3a1b6a87212e)

6. Implementación de una API REST con FastAPI
7. Exposición pública de la API usando pyngrok

![image](https://github.com/user-attachments/assets/b4963720-e5e4-4ca7-955c-51d60255c496)

![image](https://github.com/user-attachments/assets/75ca8249-0e1e-4f46-b947-9b464001cc53)

![image](https://github.com/user-attachments/assets/577a68aa-2f8f-49f6-8fab-9f75fa805fd0)

8. Pruebas con Postman
Después de hacer el respectivo endpoint se hacen diferentes tipos de soolicitudes con el fin de
conocer si el modelo de random forest llega a predecir de manera clara y efectiva el tipo de vino.
  - Primera solicitud desde postman: Tipo de vino 0 (alta intensidad de color y flavonoides)
![image](https://github.com/user-attachments/assets/7c3c245c-5407-4512-9c82-8ffb1d084eaf)

  - Segunda solicitud desde postman: Tipo de vino 1 (bajo contenido fenólico)
![image](https://github.com/user-attachments/assets/85d687c4-76c1-443b-a9ca-f36d3d08f8cc)

- Tercera solicitud desde postman: Tipo de vino 2 (alto contenido de alcohol y color)
![image](https://github.com/user-attachments/assets/45e6df25-d8d7-4337-b841-60edeeba8f72)

- Cuarta solicitud desde postman:
![image](https://github.com/user-attachments/assets/189bd621-05e9-4d19-89ac-a0619d8ce9bc)

Vista final desde el Colab
![image](https://github.com/user-attachments/assets/f066c7e6-6815-4da2-932d-fb03ee4dcf5e)
