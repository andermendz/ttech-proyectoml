# 🤖 Modelo de Predicción de Aprobación de Microcréditos

Este proyecto contiene un modelo de Machine Learning desarrollado en Python para predecir la probabilidad de que un solicitante sea aprobado para un microcrédito. El proceso completo, desde la generación de datos simulados hasta el despliegue de una interfaz web interactiva, se encuentra documentado en un único notebook de Google Colab.

## 📊 Demo de la Interfaz

Al ejecutar el notebook, se despliega una interfaz web creada con Gradio que permite interactuar con el modelo de forma sencilla:

| Parámetro de Entrada | Tipo de Control |
| :--- | :--- |
| **Ingresos Mensuales ($)** | Campo numérico |
| **Deuda Actual Total ($)** | Campo numérico |
| **Años de Experiencia** | Deslizador (Slider) |
| **Historial Crediticio** | Botones de opción (Radio) |
| **Nivel Educativo** | Menú desplegable (Dropdown) |
| **Edad** | Deslizador (Slider) |

Al hacer clic en el botón **"Analizar Solicitud y Predecir"**, el modelo devuelve dos resultados:
1.  **Resultado de la Predicción**: ✅ APROBADO o ❌ NO APROBADO.
2.  **Confianza**: El nivel de probabilidad con el que el modelo emite su predicción.

## ✨ Características

*   **Generación de Datos**: Incluye un script para crear un dataset simulado y reproducible con `numpy` y `pandas`.
*   **Análisis Exploratorio (EDA)**: Visualizaciones con `matplotlib` y `seaborn` para entender la distribución y relación de las variables.
*   **Preprocesamiento**: Codificación de variables categóricas (`nivel_educativo`) a numéricas usando `scikit-learn`.
*   **Entrenamiento de Modelos**: Se entrenan y comparan dos algoritmos de clasificación:
    1.  **Regresión Logística**: Un modelo lineal robusto.
    2.  **Árbol de Decisión**: Un modelo no lineal e interpretable.
*   **Evaluación del Modelo**: El rendimiento se mide con métricas como **Accuracy** y una **Matriz de Confusión**.
*   **Interfaz Interactiva**: Se utiliza la librería `Gradio` para desplegar una demo funcional directamente desde el notebook.

## 🛠️ Tecnologías Utilizadas

*   **Lenguaje**: Python 3
*   **Librerías Principales**:
    *   `pandas`: Manipulación y análisis de datos.
    *   `numpy`: Soporte para operaciones numéricas.
    *   `scikit-learn`: Para el modelado de Machine Learning (entrenamiento, división de datos, métricas).
    *   `matplotlib` & `seaborn`: Visualización de datos.
    *   `Gradio`: Para crear y desplegar la interfaz de usuario web.
*   **Entorno**: Google Colab.

## 🚀 Instalación y Ejecución

El proyecto está diseñado para ejecutarse en Google Colab, lo que elimina la necesidad de instalaciones locales.

1.  **Clonar el repositorio (Opcional):**
    ```bash
    git clone https://github.com/TU_USUARIO/TU_REPOSITORIO.git
    ```

2.  **Abrir en Google Colab:**
    *   Ve a [Google Colab](https://colab.research.google.com/).
    *   Haz clic en `Archivo` > `Subir notebook...` y selecciona el archivo `.ipynb` de este repositorio.

3.  **Ejecutar el Notebook:**
    *   Una vez abierto, puedes ejecutar todas las celdas de una vez haciendo clic en `Entorno de ejecución` > `Ejecutar todas`.
    *   La librería `Gradio` se instalará automáticamente si no está presente.

4.  **Interactuar con la Demo:**
    *   Desplázate hasta la última celda. La interfaz de Gradio aparecerá en la salida, lista para usar.

## 📂 Estructura del Proyecto

El proyecto se concentra en un único archivo para simplicidad y portabilidad:

```
.
└── microcredit_prediction_model.ipynb
```

## 🎯 Resultado Final

El objetivo de este proyecto es entregar dos productos clave:
1.  **Un notebook de Google Colab limpio y comentado** que sirve como un registro completo del proceso de desarrollo del modelo.
2.  **Un modelo funcional** accesible a través de una interfaz simple, demostrando una solución de extremo a extremo (end-to-end).
