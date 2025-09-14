
Trabajo realizado por 
SERGIO ARMIJO CABRERIZO 


[[Optimización de Rutas]]

Según la aplicación Harzing´s Pulish or Perish el libro mas citado en trabajos e investigaciones científicas es "Network Flows"

## Libro mas vendido y consultado 
<img width="307" height="423" alt="NETWORK FLOWS" src="https://github.com/user-attachments/assets/68a03f5b-6db8-431a-9b98-cee09950dc92" />
el libro tiene mas de 17,000 citas
<img width="1567" height="261" alt="Citas del libro 1" src="https://github.com/user-attachments/assets/4ec782d3-c4ff-44f4-b9ca-938234a098d6" />
Sobre el tema el libro toca los siguientes puntos 
### Optimización de Rutas en Transporte Logístico con Flujos en Redes
El libro analiza los **modelos de flujos en redes** como herramienta matemática fundamental para resolver problemas de transporte y distribución. La idea principal es representar el sistema logístico como una **red de nodos y arcos**, donde:

 **Nodos** → representan almacenes, centros de distribución, fábricas o clientes.
 **Arcos** → representan rutas de transporte (carreteras, vías férreas, aéreas, etc.) con capacidades y costos asociados.
 **Flujos** → representan cantidades de mercancía que deben moverse a través de la red.
###  Principales modelos aplicados a logística

1 **Problema de Transporte**
   - Determina cómo enviar bienes desde varios orígenes (almacenes) hasta múltiples destinos (clientes) al **menor costo total posible**, cumpliendo con la oferta y la demanda.
   - Ejemplo: distribución de productos desde un centro logístico a supermercados.
2.**Problema de Ruta más Corta**
   - Busca la ruta que minimice distancia, tiempo o costo entre dos puntos.
   - Aplicado en logística para seleccionar caminos eficientes para vehículos de reparto .
3.**Flujo de Costo Mínimo**
- Generalización del transporte: no solo asegura cumplir demanda y oferta, sino que **considera restricciones de capacidad en las rutas**.    
- Optimiza asignando flujos en toda la red, reduciendo tiempos de entrega y costos operativos .
4 **Problemas Multicommodity (múltiples productos)**
   - Se aplican cuando distintos tipos de mercancía comparten la misma red.    
   - El reto es coordinar envíos de varios productos sin saturar rutas y equilibrando costos .
5 **Problema del Viajante (TSP) y Ruteo de Vehículos (VRP)**
- Modelos que buscan **planificar la secuencia de visitas** de un vehículo a múltiples clientes con el mínimo recorrido.
- Muy usados en logística urbana y de última milla .
###  Técnicas de Optimización

 **Programación lineal y entera**: herramientas matemáticas clave para formular y resolver estos problemas .
 **Algoritmos clásicos**: Dijkstra y Bellman-Ford (para rutas más cortas), simplex y métodos de descomposición (para transporte y costos mínimos).
 **Relajación lagrangiana**: útil para problemas de gran escala donde no se puede resolver de forma exacta .
### 🚛 Impacto en la Logística

- **Reducción de costos** → menos gasto en combustible y personal.
- **Mejor utilización de recursos** → camiones, almacenes y rutas se aprovechan al máximo.
- **Mayor satisfacción del cliente** → entregas rápidas y confiables.
- **Flexibilidad** → permite simular diferentes escenarios (cierres de carreteras, cambios en la demanda, etc.).


###  **Problema de Flujo de Costo Mínimo (Minimum Cost Flow)**


### 1. Flujo de Costo Mínimo
$$
\text{Minimizar } \sum_{(i,j)\in A} c_{ij} x_{ij}
$$
**Restricciones:**
$$
\sum_{j:(i,j)\in A} x_{ij} - \sum_{j:(j,i)\in A} x_{ji} = b(i), \quad \forall i \in N
$$

$$
l_{ij} \leq x_{ij} \leq u_{ij}, \quad \forall (i,j)\in A
$$

 **Uso:** modelo general para redes con múltiples orígenes y destinos, con costos y capacidades.

- $x_{ij}$ : cantidad transportada por la ruta de $i$ a $j$.
- $c_{ij}$ : costo por unidad en la ruta $(i,j)$.
- $b(i)$ : oferta/demanda del nodo  
  - $b(i) > 0$ → nodo origen (oferta)  
  - $b(i) < 0$ → nodo destino (demanda)  
  - $b(i) = 0$ → nodo de transbordo  
- $l_{ij}, \; u_{ij}$ : límites de capacidad de la ruta $(i,j)$  
  - $l_{ij}$ = flujo mínimo permitido  
  - $u_{ij}$ = flujo máximo permitido

### 2. **Problema de Ruta Más Corta (Shortest Path Problem)**

Busca la mejor ruta entre un origen y un destino.  
Se modela como un caso particular del flujo de costo mínimo:


$$
\text{Minimizar } \sum_{(i,j)\in A} c_{ij} x_{ij}
$$

**Restricciones de flujo:**
$$
\sum_{j:(i,j)\in A} x_{ij} - \sum_{j:(j,i)\in A} x_{ji} =
\begin{cases} 
1 & \text{si } i=s \\ 
-1 & \text{si } i=t \\ 
0 & \text{en otro caso}
\end{cases}
$$

📌 **Uso:** encontrar la ruta mínima en costo/tiempo entre un origen y un destino.



---

### 3. **Problema de Transporte (Transportation Problem)**

Es un caso clásico aplicado en logística:

$$
\text{Minimizar } \sum_{i \in Orígenes}\sum_{j \in Destinos} c_{ij} x_{ij}
$$

**Restricciones:**
$$
\sum_{j} x_{ij} = s_i \quad \forall i \quad (\text{oferta})
$$

$$
\sum_{i} x_{ij} = d_j \quad \forall j \quad (\text{demanda})
$$

$$
x_{ij} \geq 0
$$

📌 **Uso:** asignar envíos desde almacenes a clientes al menor costo cumpliendo oferta y demanda.

- $s_i$ : oferta del origen $i$  
- $d_j$ : demanda del destino $j$


## Como artículos científicos que hablan del tema 

Podemos citar
1 **Industria Data** "Modelo de optimización de programación de rutas para una empresa logística peruana usando herramientas FSMVRPTW" de Reyes Morales, Norman
[Industria data.pdf](https://github.com/user-attachments/files/22322866/Industria.data.pdf)

2 **El Hombre y la Máquina** "Diseño de un modelo de optimización de rutas de transporte" de Bermeo Muñoz, Elver A.; Calderón Sotero, Jaime Hernán
[El hombre y la maquina.pdf](https://github.com/user-attachments/files/22322867/El.hombre.y.la.maquina.pdf)

![[Industria data.pdf]]![[El hombre y la maquina.pdf]]
## Evolución del tema 

Segun Google Gram el tema se aborda desde 1970
![[Evolucion en el tiempo 1.png]]
<img width="1659" height="621" alt="Evolucion en el tiempo 1" src="https://github.com/user-attachments/assets/34934d99-ecb0-4dbb-b08f-2fdb65eb3b29" />

## Comentarios 

Creo que todo lo que vimos sobre la optimización de rutas es súper útil para pensar en cómo mejorar el transporte y la logística en Bolivia. Nuestro país tiene muchas dificultades por la geografía, como caminos largos o rutas que no siempre están en buen estado, y eso encarece el costo de mover productos. Si aplicamos modelos como el del transporte, el flujo de costo mínimo o la ruta más corta, se podrían diseñar planes de distribución que reduzcan gastos de combustible y tiempo, además de organizar mejor el uso de camiones y almacenes, usar estas herramientas matemáticas puede servir para modernizar la logística boliviana y hacerla más eficiente frente a los desafíos que tenemos.

Pienso que en el libro s _network flows_ también puede servir mucho para las empresas en Bolivia, porque les da una forma clara de organizar mejor sus procesos de transporte, distribución y hasta producción. Por ejemplo, con los modelos de costo mínimo una empresa que manda mercadería desde La Paz, Santa Cruz o Cochabamba podría decidir cómo repartir sus envíos de la manera más barata sin perder tiempo ni dinero en rutas innecesarias. Los problemas de ruta más corta ayudan a planificar los recorridos de los camiones en ciudades donde el tráfico o el mal estado de las calles pueden hacer que un viaje sea más caro de lo pensado, estas técnicas ayudan a aprovechar mejor los recursos y a reducir pérdidas. 

[[Plataformas TMS]]
Según lo investigado uno de los Mas leídos es
<img width="624" height="763" alt="Plataformas T" src="https://github.com/user-attachments/assets/ec580f68-6283-490e-a3a8-3366c77739cc" />
En el libro Transportation: A Global Supply Chain Perspective de John J. Coyle, C. John Langley Jr., Robert A. Novack, Brian J. Gibson

Trata TMS de forma explícita el capitulo 3 "TRANSPORTATION TECHNOLOGY AND SYSTEMS" 
“**Next Generation TMS**”

**Sistemas de Gestión del Transporte (TMS)** son plataformas tecnológicas que permiten planificar, ejecutar y controlar de manera más eficiente el movimiento de mercancías dentro de la cadena de suministro. Estas herramientas no solo optimizan rutas, consolidan cargas y reducen costos, sino que también mejoran la visibilidad y el control de los envíos en tiempo real. Además, el libro muestra cómo las **apps móviles tipo Uber Freight** y los **modelos de precios dinámicos** están transformando la contratación del transporte al hacerla más ágil y transparente, eliminando intermediarios y ajustando tarifas según la demanda. Si bien los beneficios son claros en términos de eficiencia, reducción de errores y ahorros económicos, su adopción requiere superar desafíos como altos costos de implementación, integración entre sistemas y la necesidad de cambios culturales dentro de las empresas.

- Un **TMS** es una plataforma de software que ayuda a planear, ejecutar y evaluar el transporte.
- Funciona como el “cerebro” de las operaciones de transporte, conectando cargadores, carriers, almacenes y clientes.
- **LasCapacidades principales que tienen los TMS**
    - **Planificación**: selección de rutas, carriers y modos de transporte; optimización de cargas.
    - **Ejecución**: tendering (asignación de cargas a transportistas), visibilidad en tránsito, generación de documentos, programación de citas.
    - **Analítica**: control de costos, auditoría de facturas de flete, monitoreo de KPIs, dashboards de desempeño.
- **Beneficios esperados**
    - Reducción de costos de transporte (≈10–15%).
    - Mayor visibilidad y control de envíos.
    - Mejor cumplimiento contractual y nivel de servicio.
    - Rápido ROI gracias a soluciones en la nube.
    - Integración con WMS, ERP y sistemas de planeación.
- **Tendencias (“Next Generation TMS”)**
    - Migración a **plataformas cloud**.
    - Uso de **analytics avanzados** y **machine learning**.
    - Conexión en tiempo real con carriers vía APIs.
    - Enfoque en **control towers** para visibilidad global.
| **Plataforma / Proveedor**                 | **Funcionalidad destacada**                                   | **Efectividad**                                       | **Problema que resuelve**                                      |
| ------------------------------------------ | ------------------------------------------------------------- | ----------------------------------------------------- | -------------------------------------------------------------- |
| **Oracle Transportation Management (OTM)** | Gestión global de transporte multimodal, integración con ERP. | Altamente escalable, usado por grandes corporaciones. | Complejidad en redes globales; optimización costo–servicio.    |
| **SAP Transportation Management (SAP TM)** | Integración profunda con SAP ERP y SCM.                       | Fuerte en compañías que ya usan SAP.                  | Visibilidad unificada y automatización de procesos.            |
| **MercuryGate TMS**                        | Flexibilidad en gestión de cargas TL/LTL y multimodal.        | Eficaz en medianas y grandes empresas.                | Control de costos, tendering eficiente.                        |
| **JDA / Blue Yonder TMS**                  | Optimización avanzada de ruteo y planeación.                  | Potente en analytics.                                 | Selección de rutas/carriers de manera óptima.                  |
| **Transplace (ahora Uber Freight)**        | Plataforma 3PL + TMS con visibilidad y analítica.             | Muy efectiva en outsourcing de transporte.            | Reduce riesgos y simplifica la gestión con múltiples carriers. |
| **Descartes Systems**                      | Fuerte en visibilidad y cumplimiento regulatorio.             | Ampliamente usado en comercio internacional.          | Cumplimiento normativo y documentación global.                 |
## Artículo científico que hablan del tema 

Podemos citar

1 **GESTIÓN DE ALMACENES Y TECNOLOGÍAS DE LA INFORMACIÓN Y COMUNICACIÓN (TIC)**

en el articulo menciona los **sistemas y tecnologias aplicadas

- **WMS (Warehouse Management System):** Administra inventarios, recepción, almacenamiento, pedidos y cobros.
- **LMS (Labor Management System):** Optimiza la productividad del personal.
- **YMS (Yard Management System):** Control de patios y muelles.
- **Código de barras:** Identificación y trazabilidad básica.
- **RFID:** Identificación automática por radiofrecuencia, con mayor alcance que el código de barras.
- **Picking to Light / Voice:** Preparación de pedidos asistida por luces o voz.
- **SCE (Supply Chain Execution):** Integra TMS, LMS y WMS para optimizar flujos logísticos.

También menciona los **Beneficios esperados de estas tecnologías:**

- Reducción de costos.
- Mejora de la trazabilidad y coordinación.
- Productividad y cumplimiento de pedidos a tiempo.
- Uso óptimo de recursos y mayor rentabilidad.
[TMS.pdf](https://github.com/user-attachments/files/22323789/TMS.pdf)
## Evolución del tema 

Segun Google Gram el tema se aborda desde 1970 y tiene un aumento significativo entre 1995 y los 2000
<img width="1758" height="786" alt="TMS GGRAM" src="https://github.com/user-attachments/assets/0b56fc1d-e60c-4c00-a4c4-7d49f8826dcb" />
## Comentarios 


Creo que todo lo visto hoy sobre los TMS tiene una aplicación muy directa para las empresas en Bolivia, especialmente porque muchas todavía gestionan el transporte de forma manual o con sistemas poco integrados. Un TMS podría ayudarles a reducir costos logísticos, que en nuestro país suelen ser altos por la infraestructura limitada y la dispersión geográfica de los mercados. Además, el uso de plataformas móviles de reserva de carga o modelos de precios dinámicos permitiría aprovechar mejor la capacidad de los transportistas locales, dándoles más visibilidad y acceso a clientes sin depender tanto de intermediarios. se que muchas empresas grandes en Bolivia utiliza algún sistema pero muchas aun no se lanzan a mejorar por lo que me parece una gran inversión y  para la industria en Bolivia 

[[Blockchain para trazabilidad]]

Según lo investigado este tema es bastante moderno y uno de los libros que habla del tema es "Blockchain and the supply chain"
<img width="307" height="462" alt="Libro Blockchain" src="https://github.com/user-attachments/assets/1b9f0458-58a4-476c-8037-30818082a81f" />
El libro explica la evolución de la cadena de suministro global: más globalización, más complejidad, mayores expectativas del consumidor (rapidez, transparencia, sustentabilidad)

Identifica los retos modernos: rupturas recientes (ej. COVID-19) muestran fragilidad en flujos físicos, de información y financieros. Problemas como retrasos, falta de visibilidad, dependencia de intermediarios, burocracia documental.

- Un **marco estratégico** para decidir si adoptar blockchain: identificar puntos de dolor (ineficiencias, falta de transparencia, pérdidas, litigios, devoluciones) y medir métricas actuales. Luego evaluar si blockchain aporta mejora clara frente a soluciones alternativas. 
- Cómo seleccionar el tipo de blockchain (pública, permissionada, híbrida) según necesidades de privacidad, rendimiento, coste y escala. 
- Integración con otros sistemas: ERP, sistemas de gestión de almacén, sensores IoT, plataformas de datos, análisis. Importancia de captura de datos correcta (garantizar integridad desde origen).
- 
Aunque no siempre el libro revela todos los detalles técnicos internos, el ejemplo de _Maersk & IBM / TradeLens_ es uno de los casos más desarrollados y sirve para ilustrar cómo se conjugan varios elementos:

- **Objetivo**: reducir el papeleo, mejorar visibilidad de contenedores en tránsito, agilizar los documentos aduaneros y de envío.

- **Arquitectura**: basado en _blockchain permissionada_ (hyperledger fabric). Los nodos los operan navieras, puertos, agentes de carga, autoridades aduaneras. No es una red abierta.

- **Datos registrados**: ubicación del contenedor, estado documental (factura, certificado de origen, conocimiento de embarque), eventos en tránsito (entrada/salida de puertos, escaneo de sensores si hay condiciones especiales), avisos de discrepancias.

- **Integración**: con los sistemas de los puertos y las aduanas; interfaz digital para los participantes; APIs/portales para ver el estatus; uso de sensores IoT para condiciones ambientales en ciertos tipos de carga refrigerada.

- **Beneficios observados**: reducción de tiempos de despacho, menor costo operativo por trámites manuales, mejor predicción de llegada de contenedores, mayor transparencia entre actores, menos demoras sanitarias/regulatorias.

- **Limitaciones encontradas**: adopción desigual de participantes, resistencia al cambio, problemas de interoperabilidad, costos iniciales de sensores, infraestructura de red en puertos o rutas remotas, complejidad de escalar para muchas rutas internacionales.
## ¿Qué es Blockchain?

- **Definición**: Es una tecnología de registro distribuido (Distributed Ledger Technology, DLT) que almacena transacciones en bloques enlazados criptográficamente, creando un historial inmutable.

- **Características clave** :
    - Descentralización (no hay una sola autoridad de control).    
    - Inmutabilidad (los datos no pueden alterarse sin consenso).
    - Autenticación y sellado temporal (timestamping).
    - Trazabilidad de transacciones.
- **Tipos**:
    - **Públicas** (ej. Bitcoin, Ethereum).
    - **Permisionadas** (ej. Hyperledger, R3 Corda).
    - **Híbridas** según el nivel de acceso y gobernanza .

## ¿Cómo funciona?

- Cada transacción es validada por consenso entre nodos.

- Una vez aprobada, se añade a un bloque que se enlaza al anterior mediante hash criptográfico .

- Los contratos inteligentes (smart contracts) permiten ejecutar automáticamente acuerdos cuando se cumplen condiciones .

- Comparado con sistemas tradicionales, blockchain aporta:
    - Mayor transparencia.
    - Eliminación de intermediarios en validación de datos.
    - Reducción de errores y fraudes en la gestión documental .
## Aplicaciones en Supply Chain e International Trade

El estudio analiza **ocho casos representativos** :

1. **Mercados descentralizados** (comercio P2P).
2. **Cartas de crédito basadas en blockchain** (trade finance).
3. **Pagos transfronterizos instantáneos**.
4. **Seguros marítimos** con datos compartidos en tiempo real.
5. **Trazabilidad y documentos de embarque** (ej. TradeLens de Maersk e IBM) .
6. **Certificados de origen electrónicos**.
7. **Prueba de autenticidad** de bienes de lujo y farmacéuticos .
8. **Trazabilidad de origen ético en alimentos** (ej. cadena de suministro sostenible).

## Artículo científico que hablan del tema 
1. Blockchain technology and its relationships to sustainable supply chain management
2. Sistema de trazabilidad de la cadena de suministro agroalimentario para cooperativas de frutas y hortalizas basado en la tecnología Blockchain
[Blockchain technology.pdf](https://github.com/user-attachments/files/22323988/Blockchain.technology.pdf)
[Sistema detrazabilidad.pdf](https://github.com/user-attachments/files/22323989/Sistema.detrazabilidad.pdf)
utiliza **tecnología blockchain** para mejorar la transparencia y la confianza entre productores, distribuidores y consumidores.
**Contexto y problema:**  
La creciente demanda de información sobre el origen y calidad de los alimentos, sumada a casos de fraude y certificaciones poco fiables, ha reducido la confianza de los consumidores. Las cooperativas, formadas por pequeños agricultores, necesitan demostrar el origen y las buenas prácticas de sus productos para ser competitivas en un mercado global.

**Propuesta tecnológica:**  
El estudio desarrolla una **Prueba de Concepto (PoC)** en una cooperativa de berries del sur de España. Mediante **Hyperledger Fabric** y **contratos inteligentes**, se registra en blockchain cada etapa del proceso: cultivo, recolección, manipulación, almacenamiento, transporte y venta. Sensores IoT, códigos QR/RFID y datos del ERP de la cooperativa alimentan la cadena de bloques, generando un **certificado digital único e inmutable** para cada lote de fruta.

**Ventajas del sistema:**

- **Transparencia y confianza:** todos los participantes (productores, certificadores, logística, retail y consumidores) pueden verificar en tiempo real la información del producto.

- **Seguridad y eficiencia:** los datos son inalterables y auditables, reducen fraudes y costos al eliminar intermediarios.

- **Competitividad:** mejora la reputación de las cooperativas y facilita su internacionalización.

- **Acceso público:** el consumidor puede escanear un código y conocer origen, fechas, tratamientos y condiciones de producción.


**Limitaciones y retos:**

- Escalabilidad: la prueba abarca pocos datos y un solo contrato inteligente; se requieren más pruebas para grandes volúmenes.

- Privacidad y regulación: compatibilidad con el Reglamento de Protección de Datos (GDPR) europeo.

- Fiabilidad de los datos iniciales: la tecnología no evita que alguien ingrese información falsa, aunque el uso de sensores reduce riesgos.

- Costos y conocimiento técnico: muchas cooperativas son pequeñas y necesitan apoyo para adoptar la solución.

## Evolución del tema 

El tema es muy nuevo recién se empieza a tocar desde el 2015 aproximadamente
<img width="1651" height="619" alt="Blockchain time" src="https://github.com/user-attachments/assets/9d8dff94-2531-48af-970c-083cc03803c4" />
## Comentarios 

La adopción de blockchain en las cadenas de suministro bolivianas representa una oportunidad estratégica para aumentar la competitividad, la sostenibilidad y la confianza de los mercados internacionales. Sectores clave como la agroindustria, la minería y la exportación de alimentos enfrentan hoy problemas de trazabilidad, altos costos logísticos y creciente presión de clientes que exigen certificaciones ambientales y sociales. La tecnología blockchain, con sus registros inmutables y contratos inteligentes, permite a productores y exportadores bolivianos garantizar el origen de productos como café de altura, cacao, quinua o carne, reducir fraudes y acelerar procesos de control sanitario, a la vez que mide huellas de carbono, consumo de agua y energía, requisitos cada vez más valorados en Europa y Norteamérica. El uso de sensores IoT integrados en blockchain facilitaría el monitoreo del transporte y la optimización de rutas en una geografía compleja, disminuyendo pérdidas poscosecha y costos de distribución; además, los smart contracts automatizarían pagos a pequeños productores y reducirían la dependencia de intermediarios financieros, favoreciendo la inclusión en zonas rurales. Sin embargo, para materializar estos beneficios Bolivia debe superar barreras importantes: escasa infraestructura digital en áreas rurales, falta de capital y de talento especializado en cooperativas y pymes, cultura de poca transparencia en el intercambio de datos y ausencia de un marco legal claro para contratos inteligentes y protección de datos. Para avanzar, se recomienda impulsar proyectos piloto en productos de alto valor de exportación, invertir en conectividad y capacitación técnica, crear estándares nacionales compatibles con normas internacionales de trazabilidad y sostenibilidad, y vincular estas iniciativas a fondos de financiamiento verde. Con el apoyo del Estado, la academia y el sector privado, blockchain puede convertirse no solo en una innovación tecnológica, sino en un instrumento de desarrollo que permita a Bolivia asegurar la calidad de sus productos, cumplir metas de sostenibilidad y posicionarse con ventaja en los mercados globales.







