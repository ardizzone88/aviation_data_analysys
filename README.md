[README (2).md](https://github.com/user-attachments/files/27773250/README.2.md)
#  ✈️ Análisis de Datos de Aviación

<div align="center">

![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-5.x-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)
![Colab](https://img.shields.io/badge/Google%20Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)
![API](https://img.shields.io/badge/AviationStack%20API-0057B7?style=for-the-badge&logo=airplane&logoColor=white)

**Proyecto de portfolio para analista de datos** — Extracción, limpieza, análisis y visualización de datos de vuelos en tiempo real.

[![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/TU_USUARIO/TU_REPO/blob/main/aviation_analysis_es.ipynb)

</div>

---

## 📋 Descripción

Este proyecto analiza datos de vuelos reales obtenidos mediante la **API de AviationStack** para identificar patrones de puntualidad, distribución de demoras y tendencias geográficas del tráfico aéreo mundial.

Incluye **10 gráficos interactivos** construidos con Plotly, un pipeline completo de datos con Pandas y un dashboard de KPIs listo para presentar en un portfolio profesional.

---

## 🎯 Objetivos del Análisis

- Identificar patrones de **puntualidad** por aerolínea y ruta
- Analizar la **distribución de estados** de vuelo (a tiempo, demorado, cancelado)
- Visualizar el **volumen de tráfico** por aeropuerto y franja horaria
- Detectar **tendencias geográficas** en la actividad aérea mundial

---

## 📊 Gráficos Generados

| # | Tipo | Descripción |
|---|------|-------------|
| 1 | 🍩 Dona | Distribución de estados de vuelo |
| 2 | 📊 Barras horizontales | Vuelos por aerolínea (color = demora promedio) |
| 3 | 📈 Área apilada | Tráfico aéreo por franja horaria |
| 4 | 📉 Histograma | Distribución de demoras con boxplot |
| 5 | 📊 Barras agrupadas | Puntualidad vs demoras por aerolínea |
| 6 | 🗺️ Mapa mundial | Rutas aéreas globales (a tiempo / demorado) |
| 7 | 🌳 Treemap | Top aeropuertos de salida |
| 8 | 🔵 Burbujas | Bandas de demora por aerolínea |
| 9 | 📈 KPI Dashboard | Indicadores clave del análisis |
| 10 | ☀️ Sunburst | Análisis jerárquico Estado → Aerolínea → Demora |

---

## 🛠️ Tecnologías

```
Python 3.10+
├── requests       — Consumo de la API REST
├── pandas         — Limpieza y transformación de datos
├── numpy          — Cálculos numéricos y datos sintéticos
├── plotly         — Visualizaciones interactivas
└── kaleido        — Exportación de gráficos a PNG/PDF
```

---

## 🚀 Cómo Ejecutar el Proyecto

### Opción A — Google Colab (recomendado, sin instalación)

1. Hacé clic en el botón **"Open in Colab"** al inicio de este README
2. Guardá una copia en tu Drive: `Archivo → Guardar una copia en Drive`
3. Pegá tu API key en la celda de configuración
4. Ejecutá todo: `Entorno de ejecución → Ejecutar todo`

### Opción B — Entorno local

```bash
# 1. Clonar el repositorio
git clone https://github.com/TU_USUARIO/TU_REPO.git
cd TU_REPO

# 2. Crear entorno virtual
python -m venv venv
source venv/bin/activate        # Linux / macOS
venv\Scripts\activate           # Windows

# 3. Instalar dependencias
pip install -r requirements.txt

# 4. Iniciar Jupyter
jupyter notebook aviation_analysis_es.ipynb
```

---

## 🔑 Configuración de la API

1. Registrate gratis en [aviationstack.com](https://aviationstack.com)
2. Copiá tu API key desde el dashboard
3. En el notebook, reemplazá la siguiente línea:

```python
API_KEY = 'TU_API_KEY_AQUI'
```

> **Nota:** Si no tenés una API key, el notebook carga automáticamente un **dataset de demostración con 300 vuelos sintéticos** para que puedas explorar todos los gráficos sin restricciones.

---

## 📁 Estructura del Proyecto

```
📦 aviation-data-analysis/
 ┣ 📓 aviation_analysis_es.ipynb   ← Notebook principal
 ┣ 📄 requirements.txt             ← Dependencias
 ┣ 📄 README.md                    ← Este archivo
 ┗ 📂 graficos_aviacion/           ← Gráficos exportados (.html)
    ┣ 01_distribucion_estados.html
    ┣ 02_vuelos_por_aerolinea.html
    ┣ 03_trafico_por_hora.html
    ┣ 04_histograma_demoras.html
    ┣ 05_puntualidad.html
    ┣ 06_mapa_rutas_mundial.html
    ┣ 07_treemap_aeropuertos.html
    ┣ 08_burbujas_demoras.html
    ┣ 09_dashboard_kpis.html
    ┗ 10_sunburst_jerarquico.html
```

---

## 📈 Principales Insights

A partir del análisis de los datos se obtienen conclusiones como:

- **Puntualidad general** — qué porcentaje de vuelos sale a tiempo
- **Aerolínea más puntual** — ranking por demora promedio
- **Hora pico** — franja con mayor concentración de salidas
- **Tasa de cancelación** — proporción de vuelos cancelados
- **Distribución de demoras** — cuántos vuelos se demoran 0–15 min, 15–30 min, etc.

> Los valores exactos varían según los datos del día de ejecución.

---

## 📦 Requirements

Creá el archivo `requirements.txt` con el siguiente contenido:

```
requests>=2.31.0
pandas>=2.0.0
numpy>=1.24.0
plotly>=5.15.0
kaleido>=0.2.1
jupyter>=1.0.0
```

---

## 🤝 Contribuciones

Las sugerencias y mejoras son bienvenidas.

1. Hacé un fork del repositorio
2. Creá una rama: `git checkout -b feature/nueva-funcionalidad`
3. Commiteá tus cambios: `git commit -m 'Agrega nueva funcionalidad'`
4. Hacé push: `git push origin feature/nueva-funcionalidad`
5. Abrí un Pull Request

---

## 📄 Licencia

Distribuido bajo la licencia MIT. Consultá el archivo `LICENSE` para más información.

---

## 👤 Autor

**Tu Nombre**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/TU_PERFIL)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/TU_USUARIO)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=googlechrome&logoColor=white)](https://TU_WEB.com)

---

<div align="center">
  <sub>⭐ Si este proyecto te fue útil, dejá una estrella en el repositorio</sub>
</div>
