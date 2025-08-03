# 📊 Análisis de Unidades Económicas DENUE en Aguascalientes

Este proyecto analiza y visualiza las unidades económicas registradas en el Directorio Estadístico Nacional de Unidades Económicas (DENUE), específicamente en el estado de Aguascalientes. Se utilizó MongoDB Atlas como base de datos en la nube y se desarrolló una interfaz de análisis interactivo mediante Google Colab, Python, Pandas y Plotly.

## 📁 Dataset utilizado

- **Fuente**: [INEGI - DENUE](https://www.inegi.org.mx/app/descarga/)
- **Archivo**: `.csv` descargado de la sección de DENUE filtrado por estado: *Aguascalientes*
- **Contenido**: Información de negocios como nombre, tipo, personal ocupado, ubicación geográfica (latitud, longitud), colonia, municipio, entre otros.

## 🛠️ Librerías requeridas

Este proyecto se ejecuta en Google Colab y requiere las siguientes librerías:

```bash
pip install pandas plotly pymongo ipywidgets
