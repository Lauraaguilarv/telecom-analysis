# telecom-analysis
Análisis de uso de servicios móviles para ConnectaTel 


##  Objetivo del proyecto

Analizar el comportamiento de los clientes de ConnectaTel, una empresa de
telecomunicaciones con operaciones en México y Colombia, para identificar
patrones de uso, detectar comportamientos atípicos y segmentar clientes
según edad y nivel de consumo. El análisis busca apoyar decisiones
comerciales como el diseño de nuevos planes y estrategias de retención.

---

##  Datasets utilizados

| Archivo | Descripción |
|---|---|
| `plans.csv` | Planes disponibles: precio, minutos, GB y costos por excedente |
| `users_latam.csv` | Información de 4,000 clientes: edad, ciudad, plan, fecha de registro y churn |
| `usage.csv` | 40,000 registros de uso real: llamadas (duración) y mensajes (longitud) |

---

##  Etapas del análisis

1. **Carga y exploración** – Revisión de estructura, tipos de datos y primeras filas.
2. **Identificación de problemas de calidad** – Detección de nulos, sentinels y fechas fuera de rango.
3. **Limpieza básica** – Corrección de valores inválidos (`age: -999`, `city: '?'`, fechas con año 2026).
4. **Summary statistics** – Estadísticas descriptivas por usuario (mensajes, llamadas, minutos).
5. **Visualización y outliers** – Histogramas y boxplots para detectar distribuciones y valores extremos.
6. **Segmentación de clientes** – Clasificación por nivel de uso (Bajo, Medio, Alto) y grupo de edad (Joven, Adulto, Adulto Mayor).
7. **Insight ejecutivo** – Conclusiones y recomendaciones comerciales para stakeholders.

---

##  Cómo ejecutar el notebook

1. Abre el notebook en **Google Colab** o **Jupyter Notebook**.
2. Descarga los datasets y colócalos en la carpeta `/datasets/` o ajusta las rutas en las celdas de carga.
3. Ejecuta las celdas en orden desde la primera hasta la última.
4. Las librerías necesarias son: `pandas`, `numpy`, `seaborn` y `matplotlib`.

---

##  Tecnologías utilizadas
- Python 3.9
- pandas · numpy · seaborn · matplotlib
- Jupyter Notebook


