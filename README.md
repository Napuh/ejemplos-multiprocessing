# Ejemplos de Procesamiento Paralelo en Python

Este repositorio contiene ejemplos educativos que demuestran conceptos de procesamiento paralelo en Python utilizando diversos enfoques. Cada ejemplo compara implementaciones secuenciales (un solo hilo) versus paralelas para mostrar mejoras de rendimiento.

## Ejemplos

### 1. Integración Numérica (`integral.ipynb`)
- Calcula la integral definida de f(x) = x² desde 0 hasta 10

### 2. Conjunto de Mandelbrot (`mandelbrot.ipynb`)
- Genera el famoso fractal del conjunto de Mandelbrot

### 3. Multiplicación de Matrices (`multiplicacion_matrices.ipynb`)
- Implementa multiplicación de matrices de diferentes maneras:
  - Implementación secuencial
  - Implementación paralela usando multiprocesamiento
  - Implementación con NumPy
  - Implementación con PyTorch (CPU y GPU)
- Compara rendimiento entre diferentes implementaciones

### 4. Suma de Cuadrados (`suma_cuadrados.ipynb`)
- Calcula la suma de cuadrados para una lista de números

### 5. Suma de Vectores (`suma_vector.ipynb`)
- Realiza la suma de dos vectores grandes

## Conceptos

- Procesamiento paralelo básico usando el módulo `multiprocessing` de Python
- Distribución de trabajo entre múltiples núcleos de CPU usando `Pool`
- Comparación de rendimiento entre implementaciones secuenciales y paralelas
- Integración con bibliotecas especializadas (NumPy, PyTorch)
- Aceleración por GPU

## Ejercicio a implementar:

- Calcular que posiciones de una lista contiene números primos.

Dada una lista de entrada, indicar que posiciones de la lista corresponden a números primos:

```python
entrada = [1, 2, 3, 4, 5, 6]
salida = [False, True, True, False, True, False]
```

1. Implementar la función `is_primo(n: int) -> bool`. 
2. Implementar una versión secuencial del programa.
3. Implementar una versión paralela del programa.
4. Preguntas:

- Para tamaños de entrada pequeños (<1000), ¿qué versión es más rápida?
- Para tamaños de entrada grandes (>100k), ¿qué versión es más rápida?
- ¿Porqué?
- ¿A partir de qué tamaño comienza a merecer la pena la versión paralela?

## Notas

- Los resultados de rendimiento pueden variar según las especificaciones del hardware
- Algunos ejemplos pueden funcionar mejor o peor con procesamiento paralelo dependiendo del tamaño de entrada
- La aceleración por GPU requiere hardware compatible y una instalación adecuada de PyTorch