# Gestion de Datos 
Mariana Bedoya Barrero


La **Gestión de Datos** es un concepto fundamental y cada vez más vital en la era del Big Data, especialmente en entornos indusstriales y empresariales. Las fuentes la abordan tanto desde una perspectiva conceptual y metodológica como a través de ejemplos prácticos que ilustran su importancia y aplicación.
La gestión de datos se refiere al **manejo de la información desde su recolección hasta su procesamiento**. Implica la necesidad de gestionar volúmenes de información cada vez mayores, comúnmente denominados Big Data. Los autores categorizan la gestión de datos en tres grupos principales:

1. **Presencia de Datos**: Relacionado con la recolección o recopilación de datos.

2. **Coordinación de Datos**: Incluye el preprocesamiento o limpieza de datos (como la eliminación de errores de medición o la anotación de información) y el almacenamiento.

3. **Computación de Datos**: Se refiere al procesamiento o análisis de datos (compilar, establecer relaciones y conocimientos, integrar con otras herramientas).

Además de estos aspectos técnicos, la gestión de datos abarca áreas como la **privacidad, seguridad, ética, integración y estándares de calidad**.

Las características del Big Data, conocidas como las "Vs", son cruciales:

• **Volumen**: La inmensa cantidad de datos generados y recolectados.

• **Velocidad**: La rapidez con la que se generan y deben procesarse o analizarse los datos, crucial para sistemas en tiempo real.

• **Variedad**: Los innumerables tipos y formatos que pueden tomar los datos (estructurados, semi-estructurados, no estructurados).

• **Veracidad**: La fiabilidad, precisión y confianza en los datos, que pueden provenir de fuentes propensas a errores, ruido o inconsistencias.

• **Variabilidad**: La volatilidad e inconsistencia de los datos en estructura, formato y tasa de llegada.

• **Visualización**: La presentación de Big Data y su análisis en un formato significativo y comprensible para facilitar la toma de decisiones.

• **Valor**: El objetivo final del proceso de Big Data: extraer información, patrones y correlaciones útiles.

La existencia de **"Dark Data"** (datos ocultos o no utilizados) subraya un desafío en la gestión de datos, ya que estos pueden constituir el mayor volumen dentro de un sistema de Big Data.
## Aspectos Cruciales de la Gestión de Datos en la Práctica

1. **Extracción de Datos**: Es el componente crítico para recolectar datos de diversas fuentes, siendo los sensores la más común. El auge del Internet de las Cosas (IoT) ha provocado una proliferación masiva de dispositivos que generan datos, haciendo que las infraestructuras y metodologías para cosechar estos datos de manera efectiva sean esenciales para evitar desbordamientos del sistema y asegurar la escalabilidad. Las arquitecturas a menudo emplean **middleware**, plataformas de ingesta, y **"message brokers"** como Apache Kafka, RabbitMQ o Amazon Kinesis. Protocolos como OPC-UA son cada vez más adoptados en la industria.

2. **Preprocesamiento de Datos**: Los datos brutos a menudo son difíciles de procesar y contienen información que complica la extracción de conocimiento. El preprocesamiento busca ajustar los datos extraídos para mejorar su idoneidad para la utilización.
   
3. **Operaciones Comunes**: Limpieza (eliminación de valores atípicos o ruido), Normalización (ajuste de escalas), Imputación (manejo de valores perdidos) y Transformación (agregar, agregar, reorganizar).

El preprocesamiento es vital para manejar datos heterogéneos, optimizar el uso de ancho de banda al transmitir datos a la nube y preparar la información para el análisis, aunque puede introducir demoras en el flujo de datos.

## Herramientas de Procesamiento, Análisis y Visualización de Datos (Business Intelligence y Analytics)
Estas herramientas son el "cerebro" del sistema, convirtiendo los datos en información valiosa y presentando los resultados:

**ETL (Extract, Transform, Load)**: Un método tradicional que extrae datos de una fuente, los transforma para cumplir con un esquema de almacenamiento y luego los carga en el almacén de datos. Requiere un sistema intermedio de "data staging".

**ELT (Extract, Load, Transform)**: Extrae datos de la fuente, los carga directamente en el sistema de almacenamiento y luego los transforma. Es más adecuado para aplicaciones en tiempo real y Big Data.

**Query Editor (en Power BI Desktop)**: Una herramienta poderosa para la transformación y combinación de datos, que utiliza el lenguaje M (anteriormente Power Query). Permite fusionar consultas, añadir columnas calculadas y definir tipos de datos.

**Microsoft Power BI**: Un ecosistema completo para Business Intelligence de autoservicio (Self-Service BI), que opera como un servicio en la nube.

**Power BI Desktop**: Aplicación de escritorio para construir modelos de datos complejos, conectar a diversas fuentes (Excel, SQL Server, Google Analytics) y diseñar informes.

**Servicio en la Nube**: Permite subir y compartir paneles (dashboards) e informes, ofrece consultas en lenguaje natural (Q&A), Quick Insights (basado en IA para encontrar patrones), interacciones visuales y filtrado.

**DAX (Data Analysis Expressions)**: Lenguaje utilizado para crear medidas, columnas calculadas y tablas calculadas, lo que permite análisis más avanzados y el control del diseño del informe.

**Gateways (Personal y Enterprise)**: Software para conectar Power BI en la nube a fuentes de datos locales para la actualización de datos.

**Integración con Office**: Permite incrustar visualizaciones de Power BI en Excel y PowerPoint.

**Custom Visualizations**: Una galería de visualizaciones creadas por la comunidad para extender las capacidades estándar.

**REST API**: Para integrar Power BI con otras aplicaciones y automatizar operaciones, incluyendo paneles en tiempo real.

**Tableau**: Un software líder en visualización de datos, enfocado en Business Intelligence y la gestión de Big Data.

**Tableau Desktop**: Herramienta de arrastrar y soltar para explorar y visualizar todo tipo de datos, creando visualizaciones, informes y paneles.

**Tableau Server y Tableau Online**: Permiten publicar y compartir informes y paneles de forma online o en la nube.

**Tableau Public y Tableau Reader**: Versiones gratuitas para crear y ver visualizaciones interactivas.

**Tibco Spotfire**: Otra plataforma de Business Intelligence con capacidades de análisis y visualización.
◦ Ofrece análisis ad hoc, reporting, y funcionalidades estadísticas avanzadas (MATLAB, SAS, R, S+) directamente desde su interfaz.
    ◦ Se destaca por su capacidad de integración nativa con bases de datos (incluidas herramientas de Big Data) y herramientas de terceros como CRM, ERP, Excel.

**Microsoft Excel**: Una herramienta muy extendida y fácil de usar para analizar y visualizar datos, especialmente para usuarios no especializados en TI.

**Microsoft SQL Server Reporting Services (SSRS)**, **Analysis Services (SSAS)** e **Integration Services (SSIS)**: Parte de la suite de SQL Server, ofrecen herramientas para informes, análisis multidimensional y ETL.

**Pentaho**: Un kit de herramientas de Business Intelligence de código abierto que proporciona integración de datos, servicios OLAP, reporting, tabulación, minería de datos y capacidades ETL.

**SAS Visual Analytics**: Permite obtener respuestas rápidas a consultas complejas con datos de cualquier tamaño, incluidos grandes datos en Hadoop.

**SAP Lumira**: Software para el descubrimiento rápido de datos de conjuntos pequeños y grandes, permitiendo la descarga y consolidación directa de datos.

**MicroStrategy y QlikView**: Otros proveedores de herramientas de Business Intelligence.

**IBM Watson y Apple Siri**: Ejemplos de sistemas comerciales de respuesta a preguntas basados en procesamiento de lenguaje natural y IA.

En resumen, la gestión de datos en la era del Big Data exige un amplio conjunto de herramientas y técnicas, que van desde sistemas de infraestructura distribuida y de almacenamiento innovadores (Hadoop, NoSQL, data lakes) hasta potentes plataformas de análisis y visualización (Power BI, Tableau, Spotfire), respaldadas por algoritmos avanzados de inteligencia artificial y machine learning. El éxito reside en la integración y aplicación inteligente de estas herramientas para transformar los datos brutos en valor estratégico y decisiones informadas.


# Quien es el autor destacado y que libro es el mas leido 
El libro "Big Data in Practice" de Bernard Marr, según los extractos y reseñas, es una obra fundamental que desmitifica el concepto de Big Data, ofreciendo una visión práctica y tangible de cómo diversas empresas, desde gigantes minoristas hasta pequeños negocios y organizaciones especializadas, están utilizando el análisis de datos para lograr resultados extraordinarios. El consenso general es que el Big Data ya no es una teoría o una "moda pasajera", sino una realidad transformadora que afecta cada aspecto de los negocios y la sociedad. La clave del éxito radica en la capacidad de las organizaciones para recopilar, almacenar y, crucialmente, analizar grandes volúmenes y variedades de datos para obtener información accionable y una ventaja competitiva.

Big Data: No es una Moda, Sino el Nuevo Normal
Los autores y revisores enfatizan que el Big Data es una fuerza imparable y duradera. Como señala el autor Bernard Marr en la Introducción: "La palabra que le hemos dado a este movimiento es Big Data y lo cambiará todo, desde la forma en que operan los bancos y las tiendas hasta la forma en que tratamos el cáncer y protegemos nuestro mundo del terrorismo. No importa en qué trabajo estés y no importa en qué industria trabajes, Big Data lo transformará." Asimismo, Mark van Rijmenam, autor de "Think Bigger", afirma que "Bernard Marr proporciona una visión general completa de lo lejos que ha llegado Big Data en los últimos años. Con ejemplos inspiradores muestra claramente cómo grandes y pequeñas organizaciones pueden beneficiarse de Big Data. Este libro es una lectura obligatoria para cualquier organización que quiera ser un negocio impulsado por los datos."

<img width="270" height="407" alt="image" src="https://github.com/user-attachments/assets/c1cbb21b-65f7-4731-a6c3-bc58e083b360" />


# Artículo científico 
El documento "BIG DATA, UN SISTEMA DE GESTIÓN DE DATOS" de Ángel Gómez Degraves, un PhD en Estadística Aplicada y Organizaciones Inteligentes, explora la creciente importancia de Big Data como una nueva revolución industrial en la transformación empresarial. El estudio, realizado en 2021, presenta una investigación exploratoria documental que analiza el auge de Big Data y su aplicación en la reducción de tiempos de captura, organización, almacenamiento, procesamiento y análisis de grandes volúmenes de datos. Se abordan aspectos clave como la definición de Big Data, sus tipos de datos (estructurados, semiestructurados y no estructurados), las dimensiones conocidas como las "V" (Volumen, Velocidad, Variedad, Valor y Veracidad), y las herramientas tecnológicas y técnicas empleadas para su tratamiento, destacando Apache Hadoop como una solución fundamental. El autor concluye que Big Data es una respuesta esencial para la gestión de datos, la obtención de información y conocimiento, y la mejora de la competitividad empresarial, a pesar de los desafíos de implementación.

Autor: Ángel Gómez Degraves PhD in Applied Statistics and Intelligent Organizations, Tecana American University, of the USA
gomezdegraves@gmail.com
2021

**Journal of Intelligent Manufacturing** https://doi.org/10.1007/s10845-025-02570-z
Data management in industry: concepts, systematic review and future directions
Nelson Freitas1 · Andre Dionisio Rocha1 · Jose Barata1
Received: 22 May 2024 / Accepted: 10 January 2025 © The Author(s) 2025
Este estudio aborda la creciente importancia de la gestión de datos en entornos industriales, especialmente frente al aumento de grandes volúmenes de información (Big Data) generado por la Cuarta Revolución Industrial. Los autores llevan a cabo una revisión sistemática de la literatura para comprender las prácticas actuales en el sector manufacturero. Destacan que, a pesar de la vitalidad de una buena gestión de datos para la seguridad, productividad y eficiencia, existe una deficiencia metodológica en las implementaciones, incluso dentro de industrias similares. El trabajo enfatiza la necesidad de una comprensión profunda de conceptos clave como la extracción, almacenamiento, preprocesamiento y procesamiento de datos, así como la identificación de principios fundamentales para construir sistemas de gestión de datos eficientes y optimizados, buscando también futuras direcciones y mejoras en este campo.

# Cuál es la evolución a lo largo del tiempo de Gestión de datos o Data Management

<img width="3446" height="1720" alt="image" src="https://github.com/user-attachments/assets/34e3b456-2fb4-4829-925a-d30f39fb30d6" />

A partir de los años 60 empezo el auge de la gestión de datos, luego en el año 2000 empezo a caer esta tendencia, pero despues sigue en constante crecimiento asi como las herramientas para la gestion de los datos

# Opinión personal de aporte a mi carrera y en el país

Realmente el conocimiento es poder, tener un correcto control y manejo de datos, pero sobre todo el conocimiento de los datos ayudara a poder tomar decisiones para mejoras en todo ambito de la empresa, muchas veces en las empresas se tienen datos sobre todo en el área de producción, se tiene registros que muchas veces se quedan en el papel solo por cumplir la norma, pero son datos que pueden dar mucha información para la toma de decisiones, para encontrar cuellos de botella, para disminuir costos innecesarios. Lamentablemente en nuestro país solo se hace las cosas con el fin de cumplir un reglamento y una norma, pero si realmente se tomaria los datos de una forma que ayude a mejorar todo el sistema, realmente seria diferente el nivel de industria que ofrecemos para la transformacion de materias primas y servicios. 
La gestion de datos no solo es importante en las industrias manufactureras, es importante en todo ambito empezando desde la salud, continuando en las empresas de servicio como banca y todas las empresas estatales y municipales. Esta en nuestras manos el capacitar a las personas operativas a tener buenos datos, explicar el porque necesitamos registrarlos y luego mostrar los resultados y mejoras, para que todo eso no sea un mero trabajo para cumplir tareas asignadas.

Esta materia me inspiro mucho porque la inteligencia esta a nuestro servicio y que ahora podemos tener la informacion mucho mas rapido y nos ayuda a mejorar y tener la capacidad de aprender mejor en menos tiempo, en las demas materias se aplicara estos conocimientos que se aprendieron porque realmente son llaves para mejorar nuestro propio aprendizaje 

LaPaza 15092025 horas 15:22
