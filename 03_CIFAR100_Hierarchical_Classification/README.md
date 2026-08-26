# Optimización de Clasificación Jerárquica en CIFAR-100 📊

**Autor:** Gonzalo Cazorla Sánchez

## 🎯 Objetivo del Proyecto
Estudiar si la información jerárquica de las etiquetas gruesas (20 superclases) puede mejorar el rendimiento de un sistema de clasificación sobre etiquetas finas (100 clases) en el dataset CIFAR100.

## 🧠 Arquitectura y Conceptos Clave
* **Comparativa de Modelos:** Entrenamiento de un modelo base (Modelo A) directo a 100 clases y un modelo auxiliar (Modelo B) enfocado en las 20 superclases.
* **Probabilidad Condicionada:** Formulación matemática del modelo asistido utilizando la regla de la cadena P(A) = P(A|B) / P(B), donde P(B) proviene del Modelo B y P(A|B) se obtiene renormalizando las predicciones del Modelo A.
* **Análisis de Propagación de Errores:** El proyecto concluye analíticamente por qué el enfoque combinado no superó al *baseline*. Se documenta cómo la multiplicación de probabilidades propaga errores catastróficos si el modelo de superclases falla, y cómo el ruido en la renormalización sabotea los aciertos directos.
