# Análisis Estadístico Comparativo: Flota de Autotaxis en la Comunidad de Madrid

> **Asignatura:** Estadística (1° Grado en Ingeniería de Computadores - Grupo A)
> **Universidad:** Universidad de Alcalá (UAH)  
> **Autor:** Pablo Kratochvil Molpeceres 

---

## Introducción
Este repositorio contiene el desarrollo completo de la **Práctica de Laboratorio 1 (PL1)** de la asignatura de Estadística. El objetivo principal es realizar un análisis estadístico descriptivo y bivariante de la potencia mecánica de los vehículos que componen la flota oficial de autotaxis de la Comunidad de Madrid, comparando de forma directa las diferencias técnicas entre los dos fabricantes predominantes en el sector: **Toyota** y **Skoda**.

---

## Metodología y Herramientas

* **Origen de los datos:** Fichero oficial abierto de licencias de autotaxi de la Comunidad de Madrid (`300226-0-taxi-flota-diaria-csv.csv`).
* **Herramientas de software:** Procesamiento y cálculos realizados mediante **RStudio**, utilizando el lenguaje R y paquetes estadísticos como `qcc` (diagramas) y `e1071` (medidas de asimetría y curtosis).
* **Muestra analizada:** 11.371 vehículos autorizados en total, de los cuales 10.809 corresponden a la marca Toyota y 562 a Skoda.
* **Variables de estudio:**
  * **Marca del vehículo** (cualitativa nominal: Toyota vs. Skoda).
  * **Potencia mecánica del vehículo** (cuantitativa continua, medida en CV o kW).

---

## Resultados Principales de las Medidas estadísticas

A partir del análisis de las medidas estadísticas e intervalos de potencia, se obtuvieron las siguientes conclusiones clave:

1. **Dominio de Toyota:** La marca Toyota representa el **95% de la flota diaria** en la muestra analizada (10.809 taxis).
2. **Homogeneidad vs. Variabilidad:** 
   * **Toyota** destaca por una potencia media de **76,96 CV** con una gran concentración de vehículos estandarizados en torno a los 72-73 CV, mostrando una dispersión muy baja ($CV = 0,23$).
   * **Skoda** presenta una media significativamente superior de **112,6 CV** con una mayor dispersión y variedad mecánica ($CV = 0,37$).
3. **Tablas de contingencia:** Al agrupar la potencia en intervalos, se observa que casi el 99.4% de los vehículos Toyota se concentran en el rango de [60.8, 110.5) CV, mientras que Skoda distribuye más de un 24% de su flota en gamas superiores a 110.5 CV.

---

## Estructura del Repositorio

* `Informe Estadístico - PL1 - Kratochvil Molpeceres Pablo.pdf`: Memoria formal del informe descriptivo completo.
* `codigo_R/`: Scripts y comandos utilizados en RStudio para la depuración, cálculo de estadísticos, tablas de contingencia y generación de diagramas.
* `graficos/`: Exportación de los histogramas, diagramas de tarta y boxplots generados en el análisis.

---

## Referencias
* Hilera, J.R. (2026). *Prácticas de Estadística descriptiva*. Universidad de Alcalá.
* Portal de Datos Abiertos de la Comunidad de Madrid. *Registro de la Flota Diaria de Vehículos Autotaxis*.
