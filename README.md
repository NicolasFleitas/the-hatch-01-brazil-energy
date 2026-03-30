# ⚡ Optimización Energética para Data Center en Brasil

Este proyecto corresponde a la segunda fase del primer desafío de la etapa **The Hatch**. El objetivo es analizar el histórico de consumo eléctrico nacional en Brasil para determinar la ubicación geográfica óptima y la mejor ventana de mantenimiento para un nuevo Centro de Datos, basándonos en la disponibilidad y estabilidad de la red pública.

## 🎯 Objetivos del Proyecto
* Trabajar con datos de series temporales para identificar estacionalidades y tendencias macroeconómicas.
* Filtrar anomalías físicas (registros de consumo negativos o nulos).
* Aplicar lógica de negocio para equilibrar infraestructura tecnológica y baja demanda energética.

## 🛠️ Tecnologías y Herramientas
* **Lenguaje:** Python
* **Análisis y Manipulación:** Pandas (Manejo de Series Temporales e Índices Datetime)
* **Visualización:** Matplotlib, Seaborn
* **Entorno:** Jupyter Notebook

## 📊 Hallazgos y Decisión Estratégica
1. **Estabilidad Operativa:** A través de análisis de varianza y diagramas de caja (Boxplots), se determinó que el mes de **Julio** (invierno en el hemisferio sur) ofrece la red eléctrica más estable a nivel nacional, siendo la ventana ideal para mantenimientos de alto consumo.
2. **Paradoja de la Baja Demanda:** El análisis inicial sugería estados amazónicos (como Acre o Roraima) por su bajo consumo. Sin embargo, aplicando conocimiento de dominio, se corrigió el modelo para evitar zonas sin infraestructura eléctrica industrial, evitando así colapsos en la red local.
3. **El Ganador Definitivo (Pernambuco):** Al filtrar exclusivamente el Top 10 de estados con mayor infraestructura eléctrica (los "gigantes"), **Pernambuco (PE)** se posicionó como la ubicación óptima. Ofrece una red madura capaz de soportar operaciones de grado empresarial y presenta el "valle" de consumo más profundo durante la ventana operativa de invierno.

## 🚀 Cómo ejecutar este proyecto
1. Clona este repositorio: `git clone https://github.com/tu-usuario/the-hatch-01-brazil-energy.git`
2. Descarga el archivo de datos bruto (`dados_brutos.xlsx`) y colócalo en la raíz del proyecto.
3. Abre el archivo principal `.ipynb` en tu entorno preferido.
4. Ejecuta las celdas en orden (el notebook incluye la corrección iterativa de limpieza de datos en tiempo real).