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
También se requiere una cuenta de MongoDB Atlas y una conexión a internet activa para acceder a la base de datos remota.

🗄️ Estructura de la base de datos MongoDB
Cluster: MongoDB Atlas

Base de datos: proyecto_datos

Colección: denue_aguscalientes

Cada documento en la colección representa una unidad económica con campos como:

json
Copiar
Editar
{
  "nombre_de_la_unidad_económica": "Abarrotes El Centro",
  "municipio": "Aguascalientes",
  "colonia": "Centro",
  "latitud": 21.8836,
  "longitud": -102.2916,
  "descripcion_estrato_personal_ocupado": "De 0 a 5 personas"
}
🌐 Conexión a MongoDB (segura)
La conexión se realiza a través de una URI como:

perl
Copiar
Editar
mongodb+srv://<usuario>:<contraseña>@cluster0.xxxxx.mongodb.net/
🔐 Recomendación: mantener las credenciales fuera del código fuente (usar variables de entorno o secrets.py).

📈 Visualizaciones interactivas
El proyecto permite realizar:

Gráficos de barras de unidades económicas por municipio.

Histogramas del estrato de personal ocupado.

Mapa de geolocalización con Plotly + Mapbox.

Búsqueda por colonia y actualización de datos (vía widgets).

💻 Cómo ejecutar
Abre el archivo .ipynb en Google Colab.

Ejecuta cada celda paso por paso:

Subida del CSV

Limpieza y transformación

Inserción a MongoDB

Visualizaciones

Usa los widgets para filtrar por colonia o actualizar registros.

📂 Estructura del repositorio
kotlin
Copiar
Editar
📁 data/
    └── denue_aguascalientes.csv
📁 notebooks/
    └── analisis_denue.ipynb
📁 images/
    └── visualizacion_mapa.png
📄 README.md
👥 Créditos
Alumnos: Luis David Camarillo Leon
Juan Carlos Arias Camarena
Francisco Fabian Rodriguez Sanchez
Adrian Juarez Moreno

Materia: Bases de datos para computo en la nube

Profesor: Ruth Marcela Romero Rojas

Institución: Universidad Tecnologica Fidel Velazquez
