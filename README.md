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
Una vez desplegada, la API se pudo probar en: https://fe6b-34-150-163-63.ngrok-free.app/predecir/

## 🛠️ Flujo de trabajo
1. Preprocesamiento y escalado de datos
3. Entrenamiento del modelo Random Forest
4. Guardado del modelo y el escalador
5. Implementación de una API REST con FastAPI
6. Exposición pública de la API usando pyngrok
![image](https://github.com/user-attachments/assets/58e73c00-94bb-49d2-a532-47e18805c99a)
![image](https://github.com/user-attachments/assets/9b7f4358-02b5-4670-aa31-7a828afca1cc)
![image](https://github.com/user-attachments/assets/68af512a-3df6-406c-a7ca-c4a4287b1caf)
8. Pruebas con Postman y documentación Swagger
Primera solicitud desde postman: Tipo de vino 0 (alta intensidad de color y flavonoides)
![image](https://github.com/user-attachments/assets/d058a703-90d3-40a0-9718-f7e59457dc8e)

Segunda solicitud desde postman: Tipo de vino 1 (bajo contenido fenólico)
![image](https://github.com/user-attachments/assets/eb2d8b04-ca5b-41e2-ae19-699af7ee7595)

Tercera solicitud desde postman: Tipo de vino 2 (alto contenido de alcohol y color)
![image](https://github.com/user-attachments/assets/e1148303-1d8c-4d74-a300-afd60ea03997)
![image](https://github.com/user-attachments/assets/0a6b320a-2ec3-4b91-9444-8c0339bd6c60)



