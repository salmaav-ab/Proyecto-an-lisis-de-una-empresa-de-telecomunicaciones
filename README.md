# Proyecto-an-lisis-de-una-empresa-de-telecomunicaciones

🎯 Objetivo del proyecto
Explorar, limpiar y analizar tres fuentes de datos para construir una visión clara, confiable y accionable sobre el comportamiento de uso de los clientes, respondiendo preguntas clave del negocio:

¿Qué segmentos muestran mayor o menor uso de llamadas y mensajes?
¿Qué usuarios presentan valores atípicos (posible fraude o error de registro)?
¿Cómo varía el uso según la edad y el tipo de plan contratado?
¿Qué patrones pueden guiar el diseño de mejores planes?

📂 Datasets utilizados
ArchivoDescripciónplans.csvCatálogo de planes: precio, minutos incluidos, GB incluidos y costo por extra.users_latam.csvInformación de clientes: edad, ciudad, fecha de registro, plan contratado y churn.usage.csvActividad de uso: llamadas (duración) y mensajes (longitud) por usuario.
Los tres datasets se relacionan a través del identificador de usuario y el nombre del plan.

🔄 Etapas del análisis

Carga y exploración inicial — Revisión de estructura, tipos de datos y primeras observaciones de cada dataset.
Identificación de problemas de calidad — Detección de valores nulos, sentinels (-999, "NA", "?"), fechas fuera de rango e inconsistencias lógicas.
Limpieza de datos — Reemplazo de sentinels, conversión de tipos, imputación o marcado de valores faltantes según reglas de negocio.
Estadísticas descriptivas — Cálculo de media, mediana, percentiles y distribuciones para variables numéricas y categóricas.
Visualización y detección de outliers — Histogramas y boxplots para identificar sesgos y valores atípicos; método IQR para cuantificarlos.
Segmentación de clientes — Creación de grupos basados en edad, país, plan contratado y nivel de consumo; visualización con countplots y gráficas comparativas.
Insights y recomendaciones comerciales — Conclusiones orientadas al negocio con acciones concretas para cada segmento identificado.

🛠️ Herramientas y librerías

Python 3.x
pandas — manipulación y limpieza de datos
numpy — cálculos estadísticos
matplotlib y seaborn — visualizaciones
Jupyter Notebook

🚀 Cómo ejecutar el notebook
Google Colab

Abrir Google Colab.
Ir a Archivo → Abrir notebook → GitHub y pegar la URL de este repositorio, o usar Subir para cargar el archivo .ipynb directamente.
Subir los tres archivos CSV desde una computadora usando el panel de archivos.
Ejecutar todas las celdas con Runtime → Run all.

📋 Guía de reproducción

Asegurarse de que los tres archivos CSV (plans.csv, users_latam.csv, usage.csv) estén en la misma carpeta que el notebook.
Ejecutar las celdas en orden secuencial — cada sección depende de la limpieza y transformaciones realizadas en las anteriores.
Los gráficos se generan automáticamente al ejecutar cada celda correspondiente; no se requiere configuración adicional.
Los resultados del análisis (tablas de segmentación, outliers detectados) se muestran directamente en el notebook con texto interpretativo en cada sección.
numpy — cálculos estadísticos
matplotlib y seaborn — visualizaciones
Jupyter Notebook**
