# Análisis de Uso de Internet en Chile – SUBTEL 2024

## Descripción General
Este proyecto analiza el uso de Internet en Chile utilizando datos públicos de la Décima Encuesta de Acceso y Usos de Internet (2024), publicada por la Subsecretaría de Telecomunicaciones (SUBTEL).

El objetivo es construir un análisis simple, claro y reproducible, enfocado en entender diferencias de uso según zona geográfica y grupos etarios, priorizando la claridad analítica y comunicacional por sobre la complejidad técnica.

---

## Pregunta Analítica
**¿Existen diferencias en el uso de Internet según zona (urbana vs rural) y grupo etario en Chile?**

---

## Fuente de Datos
- **Organismo:** Subsecretaría de Telecomunicaciones (SUBTEL)
- **Dataset:** Décima Encuesta Acceso y Usos de Internet 2024
- **Formato original:** SPSS (.sav)
- **Origen:** Datos públicos disponibles en el sitio oficial de SUBTEL

---

## Proceso de Preparación de Datos
El procesamiento de datos se realizó utilizando Python en un Jupyter Notebook, siguiendo estos pasos:

1. Carga del archivo `.sav` mediante la librería `pyreadstat`.
2. Exploración inicial para entender estructura, variables y calidad de los datos.
3. Selección de variables relevantes para el análisis:
   - Edad
   - Sexo
   - Zona (urbana / rural)
   - Región
   - Factor de expansión (POND_USO)
4. Creación de grupos etarios para facilitar el análisis comparativo.
5. Transformación de códigos numéricos a valores descriptivos.
6. Eliminación de registros con valores nulos.
7. Exportación del dataset final en formato CSV para su uso en herramientas de visualización.

---

## Dataset Final
El archivo generado se encuentra en:

data/processed/internet_uso_zona_edad_chile.csv


Este dataset fue utilizado para la construcción del panel de analítica.

---

## Decisiones de Diseño del Dashboard
- Se definió una pregunta clara y acotada para orientar el análisis.
- Se priorizó la comparación entre zonas urbanas y rurales.
- Se utilizaron visualizaciones simples (barras y tablas) para facilitar la lectura.
- Se incorporaron filtros para permitir la exploración por región y grupo etario.
- Se evitó complejidad innecesaria, enfocándose en comunicar insights de forma clara.

---

## Herramientas Utilizadas
- Python (pandas, pyreadstat)
- Jupyter Notebook
- Power BI / Tableau / Looker Studio (panel de analítica)
- GitHub (repositorio público)

---

## Autor
Proyecto desarrollado como parte de un proceso de postulación al cargo de **Data Analyst** en Datalized.


