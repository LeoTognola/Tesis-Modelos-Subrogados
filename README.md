## Modelos Subrogados para Ondas Gravitacionales

Este repositorio contiene los códigos desarrollados e implementados para mi Tesis de Licenciatura en Física en la Facultad de Ciencias Exactas y Naturales de la Universidad Nacional de Catamarca (UNCA, Argentina).

El trabajo está orientado al desarrollo y estudio de modelos subrogados de ondas gravitacionales, con el objetivo de generar señales, construir modelos reducidos y evaluar su desempeño en la estimación de parámetros como las masas de sistemas binarios.

---

## Contenido del repositorio

- 01_generación_señales/
Scripts para generar ondas gravitacionales exactas utilizando PyCBC. Incluye ejemplos con distintos rangos de masas y aproximantes.

- 02_modelos_subrogados/
Implementación de la construcción de bases reducidas (SVD) y la interpolación en el espacio de parámetros.

  - 1_modelo_subrogado.ipynb: Primer modelo subrogado, trabaja con una señal observada más simple y resultados a mejorar.
  - 2_modelo_subrogado_mejorado.ipynb: Versión mejorada, trabaja con una onda más compleja, con cambios significativos en la construcción y resultados.

- 03_estimación_parámetros/
Códigos para la estimación de masas mediante filtrado por correlación (matched filtering) y comparación de formas de onda (Match).

- 04_resultados/
Gráficos de ondas, análisis de errores y comparación entre los modelos.

---

##  Librerías utilizadas

Los códigos fueron desarrollados y requieren las siguientes librerías principales de Python:

- [`numpy`](https://numpy.org/) → operaciones numéricas.
- [`scipy`](https://scipy.org/) → análisis matemático y optimización.
- [`matplotlib`](https://matplotlib.org/) → visualización y gráficos.
- [`pycbc`](https://pycbc.org/) → generación y análisis de ondas gravitacionales.
- [`arby`](https://github.com/ligo-cbc/arby) → construcción de modelos subrogados y bases reducidas.
- [`lal`](https://lscsoft.docs.ligo.org/lalsuite/lal/) (opcional, instalado con PyCBC) → librerías de análisis de LIGO.

---

## Entorno de ejecución con Docker

Los códigos se desarrollaron y probaron en un entorno **Docker** usando la imagen oficial de PyCBC.  
La imagen puede descargarse directamente desde **Docker Hub**:  

🔗 [PyCBC Docker Hub: pycbc/pycbc-el7](https://hub.docker.com/r/pycbc/pycbc-el7)  

Comando para obtener la última versión:  

bash docker pull pycbc/pycbc-el7:latest

---

## Limitaciones

- Los modelos subrogados implementados en este repositorio fueron desarrollados y probados únicamente para sistemas con masas iguales ($m_1 = m_2$).

- La extensión a configuraciones con $m_1 \neq m_2$ u otros parámetros no está incluida en este trabajo.

- El objetivo principal fue validar la metodología en un caso simple antes de considerar espacios de parámetros más generales.

---

## Autor

Leandro Ezequiel Tognola – Septiembre 2025

