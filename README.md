# Curso de Entorno de Trabajo para Ciencia de Datos con Jupyter Notebooks y Anaconda

## Introducción a las Notebooks

### ¿En qué lugares programar para ciencia de datos?

Notebooks vs Scripts

- Ambos son útiles
- La organización es distinta
  - Script: Puedes ver lo que el programador quiso escribir.
  - Notebook: Está un poco más orientado a presentar tus resultados, experimentar.

### Google Colab: primeros pasos

Google Colab nos da acceso gratuito a GPU y TPU.

Además de poder escribir código, markdown e insertar imágenes, también podemos escribir comandos de UNIX. Solamente debemos escribir al inicio el símbolo '!'.

### Google Colab: ciencia de datos

Librerías para Ciencia de Datos

- 📊 matplotlib: Generación de gráficos a partir de listas o arrays.
- 🧑‍💻 numpy: Cómputo científico para la manipulación de vectores.
- 🧑‍💻 pandas: Manipulación y análisis de datos de tablas y series temporales.
- 🧑‍💻 scipy: Herramientas y algoritmos matemáticos.
- 📊 seaborn: Visualización de datos estadísticos.

Podemos usar archivos de nuestra computadora en Colab. Sin embargo, cuando pase cierto tiempo de que no estemos usando el archivo, este será eliminado.

Pero para poder tener los archivos de manera persistente, debemos guardar los archivos en Google Drive y acceder a ellos desde Google Colab.

Luego, podemos por ejemplo hacer: `!cat drive/MyDrive/nombreArchivo.csv`

Google Colab ya cuenta con algunos códigos a modo de ejemplo, los encontramos en la parte de la izquierda, en 'Scripts' o 'Fragmentos de código'.

Para entrar a los atajos de teclado: `control shift p` y escribes 'Shortcuts' o 'Atajos de teclado'.

### Utilizar Deepnote

[Deepnote](https://deepnote.com/) es como Google Colab, sin embargo, este último trabaja a nivel de *archivo*, mientras que Deepnote trabaja a nivel de *proyecto*.

## Quiz 1

- ¿En qué sistemas operativos puedo hacer ciencia de datos? -> Windows, MacOS y Linux.
- Los notebooks son una herramienta muy valiosa para toda científica de datos, ¿por qué? -> Las 3 respuestas son válidas.
- Entre las ventajas de trabajar con notebooks en la nube se encuentran: Las 3 respuestas son válidas.
- Hablando de notebooks, ¿qué quiere decir que una aplicación nos permita trabajar a nivel de archivo o a nivel de proyecto? -> El trabajo a nivel de archivo hace referencia a que un único notebook es la entrada a nuestro proyecto. El trabajo a nivel de proyecto indica que tenemos múltiples puntos de entrada al proyecto.
