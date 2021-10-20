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

## Configuración de VS Code

### Instalar VS Code

Puedes descargar VS Code [aquí](https://code.visualstudio.com/download).

### Agregar extensiones para VS Code

### Uso de VSCode notebooks

En Python podemos usar `ctrl shift p -> sort imports`

## Quiz 2

- VSCode te permite sincronizar tus extensiones utilizando una cuenta de Microsoft o Github, ¿para qué podría ayudarte esta característica? ->  Al conectarme desde un lugar de trabajo nuevo puedo tener las mismas configuraciones del editor de código con las extensiones que siempre utilizo en un solo paso.
- ¿Las características "sin texto fromateado, detectar errores de sintaxis, resalta sintaxis y autocompletado" corresponden a un editor de código o a un IDE? -> Ambas.
- Un editor de código puede llegar a ser tan bueno como un IDE, ¿por qué? -> Por las múltiples extensiones.

## Entorno de desarrollo en Anaconda

### ¿Qué son los ambientes virtuales?

En la vida real, es normal que trabajes en distintos proyectos al mismo tiempo. Para trabajar en múltiples proyectos es necesario crear un entorno virtual.

### Instalar Conda a tráves de la terminal

Si en nuestra terminal tenemos 'py base' significa que ya tenemos Conda o Anaconda instalado.

Podemos abrir notebooks con el comando `jyputer-notebook`

### Conda: crear y actualizar ambientes

- Ver el listado de ambientes virtuales: `conda env list`
- Crear ambientes virtuales: `conda --name my_proyecto_chido python=3.8 pandas`
- Activar el ambiente virtual: `conda activate my_proyecto_chido`
- Desactivar el ambiente virtual: `conda deactivate`
- Actualizar el paquete del ambiente virtual: `conda update pandas`
- Instalar paquetes en el ambiente virtual: `conda install numpy`
- Clonar un ambiente virtual: `create --name my_proyecto_mas_chido --copy --clone mi_proyecto_chido`

[Conda cheat sheet](https://docs.conda.io/projects/conda/en/4.6.0/_downloads/52a95608c49671267e40c689e0bc00ca/conda-cheatsheet.pdf)

### Conda: Eliminar ambientes y librerías

- Eliminar libreria: `conda remove pandas`
- Eliminar ambiente: `conda env remove --name my_proyecto_chido` **Nota:** el ambiente debe estar desactivado.
