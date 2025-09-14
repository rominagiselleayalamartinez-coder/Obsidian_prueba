Según lo investigado este tema es bastante moderno y uno de los libros que habla del tema es "Blockchain and the supply chain"

![[Libro Blockchain.png]]

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

![[Blockchain technology.pdf]]




![[Sistema detrazabilidad.pdf]]


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

![[Blockchain time.png]]

## Comentarios 

La adopción de blockchain en las cadenas de suministro bolivianas representa una oportunidad estratégica para aumentar la competitividad, la sostenibilidad y la confianza de los mercados internacionales. Sectores clave como la agroindustria, la minería y la exportación de alimentos enfrentan hoy problemas de trazabilidad, altos costos logísticos y creciente presión de clientes que exigen certificaciones ambientales y sociales. La tecnología blockchain, con sus registros inmutables y contratos inteligentes, permite a productores y exportadores bolivianos garantizar el origen de productos como café de altura, cacao, quinua o carne, reducir fraudes y acelerar procesos de control sanitario, a la vez que mide huellas de carbono, consumo de agua y energía, requisitos cada vez más valorados en Europa y Norteamérica. El uso de sensores IoT integrados en blockchain facilitaría el monitoreo del transporte y la optimización de rutas en una geografía compleja, disminuyendo pérdidas poscosecha y costos de distribución; además, los smart contracts automatizarían pagos a pequeños productores y reducirían la dependencia de intermediarios financieros, favoreciendo la inclusión en zonas rurales. Sin embargo, para materializar estos beneficios Bolivia debe superar barreras importantes: escasa infraestructura digital en áreas rurales, falta de capital y de talento especializado en cooperativas y pymes, cultura de poca transparencia en el intercambio de datos y ausencia de un marco legal claro para contratos inteligentes y protección de datos. Para avanzar, se recomienda impulsar proyectos piloto en productos de alto valor de exportación, invertir en conectividad y capacitación técnica, crear estándares nacionales compatibles con normas internacionales de trazabilidad y sostenibilidad, y vincular estas iniciativas a fondos de financiamiento verde. Con el apoyo del Estado, la academia y el sector privado, blockchain puede convertirse no solo en una innovación tecnológica, sino en un instrumento de desarrollo que permita a Bolivia asegurar la calidad de sus productos, cumplir metas de sostenibilidad y posicionarse con ventaja en los mercados globales.