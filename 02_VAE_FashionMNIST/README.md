# Generación de Imágenes y Morphing con Variational Autoencoders (VAE) 👕

**Autor:** Gonzalo Cazorla Sánchez

## 🎯 Objetivo del Proyecto
Diseñar y entrenar un *Variational Autoencoder* (VAE) aplicado al conjunto de datos Fashion-MNIST para la generación de imágenes sintéticas a partir de un espacio latente probabilístico de 8 dimensiones.

## 🧠 Arquitectura y Conceptos Clave
* **Truco de Reparametrización:** Implementación matemática que permite la retropropagación del error muestreando desde una distribución normal estándar.
* **Divergencia Kullback-Leibler (KL):** Desarrollo de una función de pérdida personalizada que combina el error de reconstrucción (MSE) con la divergencia KL, penalizando las distribuciones que se alejan de una normal estándar regularizada N(0, 1).
* **Vectores Prototípicos e Interpolación (Morphing):** Extracción de la media de los vectores latentes para cada clase (p. ej., "Camiseta" y "Pantalón") del conjunto de test. Mediante interpolación lineal (`torch.lerp`) entre estos vectores, el modelo decodifica y genera una transición fluida y continua transformando una prenda en otra.
