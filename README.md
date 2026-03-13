# Internal Elasticity Cosmology (IEC-QFT) - Stage 5

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19001869.svg)](https://doi.org/10.5281/zenodo.19001869)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Physics: QFT](https://img.shields.io/badge/Physics-QFT%20%26%20Cosmology-blue)]([https://github.com/electronicaintegralmonje-hub/IEC_Stage5])

Este repositorio contiene el material de base, los códigos de simulación y los archivos de pre-publicación de la **Etapa 5** del modelo de Cosmología de Elasticidad Interna (IEC). 

En este trabajo —Etapa 5— demostramos que la propia gravedad métrica emerge como el modo colectivo de baja energía de
dicho medio elástico. Tratando al espacio-tiempo como un sólido elástico cuántico con rigidez κ y módulo de cizalla μ derivados de la coherencia de ϕ, derivamos las ecuaciones de Einstein a partir de la hidrodinámica de longitud de onda larga del vacío elástico, reproduciendo la Relatividad General exactamente en el límite clásico mientras se predicen desviaciones cuánticas controladas en las escalas de Planck. Los horizontes de los agujeros negros adquieren una tensión superficial elástica, resolviendo la paradoja de la información mediante estados de memoria coherente; el problema de la constante cosmológica se resuelve mediante
la relajación de la rigidez del vacío; y las ondas gravitacionales primordiales adquieren una
relación de dispersión característica testeable con LISA y futuros interferómetros.

## Estructura del Repositorio

El material se organiza en las siguientes secciones:

**`Images/`**: Contiene todas las figuras, diagramas de la Curva de Page modificada, y las composiciones de datos observacionales (JWST/Hubble) utilizadas en el manuscrito.
**`LaTeX/`**: Archivos fuente para la compilación del documento académico.
    * Incluye versiones en **Inglés** y **Español**.
    * Archivo `references.bib` con la bibliografía unificada y corregida (incluye citas a Einstein, Planck, Hawking, Kerr y otros).
**`Scripts/`**: Archivos de Python (`.py`) que contienen los algoritmos para:
    * Generación de gráficas de la tasa de evaporación modificada.
    * Simulaciones de ringdown elástico y ecos rotacionales.
    * Visualización de parámetros de cizalla circular.

---

 Guía de Uso

 1. Compilación del Documento
Para obtener el PDF con el formato académico correcto, utiliza **TeXstudio** o cualquier entorno LaTeX con soporte para **Biber**:
1. Abre el archivo principal en la carpeta `LaTeX/`.
2. Asegúrate de que el archivo `.bib` esté en el mismo directorio.
3. Ejecuta la secuencia: `PdfLaTeX` -> `Biber` -> `PdfLaTeX` (x2).

2. Ejecución de Simulaciones
Los scripts requieren Python 3.1+ y las siguientes librerías:
```bash
pip install numpy scipy matplotlib
