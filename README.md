# 📚 Apuntes de Ciencia de Datos

Repositorio académico de **Miguel Angel Solano Diaz**, estudiante de la **UNIVERSIDAD AUTONOMA DE BUCARAMANGA (UNAB)**, para organizar apuntes, ejercicios y cuadernos de práctica de la materia **Ciencia de Datos**.

El contenido actual se centra en los fundamentos del **perceptrón**, las **redes neuronales artificiales** y el entrenamiento de modelos con **scikit-learn, TensorFlow y Keras**. Combina explicaciones matemáticas, ejemplos en Python y visualizaciones para relacionar la teoría con la práctica.

## Información académica

| Campo | Información |
| --- | --- |
| Estudiante | Miguel Angel Solano Diaz |
| Universidad | UNIVERSIDAD AUTONOMA DE BUCARAMANGA (UNAB) |
| Materia | Ciencia de Datos |
| Repositorio | Apuntes-ciencia-de-Datos |

## Objetivo

Consolidar el aprendizaje de los conceptos y herramientas de ciencia de datos mediante el estudio de modelos de aprendizaje supervisado, la preparación de datos y la implementación de ejercicios de clasificación y regresión.

## Temas de estudio

- **Perceptrón:** entradas, pesos, sesgo, suma ponderada, función escalón y actualización de parámetros.
- **Entrenamiento:** épocas, tasa de aprendizaje, funciones de pérdida y descenso del gradiente.
- **Funciones de activación:** escalón, sigmoide, tangente hiperbólica, función lineal y softmax.
- **Preparación de datos:** exploración con pandas, eliminación de valores nulos, separación de entrenamiento y prueba, y escalado de características.
- **Clasificación con scikit-learn:** entrenamiento de un perceptrón, inspección de sus parámetros y evaluación con exactitud (`accuracy`) y sensibilidad (`recall`).
- **TensorFlow:** tensores, variables, operaciones matemáticas, diferenciación automática con `GradientTape`, grafos y módulos.
- **Keras:** construcción, compilación, entrenamiento, predicción y guardado de un modelo secuencial.
- **Entorno de trabajo:** consulta de paquetes instalados y comprobación de recursos de GPU.

## Guía de contenidos

| Recurso | Contenido |
| --- | --- |
| [Guía teórica del perceptrón](Perceptron/Readme.md) | Explicación de pesos, sesgos, reglas de actualización, errores, descenso del gradiente y funciones de activación. |
| [Cuaderno 1: El perceptrón](Perceptron/Avanzada_Cuaderno_1_ANN_El_Perceptron%20%281%29.ipynb) | Implementación manual y con scikit-learn, usando datos de ejemplo sobre notas de estudiantes; incluye visualización y fronteras de decisión. |
| [Cuaderno 1.1: Perceptrón con scikit-learn](Perceptron/Cuanderno_1_1_Perceptron_con_Sklearn_ipynb%20%281%29.ipynb) | Ejercicio de clasificación con edad y colesterol: limpieza, división de datos, normalización, entrenamiento y evaluación. |
| [Cuaderno 2: TensorFlow y Keras](Perceptron/Avanzada_Cuaderno_2_ANN_Red_Neuronal_sklearn_keras_tensorflow.ipynb) | Operaciones con tensores, cálculo de derivadas y ajuste de una función cuadrática mediante entrenamiento manual y un modelo Keras. |
| [Prueba de GPU](Perceptron/pruebagpu.ipynb) | Consulta de paquetes con `pip list` y del entorno NVIDIA con `nvidia-smi`. |
| [Imágenes de apoyo](imagenes/) | Ilustraciones sobre neuronas, perceptrones, redes multicapa, activaciones y gradiente. |

## Estructura del repositorio

```text
Apuntes-ciencia-de-Datos/
├── README.md
├── Perceptron/
│   ├── Readme.md
│   ├── Avanzada_Cuaderno_1_ANN_El_Perceptron (1).ipynb
│   ├── Cuanderno_1_1_Perceptron_con_Sklearn_ipynb (1).ipynb
│   ├── Avanzada_Cuaderno_2_ANN_Red_Neuronal_sklearn_keras_tensorflow.ipynb
│   └── pruebagpu.ipynb
└── imagenes/
    ├── Readme.md
    ├── ejemplrNN.jpg
    ├── funcion de activacion.jpeg
    ├── gradiente.jpg
    ├── multilayer.jpg
    ├── neurona.jpg
    ├── perceptro.jpeg
    └── step.png
```

## Herramientas utilizadas

| Herramienta | Uso en los cuadernos |
| --- | --- |
| Python | Desarrollo de los ejercicios. |
| NumPy | Operaciones numéricas y arreglos. |
| pandas | Exploración y preparación de datos tabulares. |
| Matplotlib | Gráficas de datos, funciones y predicciones. |
| scikit-learn | Perceptrón, escalado, división de datos y métricas. |
| TensorFlow / Keras | Diferenciación automática y entrenamiento de modelos. |
| SymPy | Cálculo simbólico de derivadas. |
| joblib | Guardado de objetos de aprendizaje automático. |
| Jupyter Notebook / Google Colab | Lectura y ejecución interactiva de los cuadernos. |

## Cómo utilizar el repositorio

### Opción 1: Google Colab

1. Abrir [Google Colab](https://colab.research.google.com/).
2. En el diálogo para abrir un cuaderno, seleccionar **GitHub**.
3. Introducir la URL del repositorio:

   ```text
   https://github.com/Codemikey21/Apuntes-ciencia-de-Datos
   ```

4. Elegir el cuaderno que se desea estudiar.
5. Ejecutar las celdas en orden, revisando las explicaciones y los resultados.

Si falta alguna biblioteca, instalarla en una celda con `%pip install nombre-del-paquete`.

### Opción 2: Ejecución local

Se necesita Git y una versión de Python compatible con las bibliotecas que se vayan a instalar.

**1. Clonar el repositorio:**

```bash
git clone https://github.com/Codemikey21/Apuntes-ciencia-de-Datos.git
cd Apuntes-ciencia-de-Datos
```

**2. Crear un entorno virtual:**

```bash
python -m venv .venv
```

Activarlo en Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

Activarlo en Linux o macOS:

```bash
source .venv/bin/activate
```

**3. Instalar las bibliotecas:**

El repositorio no incluye un archivo `requirements.txt`. Los siguientes comandos reúnen las dependencias utilizadas en los cuadernos y las herramientas para ejecutarlos:

```bash
python -m pip install --upgrade pip
python -m pip install notebook ipykernel numpy pandas matplotlib scikit-learn tensorflow sympy joblib
```

**4. Iniciar Jupyter Notebook:**

```bash
python -m notebook
```

Abrir la carpeta `Perceptron` y seleccionar un cuaderno. Ejecutar las celdas de arriba hacia abajo para crear las variables y modelos en el orden esperado.

## Ruta de estudio sugerida

1. Leer la guía teórica de `Perceptron/Readme.md`.
2. Trabajar el Cuaderno 1 para comprender el perceptrón y su entrenamiento paso a paso.
3. Continuar con el Cuaderno 1.1 para practicar la preparación de datos y la evaluación con scikit-learn.
4. Estudiar el Cuaderno 2 para explorar TensorFlow, las derivadas automáticas y Keras.
5. Usar `pruebagpu.ipynb` como apoyo para inspeccionar el entorno.

## Datos y ejecución de los ejercicios

- El Cuaderno 1 define sus datos de ejemplo directamente en el código.
- El Cuaderno 1.1 descarga `pacientes.csv` desde el [repositorio de datos utilizado en el ejercicio](https://github.com/adiacla/bigdata/blob/master/pacientes.csv), por lo que requiere conexión a Internet. Durante su ejecución puede generar `cardiaco_limpio.csv` y `scaler.joblib`.
- El Cuaderno 2 genera datos sintéticos para estudiar el ajuste de una función cuadrática y contiene instrucciones para guardar modelos.
- Algunas celdas consultan herramientas del sistema, como `nvidia-smi` o `grep`. Pueden omitirse o adaptarse si no están disponibles en el entorno local; no forman parte de la lógica de entrenamiento.
- Las versiones de las dependencias no están fijadas en el repositorio. Las salidas y la compatibilidad pueden variar según el entorno y la inicialización de los modelos.

## Contexto académico y créditos

Este repositorio reúne materiales de estudio y prácticas de **Miguel Angel Solano Diaz** para la materia **Ciencia de Datos** de la **UNIVERSIDAD AUTONOMA DE BUCARAMANGA**.

Los cuadernos incluyen créditos a **Alfredo Alfredo Diaz**, tal como figura en sus encabezados, y referencias a recursos de **adiacla**. Se conservan estas atribuciones como reconocimiento a los materiales utilizados para el aprendizaje.

---

**Miguel Angel Solano Diaz**  
Ciencia de Datos — **UNAB**  
[Repositorio en GitHub](https://github.com/Codemikey21/Apuntes-ciencia-de-Datos)
