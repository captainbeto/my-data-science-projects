# My Data Science Project Template 📊

Este repositorio sirve como base para desarrollar proyectos de ciencia de datos. Cada proyecto que comparta se basará en esta estructura. Para leer el readme en inglés consultar [README.md](https://github.com/sofiavalino/template-datascience-project/blob/main/README.md).

## Objetivo 🎯

Este repositorio tiene como objetivo ...

## Estructura del repositorio 📂

```plaintext
template-datascience-project/
├── data/                       # Almacenamiento de datos
│   ├── raw/                    # Datos sin procesar
│   ├── processed/              # Datos limpios y procesados
├── notebooks/                  # Notebooks Jupyter
│   ├── exploration.ipynb       # Exploración y análisis inicial
│   ├── model.ipynb             # Creación y evaluación de modelos
├── src/                        # Código fuente
│   ├── preprocessing.py        # Preprocesamiento de datos
│   ├── models.py               # Creación y evaluación de modelos
│   ├── utils.py                # Funciones auxiliares
├── outputs/                    # Resultados generados
│   ├── figures/                # Visualizaciones y gráficos
│   ├── predictions/            # Predicciones generadas
├── app/                        # Scripts de aplicación y despliegue
│   ├── main.py                 # Punto de entrada de la aplicación
│   ├── api.py                  # Funciones relacionadas con la API
│   ├── config.py               # Configuraciones específicas
├── deployments/                # Configuraciones de despliegue
│   ├── kubernetes/             # Manifiestos de Kubernetes
│   ├── docker/                 # Configuraciones de Docker
│   ├── cloudbuild/             # Configuraciones de Cloud Build
├── docs/                       # Documentación y diagramas
│   ├── diagrams/               # Arquitectura y workflows
│   ├── reports/                # Informes analíticos
├── requirements-project.txt    # Dependencias del proyecto
├── README.md                   # Documentación del proyecto
└── .gitignore                  # Archivos y carpetas ignorados por Git
```

## Repositorio compartido: `shared-resources` 🔧

Este proyecto está diseñado para trabajar junto con un repositorio compartido llamado [`shared-resources`](https://github.com/sofiavalino/shared-resources) que contiene recursos reutilizables entre múltiples proyectos.

### ¿Qué incluye `shared-resources`?

El repositorio `shared-resources` centraliza herramientas y configuraciones comunes para proyectos de ciencia de datos, tales como:

- **Logger centralizado** (`logger.py`) para unificar los registros de actividad.
- **Configuraciones globales** (`config/global_config.py`) para gestionar rutas, claves API, y parámetros comunes.
- **Utilidades compartidas** (`utils/`) como funciones para medir tiempos de ejecución (`timer.py`) o cargar datos (`data_loader.py`).
- **Plantillas de logs** (`logs/`) para monitorear actividades específicas, como preprocesamiento.

### ¿Cómo usar `shared-resources` en este proyecto?

1. Agrega el submódulo al repositorio:

   ```bash
   git submodule add https://github.com/sofiavalino/shared-resources shared/
   git submodule update --init --recursive
   ```

2. Importa y utiliza los recursos necesarios desde el submódulo. Por ejemplo:

   ```python
   from shared.utils.data_loader import load_data
   df = load_data('data/raw/dataset.csv')
   ```

3. Mantén el submódulo actualizado:

   ```bash
   git submodule update --remote
   ```

## Cómo ejecutar este proyecto 🖥️

1. Clona este repositorio y sus submódulos:

   ```bash
   git clone --recursive https://github.com/sofiavalino/template-datascience-project.git
   ```

2. Instala las dependencias necesarias:

   ```bash
   pip install -r requirements-project.txt
   ```

3. Ejecuta el proyecto siguiendo las instrucciones en los notebooks o scripts.


## Contribuciones 🤝

Si tienes alguna sugerencia para mejorar los proyectos, o si encuentras algún problema, no dudes en abrir un issue o enviar un pull request. Puedes también dejar tus comentarios en los proyectos que te interesen.


## Licencia 📜

Este proyecto está bajo la [MIT License](https://github.com/sofiavalino/template-datascience-project/blob/main/LICENSE). Si deseas usar o modificar el código, asegúrate de revisar los términos de la licencia.

## Contacto 📧

¡Explora los proyectos y si tienes alguna pregunta o sugerencia, no dudes en contactarme!

[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0077B5?logo=linkedin&logoColor=white&style=flat-square)](https://www.linkedin.com/in/sofiavalino/)  
[![Gmail](https://img.shields.io/badge/-Gmail-D14836?logo=gmail&logoColor=white&style=flat-square)](mailto:valinosofia@gmail.com)


## Por último pero no menos importante: Mi Blog =^._.^= 📚

Además de los proyectos de este repositorio, también comparto mis apuntes de la facultad y temas relacionados con Data Science y ciencias de la computación en mi blog. En él, encontrarás contenido sobre las materias que estudio, así como detalles sobre los proyectos que realizo y otros temas de interés.

[![Blog](https://affable-valinosofia.wordpress.com/wp-content/uploads/2024/07/site-logo.png?w=88&h=88)](https://affable-valinosofia.wordpress.com/)
