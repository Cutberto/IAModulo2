# Clasificador de imagenes con deep learning

Este proyecto consiste en un clasificador binario de imagenes utilizando Deep Learning.
El dataset consiste en imagenes de osos y pandas, constando de 250 imagenes de cada clase para entrenamiento y 50 imagenes de cada clase para pruebas.

## 19/05/2023

Se carga la versión inicial del código, la cual contiene el código para cargar a memoria el dataset y aplicar data augmentation para tener una mayor cantidad de muestras para cada categoría, y de esta forma ayudar a que el modelo sea capaz de reconocer los animales en situaciones diferentes a las incluidas en el dataset original.

Se incluye además una red neuronal simple para verificar el correcto funcionamiento del data augmentation.

## 26/06/2023

Se incluye una implementación del modelo MobileNetV2 usando Transfer learning.
