# Representación Neuronal Implícita (INR) para Superresolución de Imágenes 🖼️

**Autor:** Gonzalo Cazorla Sánchez

## 🎯 Objetivo del Proyecto
Entrenar un modelo de redes neuronales (Perceptrón Multicapa o MLP) capaz de aprender la representación espacial de una imagen (coordenadas a colores) para reproducirla sin necesidad de la imagen original y lograr escalarla a una resolución mayor (de 35x30 a 70x60).

## 🧠 Arquitectura y Conceptos Clave
* **Codificación Posicional (Positional Encoding):** Los MLPs clásicos tienen dificultades para aprender variaciones de alta frecuencia (cambios bruscos de color). Para solucionarlo, se implementó un codificador que descompone las coordenadas de entrada en diversas frecuencias utilizando funciones seno y coseno.
* **Resolución del Overfitting:** Durante el escalado de la imagen a 70x60, el modelo inicialmente generaba ruido al intentar interpolar puntos que no había visto. Se diagnosticó como un problema de sobreajuste por memorización de coordenadas discretas.
* **Regularización por Frecuencia:** La solución consistió en reducir el parámetro de bandas de frecuencia del codificador posicional (`L=5`). Al limitar las altas frecuencias, se forzó a la red a aprender una función de color más suave y continua, logrando una interpolación perfecta para la superresolución.
