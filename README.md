# world-cup-2026-prediction-model
FIFA World Cup 2026 prediction model built with Python, Power BI, ELO Rating, live API and Monte Carlo simulation.
# FIFA World Cup 2026 Prediction Model

Proyecto de análisis de datos y modelado predictivo aplicado al Mundial FIFA 2026.

El objetivo del proyecto fue construir un modelo capaz de analizar el rendimiento reciente de selecciones, calcular rankings propios, simular partidos individuales y proyectar la fase eliminatoria del torneo utilizando Python, Power BI, ratings ELO, API en vivo y simulaciones Monte Carlo.

---

## Dashboard

El dashboard fue desarrollado en **Power BI Desktop** y diseñado como una experiencia navegable con botones entre páginas.

### Páginas principales

1. **Inicio**

   * Portada navegable del proyecto.
   * Acceso directo a cada sección del dashboard.

2. **Resumen Ejecutivo**

   * Favorito actual.
   * Selecciones analizadas.
   * Partidos históricos analizados.
   * Simulaciones realizadas.
   * Top probabilidades de campeón.
   * Distribución de probabilidades.

3. **Ranking & Análisis**

   * Ranking general de selecciones.
   * Power Score.
   * ELO Rating.
   * Rendimiento reciente.
   * Comparación entre rating y rendimiento.

4. **Simulador de Partidos**

   * Selección dinámica de Equipo A y Equipo B.
   * Probabilidad de victoria, empate y derrota.
   * Goles esperados.
   * Resultados más probables.

5. **Simulación del Torneo**

   * Bracket real del Mundial 2026.
   * Proyección de fase eliminatoria desde 16avos hasta la final.
   * Campeón proyectado.
   * Integración de resultados y estructura real del torneo.

---

## Tecnologías utilizadas

* Python
* Pandas
* NumPy
* Scikit-learn
* OpenPyXL
* Power BI Desktop
* Excel
* API en vivo
* ELO Rating
* Simulación Monte Carlo
* Visualización de datos

---

## Metodología

El proyecto combina distintas fuentes y técnicas:

### 1. Datos históricos

Se trabajó con resultados internacionales históricos para analizar el rendimiento reciente de selecciones.

Las principales métricas calculadas fueron:

* Partidos jugados
* Victorias
* Empates
* Derrotas
* Goles a favor
* Goles en contra
* Diferencia de gol
* Puntos por partido
* Rendimiento ponderado por tipo de torneo

---

### 2. Power Score

Se construyó un indicador propio llamado **Power Score**, diseñado para medir la fortaleza relativa de cada selección.

El indicador combina:

* Rendimiento reciente
* Diferencia de gol
* Puntos ponderados
* Rating ELO
* Rendimiento actual del torneo

---

### 3. Integración de ELO Rating

El modelo incorpora ratings ELO para mejorar la evaluación de fuerza relativa entre selecciones.

Esto permite combinar rendimiento reciente con una medida histórica de fortaleza competitiva.

---

### 4. Simulador de partidos

Para cada cruce posible entre dos selecciones, el modelo estima:

* Probabilidad de victoria del Equipo A
* Probabilidad de empate
* Probabilidad de victoria del Equipo B
* Goles esperados
* Marcadores más probables

La estimación utiliza el Power Score, el rating ELO y una aproximación probabilística basada en goles esperados.

---

### 5. API en vivo

Se incorporó una conexión a una API para obtener información actualizada del torneo, incluyendo:

* Equipos
* Grupos
* Partidos
* Resultados
* Estructura real del bracket

Esto permite que la simulación respete los cruces reales del Mundial 2026.

---

### 6. Simulación Monte Carlo

Se ejecutaron simulaciones Monte Carlo para estimar probabilidades de avance y campeón.

El modelo simula múltiples escenarios posibles de la fase eliminatoria y calcula probabilidades agregadas para cada selección.

---

## Estructura del repositorio

```text
world-cup-2026-prediction-model
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── notebooks
│   ├── 01_data_exploration.ipynb
│   ├── 02_modern_team_performance.ipynb
│   ├── 03_world_cup_2026_prediction.ipynb
│   ├── 04_live_api_connection.ipynb
│   └── 05_real_bracket_simulation.ipynb
│
├── scripts
│   └── model_pipeline.py
│
├── data_sample
│   └── sample_processed_data.xlsx
│
└── outputs
    └── screenshots
        ├── 00_inicio.png
        ├── 01_resumen_ejecutivo.png
        ├── 02_ranking_analisis.png
        ├── 03_simulador_partidos.png
        └── 04_simulacion_torneo.png
```

---

## Capturas del dashboard

### Inicio

![Inicio](outputs/screenshots/00_inicio.png)

### Resumen Ejecutivo

![Resumen Ejecutivo](outputs/screenshots/01_resumen_ejecutivo.png)

### Ranking & Análisis

![Ranking & Análisis](outputs/screenshots/02_ranking_analisis.png)

### Simulador de Partidos

![Simulador de Partidos](outputs/screenshots/03_simulador_partidos.png)

### Simulación del Torneo

![Simulación del Torneo](outputs/screenshots/04_simulacion_torneo.png)

---

## Nota sobre Power BI

El dashboard fue desarrollado en **Power BI Desktop**.

El archivo `.pbix` no se incluye en este repositorio.
La visualización final se presenta mediante capturas y video de navegación en LinkedIn.

---

## Seguridad

Por seguridad, las API keys y credenciales privadas no se incluyen en este repositorio.

En los notebooks, cualquier clave debe reemplazarse por:

```python
API_KEY = "YOUR_API_KEY_HERE"
```

o por variables de entorno.

---

## Objetivo del proyecto

Este proyecto fue desarrollado como parte de mi portfolio de Data Analytics, con el objetivo de demostrar habilidades en:

* Limpieza y transformación de datos
* Análisis exploratorio
* Modelado predictivo
* Automatización con Python
* Visualización con Power BI
* Diseño de dashboards
* Integración con datos en vivo
* Comunicación visual de resultados

---

## Autor

**Iván Alderete**
Data Analytics Portfolio

Data · Insights · Impact
