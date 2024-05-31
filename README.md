# Caso Práctico: Neurona de McCulloch y Pitts

Este caso práctico ilustra el funcionamiento de una neurona de McCulloch y Pitts (MPNeuron), que es uno de los modelos más simples de neuronas artificiales. Esta neurona funciona sumando las entradas y comparando el resultado con un umbral predefinido para tomar una decisión binaria.

## 1. Implementación de la MPNeuron

### Inicialización

La clase MPNeuron se inicializa sin un umbral (threshold) definido. Este umbral es el valor con el que se compara la suma de las entradas para determinar la salida de la neurona.

### Modelo

El modelo de la neurona suma los valores de las entradas binarias. Si la suma es mayor o igual al umbral, la salida es `True` (indicando activación), de lo contrario, la salida es `False`.

### Predicción

La función de predicción evalúa una lista de entradas, utilizando el modelo definido. Para cada conjunto de entradas, calcula la suma y compara con el umbral para determinar la salida.

### Ejemplo de Uso

Se instanció la neurona y se estableció un umbral de 4. Luego, se evaluaron diferentes casos de uso:

- `[1, 0, 0, 0]`: La suma es 1, que es menor que el umbral de 4, por lo que la salida es `False`.
- `[1, 1, 1, 1]`: La suma es 4, que es igual al umbral, por lo que la salida es `True`.
- `[1, 1, 1, 0]`: La suma es 3, que es menor que el umbral, por lo que la salida es `False`.

La salida final para estos conjuntos de entradas es un array con los valores `[False, True, False]`.

Este ejemplo demuestra cómo una neurona de McCulloch y Pitts puede utilizarse para tomar decisiones binarias simples basadas en un conjunto de entradas binarias y un umbral predefinido. Esta neurona es la base para la construcción de redes neuronales más complejas, que pueden aprender a partir de datos y realizar tareas más sofisticadas.
