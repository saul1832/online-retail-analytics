# Online Retail Analytics – Python, SQL & Power BI

📄 **Este README está en español**.  
🌐 [Read in English](README.md) | 🇫🇷 [Lire en Français](README_FR.md)

---
## Descripción:  
Este proyecto es parte de mi portafolio de Análisis de datos.
Analizo el dataset Online Retail II [(Kaggle)](https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci) aplicando técnicas de limpieza de datos, análisis exploratorio y visualización. 
El objetivo es demostrar competencias técnicas en Python, SQL y Power BI, así como habilidades de comunicación de insights orientados al negocio.  

> Dataset final limpio:   
> 1,054,675 filas y 15 columnas

---
## Tecnologías utilizadas  
* Python (Pandas, Numpy, Seaborn, Matplotlib)
* SQL (SQLite vía SQLAlchemy, consultas con CTE para agregaciones)
* Power BI (dashboards interactivos con medidas DAX)
* Jupyter Notebook para documentación del análisis

---
## Estructura del repositorio  
`/data`          → datasets crudos y limpios 
`/notebooks`     → notebooks de exploración y análisis EDA  
`/powerbi`       → archivo .pbix con dashboard interactivo  
`/reports`       → capturas del dashboard y one-pager resumen  
`requirements.txt`  
`README.md` 

> **Nota sobre los datos**  
> Los archivos en la carpeta `/data` no se incluyen en el repositorio debido a su tamaño.  
> El dataset original puede descargarse desde [Kaggle – Online Retail II](https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci).  

➡️ **Importante:** Una vez descargado, colóquelo en la carpeta `/data` con el nombre `online_retail_II.csv` antes de ejecutar los notebooks.  

> **Nota sobre los notebooks**  
> Este proyecto incluye dos versiones de cada Jupyter Notebook: una en **inglés** y otra en **español**.  
> No se realizarán más traducciones a otros idiomas, ya que mantener varios idiomas en paralelo requiere un esfuerzo considerable.  
> Tanto la versión en inglés como la versión en español se mantendrán actualizadas para asegurar consistencia. 

---
## Principales hallazgos  

> A menos que se indique lo contrario, los valores se refieren a las ventas Netas. Las ventas brutas son especificadas explícitamente.

1. **Dos segmentos principales de mercado**: Reino Unido representa el 85.70% de las ventas brutas totales, mientras que el resto del mundo representa solo el 14.30%.
2. **Estacionalidad clara**: El Q4 concentra la mayor parte de las ventas, especialmente en regalos y decoraciones. 
3. **Clientes no identificados**: El 13.80% de las ventas netas carecen de Customer ID, lo que limita la segmentación.
4. **Devoluciones bajo el promedio de la industria**: Los retornos representan el 15.79 % de las facturas totales, cifra inferior al promedio de la industria (20%). – [Outvio (2024)](https://outvio.com/blog/return-rate-stats/).

---
## Aspectos destacados del dashboard

![How to Use](reports/1_How%20to%20Use.jpg)  
*Instrucciones, reglas de limpieza (ETL) y limitaciones del dataset.*

![Overview](reports/2_Overview.jpg)  
*Visión general: £20.11M en Ventas Brutas, £19.38M en Ventas Netas; Devoluciones = 3.61%; Ticket Neto Promedio = £413.29.*

![Products](reports/3_Products.jpg)  
*Top Productos por Ventas Netas: Regency Cakestand (£327.74K), White Hanging Heart T-Light (£257.51K). Las devoluciones se concentran en pocos ítems.*

![Countries](reports/4_Countries.jpg)  
*Países: Reino Unido domina con 85.70% de Ventas Netas (£16.59M). Irlanda y Países Bajos aparecen muy por detrás.*

![Sales](reports/5_Sales.jpg)  
*Ventas por hora y día de la semana: picos marcados los jueves y al mediodía (12h), insight clave para la planificación de campañas.*

---
## Recomendaciones  
1. **Campañas estacionales**: Aprovechar el Q4 con bundles estratégicos de productos top y ofrecer complementos o productos premium en el checkout (upsell).
2. **Implementar programa de registro de clientes para reducir ventas sin ID**: Reducir las ventas sin identificación del cliente en 7% en tres meses.
3. **Acciones sobre devoluciones**: Revisar la descripción, las fotos y el empaque de los 5 productos con mayor porcentaje de devoluciones (Meta: disminuir la tasa de devolución de la empresa en un 20% en un plazo de 60 días).
4. **Incorporar información de costos**: Solicitar y registrar el costo unitario y los gastos de envío de cada producto para poder calcular la rentabilidad real y priorizar aquellos con mayor margen.

---
## Dashboard en Power BI  
* **Página 1: How to Use** – Cómo usar el reporte y supuestos, notas importantes, historial de versión y contacto.
* **Página 2: Overview** – KPIs ejecutivos, top productos y clientes por ventas, ventas por día de la semana, distribución de ventas y devoluciones, evolución temporal ventas y devoluciones. Filtro disponible por país, año y mes.
* **Página 3: Products** – KPIs de producto, top ventas y devoluciones por orden de retorno, análisis temporal de ventas y devoluciones. Filtro disponible por producto, país y año.
* **Página 4: Customers** – KPIs de cliente, top ventas y devoluciones por orden de retorno, análisis de ventas por cliente y producto, análisis temporal de ventas y devoluciones. Filtro disponible por cliente y año.
* **Página 5: Countries** – KPIs de país, top ventas y ticket promedio, análisis de ventas de producto por país, análisis temporal de ventas y devoluciones. Filtro disponible por país y año.
* **Página 6: Sales** – KPIs de ventas, evolución temporal de ventas, top productos y pares de productos más comprados (estático), heatmap de ventas por día de la semana y hora. Filtro disponible por país, año y mes.
* **Página 7: Returns** – KPIs de devoluciones, evolución temporal de devoluciones, devoluciones sobre ventas, devoluciones por día de semana, mes y año, top países, clientes y productos por devoluciones. Filtro disponible por país, cliente, producto, mes y año.

---
## Cómo ejecutar el proyecto  

> Probado en Python 3.11.9 y pandas 2.2.3

1. Clonar este repositorio:  
> git clone https://github.com/saul1832/online-retail-analytics.git  
> cd online-retail-analytics

2. Instalar dependencias:  
> pip install -r requirements.txt

3. Abrir los notebooks en Jupyter:  
> jupyter notebook

---
## Autor
Saúl Huamán Alvarado  
Data Analyst (Python, SQL, Power BI) | Budget Control & Financial Reporting 

[Email](mailto:saul18_@hotmail.com) | [LinkedIn](https://www.linkedin.com/in/saulha/) | [GitHub](https://github.com/saul1832)

