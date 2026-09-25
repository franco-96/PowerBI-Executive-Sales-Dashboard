📊 Executive Sales & Profitability Dashboard Power BI 

Un dashboard analítico e interactivo diseñado para la toma de decisiones ejecutivas sobre ventas y rentabilidad global, desarrollado con Microsoft Power BI e integrado sobre el dataset Global Superstore.Demostración Visual e Interacción
<img width="718" height="364" alt="image" src="https://github.com/user-attachments/assets/2e486f17-b98e-4f9a-89e5-17ea8b16d64f" />

**Objetivo del Proyecto:** El propósito de este proyecto fue transformar un conjunto de datos transaccionales masivo en un panel ejecutivo de alto impacto visual y funcional. Se buscó optimizar la experiencia de usuario (UI/UX) reduciendo el ruido visual mediante un tema personalizado Blue - Transparent de alto contraste y resolviendo desafíos técnicos en la presentación de métricas principales.🛠️ Aspectos Técnicos y Diseño UI/UXDiseño Visual Personalizado (UI/UX):Fondo con degradados de azul y transparencias personalizadas en tarjetas y contenedores. Tipografía clara e hiperlegible en color blanco sobre contenedores oscuros.Mapa de burbujas en estilo Dark Theme para integrarse orgánicamente al lienzo.Resolución de Desafíos en DAX y Formato:Creación de medidas DAX avanzadas con formateo estricto de texto mediante la función FORMAT() para garantizar que los KPIs principales muestren cifras resumidas en millones (ej. $ 31,96 M), eliminando truncamientos de texto y garantizando responsividad.📈 Visualizaciones y FuncionalidadComponenteVisualizaciónDescripción y Uso AnalíticoKPIs PrincipalesTarjetas de IndicadoresMuestran de forma clara el Margen de Ganancia %, Crecimiento de Ventas %, Total Ventas y Total Ganancia.Distribución GeográficaMapa de Burbujas (Dark Theme)Permite analizar el volumen de ventas por país y actúa como un filtro cruzado dinámico para todo el reporte.Desglose de RentabilidadÁrbol de DescomposiciónPermite realizar drill-down interactivo sobre la Ganancia Total para explorar contribuciones por Categoría y Mercado.Análisis de TendenciasGráfico de Líneas (YoY)Compara el rendimiento del año actual respecto al anterior mes a mes para detectar estacionalidad.Análisis de DescuentosGráfico de DispersiónEvalúa el impacto del promedio de descuento frente a la ganancia generada por subcategoría de producto.

🧮 Medidas DAX Destacadas// Formateo dinámico para KPI de Ventas Totales en Millones
Total Ventas Card = 
"$ " & FORMAT([Total Ventas] / 1000000, "#,##0.00") & " M"

// Formateo dinámico para KPI de Ganancia Total en Millones
Total Ganancia Card = 
"$ " & FORMAT([Total Ganancia] / 1000000, "#,##0.00") & " M"

// Margen de Ganancia
Margen Ganancia % = 
DIVIDE([Total Ganancia], [Total Ventas], 0)
📁 Estructura del Repositorio├── assets/
│   ├── dashboard-demo.gif   # Demostración en GIF o captura
│   └── dashboard-preview.png # Imagen estática de alta calidad
├── data/
│   └── Global_Superstore.xlsx # Dataset utilizado
├── Executive_Sales_Dashboard.pbix # Archivo ejecutable de Power BI
└── README.md                # Documentación del proyecto

**🚀 Cómo Explorar este ProyectoClonar o descargar el repositorio:git clone:**(https://github.com/franco-96)repositorio.git

Abrir el archivo .pbix: Requiere tener instalado Microsoft Power BI Desktop.
Interactuar: Utiliza los segmentadores de fecha, categoría y mercado en la parte superior para filtrar las métricas en tiempo real.
✍️ Autor: Franco Vergara🔗 LinkedIn: https://www.linkedin.com/in/franco-e-vergara/
