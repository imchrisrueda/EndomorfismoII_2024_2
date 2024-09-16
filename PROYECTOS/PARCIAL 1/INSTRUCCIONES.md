# PROYECTO DEL PRIMER PARCIAL

Las líneas de transmisión son fundamentales para el sistema eléctrico trifásico, ya que permiten llevar la energía desde la fuente hasta la red de distribución. Sin embargo, estos sistemas están expuestos a perturbaciones y fallas eléctricas, lo que hace necesario detectar y clasificar rápidamente dichas fallas para garantizar la estabilidad del sistema.

Para este proyecto, se propone que los estudiantes utilicen modelos de aprendizaje no lineal como máquinas de soporte vectorial (SVM) y árboles de decisión (DT) para la clasificación de fallas. Estos modelos permiten realizar una clasificación eficiente de las fallas en el sistema eléctrico, lo que es crucial para mantener la estabilidad del sistema.

## Descripción del dataset

Se incluyen tanto los valores de las corrientes de línea como los voltajes de las tres fases del sistema. A continuación, se detalla el contenido del dataset:

    Entradas (Inputs):
        Ia, Ib, Ic: Corrientes de las líneas A, B y C, respectivamente.
        Va, Vb, Vc: Voltajes de las líneas A, B y C, respectivamente.

    Salidas (Outputs):
        El dataset clasifica los tipos de fallas utilizando una matriz de salida [G C B A], donde los valores binarios indican la ocurrencia de una falla en diferentes fases o con el neutro. Las combinaciones posibles son:
            [0 0 0 0]: Sin falla.
            [1 0 0 1]: Falla entre la fase A y tierra (LG - Línea a tierra).
            [0 0 1 1]: Falla entre las fases A y B (LL - Línea a línea).
            [1 0 1 1]: Falla entre las fases A, B y tierra (LLG - Línea a línea a tierra).
            [0 1 1 1]: Falla entre las tres fases (LLL - Línea a línea a línea).
            [1 1 1 1]: Falla trifásica simétrica entre las tres fases y tierra (LLLG - Línea a línea a línea a tierra).

El objetivo del dataset es identificar el tipo de falla eléctrica basado en los valores medidos de corriente y voltaje en cada fase del sistema. Esta información permite clasificar adecuadamente las fallas y aplicar los mecanismos de protección necesarios.

## Entregables

### Informe sobre el desarrollo del trabajo (.pdf)
Documento en formato artículo (Se anexa ejemplo). Extensión máxima: 3 hojas.
### Notebook de Python (.ipynb)
Código en el que se muestre todo el trabajo desarrollado. Use adecuadamente las secciones de código y de texto. 
-Aplicar técnicas de aprendizaje automático no lineal para resolver problemas de ingeniería mecatrónica, justificando la selección de modelos y técnicas específicas
### Archivo del mejor modelo entrenado
Archivo en cualquiera de los formatos posibles.
Más información: https://machinelearningmastery.com/save-load-machine-learning-models-python-scikit-learn/ 

## Evaluación (100%)
### Mejor modelo entrenado (50%)
El archivo de mejor modelo entrenado se cargará y validará con un conjunto no visto de datos. La métrica usada será la exactitud. La exactitud más alta alcanzada por cualquier equipo del curso será el referente para el máximo de la nota. El resto de valores logrados por los demás estudiantes se ponderarán de acuerdo a esta lógica.

#### Ponderación Funciona - 100%   No funciona - 50%
### Artículo (20%)
Presentación del artículo en el formato solicitado. 

### Notebook de Python (30%)
Originalidad del código presentado. Código y explicación del desarrollo de la solución.



# Evaluación del componente: Gestión del aprendizaje P1 (12%)
## Caso práctico - 60%
## Examen teórico - 40%


¡Éxitos en su trabajo!
