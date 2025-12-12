# Proyecto-Final-Simulaci-n-
Análisis de la operación de un cine (taquilla y dulcería) mediante simulación de eventos discretos en ProModel 2016 e integración con la Teoría de Colas (M/M/S) para proponer mejoras operativas.


# 🎬 Simulación y Análisis de la Operación de un Cine (ProModel + Teoría de Colas)

## 📝 Descripción del Proyecto

Este repositorio contiene los modelos, datos y documentación del proyecto integrador para analizar la eficiencia operativa de un complejo de cine (simulando los procesos de Taquilla y Dulcería) a través de dos metodologías complementarias:

1.  **Simulación de Eventos Discretos (ProModel 2016):** Modelado del flujo real de clientes, utilizando distribuciones de probabilidad ajustadas a partir de datos empíricos (Lognormal, Normal, Uniforme y Exponencial).
2.  **Análisis Teórico de Colas (M/M/S):** Uso de la formulación Erlang-C, aproximando los procesos por sus medias para validar la capacidad y las predicciones de la simulación.

El objetivo es identificar cuellos de botella, dimensionar la capacidad de servidores (ventanillas) y proponer escenarios de mejora que minimicen el tiempo de espera de los clientes ($\text{W}_q$).

## ⚙️ Metodología y Herramientas

* **Software de Simulación:** ProModel 2016
* **Ajuste de Distribuciones:** Stat::Fit
* **Base de Datos:** Datos reales de llegadas y tiempos de servicio recopilados en campo.
* **Modelo Teórico:** M/M/S (Multi-servidor)
* **Métricas Clave:** Longitud de cola ($\text{L}_q$), tiempo de espera en cola ($\text{W}_q$), y utilización de servidores ($\rho$).

## 📂 Estructura del Repositorio

| Directorio/Archivo | Contenido |
| :--- | :--- |
| `/doc` | Documentación formal del proyecto (artículo LaTeX, presentaciones). |
| `/datos` | Archivos de datos brutos y ajustados (muestreos, resultados de Stat::Fit). |
| `/promodel` | Archivos fuente de ProModel (`.MOD`, `.MCD`, reportes de salida). |
| `README.md` | (Este archivo) Descripción y guía del proyecto. |

## 🚀 Resultados Clave

* **Identificación de cuellos de botella:** Se determinó que la [Taquilla / Dulcería] es el área con mayor tiempo medio de espera.
* **Propuesta de mejora:** Se sugiere incrementar la capacidad de servidores en [Área] a $s=2$ (taquilla) y $m=3$ (dulcería), lo que reduce el $\text{W}_q$ en un $\text{X}\%$ según la simulación.

---

## 👥 Autores

* Ortíz Pérez Gael Fernando
* Luna Cenobio Sarai
* García Pérez César Miguel
