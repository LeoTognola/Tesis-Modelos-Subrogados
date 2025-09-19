# Modelos Subrogados para Ondas Gravitacionales

Este repositorio contiene los códigos completos utilizados para el desarrollo y prueba de **modelos subrogados** aplicados a ondas gravitacionales. 
El objetivo es generar señales, construir modelos reducidos y evaluar su desempeño en la estimación de parámetros como las masas de sistemas binarios. 

Este repositorio contiene los códigos desarrollados e implementados para el Trabajo Final de Licenciatura en Física (UNCA), orientado al estudio de modelos subrogados de ondas gravitacionales y su aplicación en la estimación de parámetros.

---

## Contenido del repositorio

01_generacion_senales → códigos para generar ondas gravitacionales exactas (PyCBC).

02_modelos_subrogados → construcción de bases reducidas y aproximación mediante.

03_estimacion_parametros → uso de filtrado por correlación y matches para estimar masas.

04_resultados → scripts para graficar ondas, calcular errores y comparar modelos.

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

bash
docker pull pycbc/pycbc-el7:latest

---

## Autor

Leandro Ezequiel Tognola – Septiembre 2025
