# Portfolio de Deep Learning & Inteligencia Artificial 🧠

**Autor:** Gonzalo Cazorla Sánchez[cite: 10, 11, 12]

Bienvenido a mi portfolio de Inteligencia Artificial. Este repositorio agrupa mis proyectos académicos más destacados en los campos de Visión Artificial, Modelos Generativos y Representaciones Neuronales, desarrollados en Python utilizando PyTorch[cite: 10, 11, 12]. 

Cada proyecto no solo aborda la implementación del código, sino que incluye un fuerte componente analítico para diagnosticar y solucionar problemas matemáticos y arquitectónicos en redes neuronales profundas.

## 📌 Proyectos Destacados

### 1. Representación Neuronal Implícita (INR) para Superresolución
* **Directorio:** [`01_INR_Image_Superresolution`](./01_INR_Image_Superresolution)[cite: 10]
* **Descripción:** Desarrollo de un modelo neuronal (Perceptrón Multicapa) diseñado para aprender y reconstruir representaciones espaciales de imágenes[cite: 10]. 
* **Hitos técnicos:** Implementación de un módulo de *Positional Encoding* para permitir el aprendizaje de variaciones de alta frecuencia[cite: 10]. Resolución analítica del problema de *overfitting* espacial mediante el ajuste de bandas de frecuencia, logrando una interpolación continua exitosa al duplicar la resolución original[cite: 10].

### 2. Generación de Imágenes con Variational Autoencoders (VAE)
* **Directorio:** [`02_VAE_FashionMNIST`](./02_VAE_FashionMNIST)[cite: 11]
* **Descripción:** Diseño, entrenamiento y evaluación de un Variational Autoencoder (VAE) aplicado al conjunto de datos Fashion-MNIST.
* **Hitos técnicos:** Uso de la Divergencia de Kullback-Leibler (KL) como técnica de regularización matemática del espacio latente probabilístico[cite: 11]. El proyecto incluye la extracción de vectores prototípicos por clase y la generación de nuevas imágenes sintéticas mediante técnicas de interpolación lineal (*morphing*) continua entre categorías[cite: 11].

### 3. Optimización de Clasificación Jerárquica en Computer Vision
* **Directorio:** [`03_CIFAR100_Hierarchical_Classification`](./03_CIFAR100_Hierarchical_Classification)[cite: 12]
* **Descripción:** Sistema de clasificación entrenado sobre el dataset CIFAR100, aprovechando su etiquetado estructurado en 100 clases finas y 20 superclases gruesas[cite: 12].
* **Hitos técnicos:** Análisis comparativo exhaustivo entre un modelo de clasificación base y un modelo asistido por probabilidad condicionada[cite: 12]. El estudio profundiza en la formulación matemática a través de la regla de la cadena ($P(A) = P(A|B) \times P(B)$) y documenta extensamente el fenómeno de la propagación de errores e inestabilidad numérica entre la red de superclases y la red de clases finas[cite: 12].

## 🛠️ Tecnologías y Herramientas
* **Lenguaje:** Python[cite: 10, 11, 12]
* **Framework Principal:** PyTorch[cite: 10, 11, 12]
* **Librerías Adicionales:** Torchvision, NumPy, Matplotlib, Scikit-learn, tqdm[cite: 10, 11, 12]

---
*Proyectos desarrollados como parte de la asignatura Programación para la Inteligencia Artificial, dirigida por Jorge García González.*[cite: 10]
