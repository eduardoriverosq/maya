# [Pre-print] Redes Neuronales Discretas Basadas en la Lógica Posicional Vigesimal Maya: Un Enfoque Alternativo para la Detección de Spam

[![DOI](https://zenodo.org)](https://doi.org)

**Autor:** Eduardo Riveros Quiroz  
**Campo de Estudio:** Etnocomputación / Computación Cognitiva / Inteligencia Artificial Alternativa  
**Estado del Proyecto:** Versión de Desarrollo / Prueba de Concepto en Progreso  

---

## 📜 Resumen (Abstract)
Este proyecto de Ciencia Abierta presenta una arquitectura alternativa de red neuronal que sustituye el procesamiento lineal continuo en base decimal o binaria tradicional por la estructura posicional vertical y acumulación vigesimal (base 20) de las matemáticas mayas. Como caso de estudio y validación práctica, se implementa un modelo de clasificación para el filtrado de correo no deseado (Spam). El objetivo central es demostrar que los sistemas numéricos prehispánicos poseen propiedades algorítmicas discretas viables para optimizar la tokenización, el empaquetado de pesos y la convergencia de modelos de Machine Learning contemporáneos.

---

## 🏛️ 1. Introducción y Marco Teórico
Las arquitecturas de Inteligencia Artificial modernas dependen críticamente del hardware optimizado para procesar matrices complejas de números flotantes (punto flotante de 32 o 16 bits). Este paradigma, aunque eficiente a nivel de silicio, hereda las limitaciones conceptuales de la continuidad matemática occidental.

Este marco de trabajo explora la **Etnomatemática aplicada**, recuperando los tres pilares del sistema de numeración maya:
1. **La Concha / Caracol (0):** Operando como un estado nulo de inhibición absoluta en el nodo.
2. **El Punto (1):** Definido como la unidad cuántica mínima de ajuste de peso.
3. **La Barra (5):** Actuando como un vector de acumulación rápida y activación por bloques.

La naturaleza posicional vertical de la matemática maya (potencias de $20^n$) se homologa directamente con las capas jerárquicas de una red neuronal, donde la información es cuantizada y forzada a "ascender" de nivel de orden solo al superar el umbral vigesimal.

---

## 🛠️ 2. Metodología y Arquitectura del Modelo

### 2.1 Tokenización Vigesimal (Capa de Entrada)
A diferencia de los enfoques tradicionales (TF-IDF o Embeddings densos continuos), el texto de los correos electrónicos entrantes se codifica mediante un mapa de frecuencia discreto. Las palabras se convierten a valores numéricos enteros expresados en base 20, segmentando su relevancia posicional según su orden vertical.

### 2.2 Cuantización de Pesos mediante Simbología Neo-Maya
Los pesos ($W$) y sesgos ($b$) de las neuronas se restringen de forma estricta a valores discretos que emulan las combinaciones de puntos y barras. Esto reduce el espacio de estados continuo de la red a una cuadrícula geométrica regular de base 20, permitiendo estudiar el comportamiento de la convergencia bajo restricciones algebraicas distintas a las de una red neuronal tradicional.

### 2.3 Función de Activación por Umbrales Mayas
Se descartan las funciones sigmoides continuas en las capas intermedias, sustituyéndolas por una función escalonada basada en múltiplos críticos de 20. La neurona solo transmite el potencial de acción hacia el siguiente nivel si el acumulador supera el umbral del orden vigesimal correspondiente.

---

## 📊 3. Diseño del Experimento y Comparativa (Benchmark)
Para validar la relevancia de esta novedad técnica, el repositorio incluye un script de prueba automatizado que ejecuta en paralelo dos configuraciones utilizando el mismo corpus de datos de spam:

1. **Modelo de Control (Tradicional):** Red neuronal simple con optimización estándar en Python.
2. **Modelo Experimental (Maya):** Red neuronal cuantizada bajo la lógica vigesimal posicional.

### Variables de Medición
Los resultados finales del entrenamiento local se registrarán en los siguientes ejes métricos:

| Métrica Evaluada | Enfoque Tradicional (Base 10 / Binario) | Enfoque Vigesimal Maya (Base 20) |
| :--- | :--- | :--- |
| **Precisión General (Accuracy)** | *Por registrar* | *Por registrar* |
| **Tasa de Falsos Positivos** | *Por registrar* | *Por registrar* |
| **Épocas para Convergencia** | *Por registrar* | *Por registrar* |
| **Uso de Memoria (Pesos Discretos)**| *Por registrar* | *Por registrar* |

---

## 🚀 4. Reproducibilidad y Ejecución
Para replicar el experimento en entornos de desarrollo locales:

```bash
# Clonar el repositorio
git clone https://github.com

# Ingresar al directorio
cd red-neuronal-maya-spam

# Ejecutar el benchmark comparativo
python ejecutar_comparativa.py
```

---

## 📜 5. Licencia y Preservación Científica
Este código se distribuye bajo la licencia **GNU General Public License v3.0 (GPL-3.0)**, garantizando que cualquier iteración, mejora o bifurcación de este algoritmo permanezca libre, abierta y de acceso público para la humanidad, respetando la autoría original de esta metodología.

---
## ✒️ Cómo Citar este Trabajo
Si utilizas esta metodología o fragmentos de este código en investigaciones académicas de etnomatematica o computación alternativa, por favor utiliza la siguiente estructura de citación (Zenodo):

> **Riveros Quiroz, E.** (2026). *Redes Neuronales Discretas Basadas en la Lógica Posicional Vigesimal Maya: Un Enfoque Alternativo para la Detección de Spam*. Zenodo. https://doi.org

