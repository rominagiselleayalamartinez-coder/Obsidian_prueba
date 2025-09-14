
==Optimización de rutas, plataformas TMS,
blockchain para trazabilidad.==


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
[[Blockchain para trazabilidad]]

