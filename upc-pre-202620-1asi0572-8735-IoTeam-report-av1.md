<div align="center">

<p align="center">
  <img src="assets/upc_logo.png" alt="logo" width="200"/>
</p>

<h3 align="center">
Universidad Peruana de Ciencias Aplicadas
</h3>

<h3 align="center">
Ingeniería de Software
<br><br>
Ciclo: 2026-20
<br><br>
1ASI0572 - Desarrollo de Soluciones IOT
<br><br>
NRC: 8735
<br><br>
Docente: Leon Bacca, Marco Antonio
<br><br>
<strong>Informe de Trabajo Final</strong>  
<br><br>
Startup: IoTeam
<br><br>
Producto: Cold2Hot  
<br><br>
<br><br>
<strong>Integrantes</strong>  
<br><br>
Alvarado De La Cruz , Juan Carlos (U202216150) 
<br><br>
Carhuancote Dominguez, Gonzalo Alonso (U202210720) 
<br><br>
Diestra Zambrano, Adriana Maria (U202218110)
<br><br>
Duran Diaz, Antonio Rodrigo (U202215721)
<br><br>
Nakasone Gomes, Marco Antonio (U202210790)
<br><br>
Shimabukuro Uku, Carlos Joel (U201912407)
<br><br>
Teves Samaniego, Joan Fernando (U202117303)
<br><br>
<br>

**Septiembre - 2026**

</h3>
</div>

# Contenido

## Tabla de contenidos

# Student Outcome

# Capítulo I: Introducción

## 1.1. Startup Profile

### 1.1.1. Descripción de la Startup

### 1.1.2. Perfiles de integrantes del equipo

## 1.2. Solution Profile

### 1.2.1 Antecedentes y problemática

### 1.2.2 Lean UX Process.

#### 1.2.2.1. Lean UX Problem Statements.

#### 1.2.2.2. Lean UX Assumptions.

#### 1.2.2.3. Lean UX Hypothesis Statements.

#### 1.2.2.4. Lean UX Canvas.

## 1.3. Segmentos objetivo.

# Capítulo II: Requirements Elicitation & Analysis

## 2.1. Competidores.

### 2.1.1. Análisis competitivo.

### 2.1.2. Estrategias y tácticas frente a competidores.

## 2.2. Entrevistas.

### 2.2.1. Diseño de entrevistas.

### 2.2.2. Registro de entrevistas.

### 2.2.3. Análisis de entrevistas.

## 2.3. Needfinding.

### 2.3.1. User Personas.

Con el propósito de garantizar una comprensión profunda y precisa de los segmentos identificados como clave para nuestro proyecto, hemos llevado a cabo un proceso estructurado y cuidadoso de creación de User Personas. Este procedimiento nos permitió definir un perfil específico y representativo para cada segmento objetivo, lo que nos brinda una perspectiva más clara y detallada de nuestros usuarios. De esta manera, podemos diseñar y ofrecer soluciones que respondan de manera efectiva a sus necesidades, expectativas y contextos particulares.

UserPersona 1
<img src="./assets/Carlos_Mendoza.png">

UserPersona 2
<img src="./assets/Miguel_Torres.png">

### 2.3.2. User Task Matrix

El User Task Matrix concentra las tareas que los User Persona, que representan a los segmentos principales de Cold2Hot, realizan para cumplir sus objetivos dentro de la cadena logística de entregas de última milla. En este caso, se consideran dos segmentos de usuarios:

* **Administradores de operaciones de delivery**, encargados de la gestión del local, control de despachos y auditoría de incidencias.
* **Operadores de entrega (repartidores)**, responsables del transporte urbano, cumplimiento de rutas y entrega final al cliente.

Es importante destacar que las tareas (tasks) reflejan actividades que los usuarios realizan independientemente de la existencia del software, es decir, forman parte natural de su día a día y no representan características o funciones del sistema.

**Indicadores de Importancia y Frecuencia**

*Indicadores de Importancia:*
* **ALTA →** La tarea es crítica para el cumplimiento de los objetivos del usuario.
* **MEDIA →** La tarea es importante pero no afecta directamente el resultado global.
* **BAJA →** La tarea aporta valor complementario o se realiza ocasionalmente.

*Indicadores de Frecuencia:*
* **ALTA →** Se realiza de manera constante o diaria.
* **MEDIA →** Se realiza semanal o mensualmente.
* **BAJA →** Se realiza esporádicamente o en circunstancias específicas.

**Tabla de Matriz de Tareas de Usuario**

| Tareas | Administradores de Delivery | Operadores de Entrega | Frecuencia | Importancia | Frecuencia | Importancia |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Empacar y preparar el pedido | Alta | Baja | Alta | Alta | Baja | Baja |
| Asegurar / bloquear el contenedor de transporte | Alta | Alta | Alta | Alta | Alta | Alta |
| Transportar pedidos en entorno urbano | Nunca | Alta | - | - | Alta | Alta |
| Revisar estado físico del paquete en ruta | Nunca | Alta | - | - | Alta | Alta |
| Verificar la temperatura del alimento | Media | Baja | Media | Alta | Baja | Media |
| Resolver incidentes de aperturas accidentales | Media | Alta | Media | Alta | Alta | Alta |
| Desbloquear contenedor en el destino | Nunca | Alta | - | - | Alta | Alta |
| Registrar foto de evidencia de la entrega | Baja | Alta | Baja | Media | Alta | Alta |
| Monitorear flota de despachos en tiempo real | Alta | Nunca | Alta | Alta | - | - |
| Auditar tiempos de entrega e incidencias | Media | Baja | Media | Alta | Baja | Baja |
| Conciliar pagos y penalizaciones de plataformas | Media | Media | Media | Alta | Media | Alta |

**Análisis de Tareas**

*Tareas con mayor frecuencia e importancia*
Tanto administradores como repartidores presentan alta frecuencia e importancia en tareas como: **Asegurar/bloquear el contenedor de transporte** y la **resolución de incidentes de aperturas accidentales**. Estas tareas reflejan la necesidad crítica de mantener la cadena de custodia y proteger la carga ante las condiciones del tránsito urbano.

*Principales diferencias entre segmentos de usuarios*
* **Monitoreo y Auditoría:** Tiene alta frecuencia e importancia para los administradores, ya que su rentabilidad depende de verificar el estado de los despachos; para los repartidores, el monitoreo propio es nulo.
* **Transporte y evidencia:** Es una tarea de importancia alta y exclusiva para los repartidores (manejar y tomar la foto de entrega), mientras que el administrador solo consume esa información a posteriori.
* **Empaque y preparación:** Es esencial y frecuente para los administradores de restaurantes, mientras que los repartidores reciben el producto ya finalizado.

*Principales similitudes*
Ambos segmentos coinciden en la alta importancia de **evitar penalizaciones**. El administrador busca evitar devoluciones por comida fría, y el repartidor busca evitar descuentos salariales por quejas injustas. Esto demuestra la necesidad compartida de un sistema (como Cold2Hot) que garantice la trazabilidad térmica y ofrezca evidencia auditable del cierre del pedido.

*Enfoque de los segmentos*
Los **administradores** se enfocan en el control centralizado, la reducción de mermas y la visibilidad remota de sus envíos. Los **repartidores**, en cambio, priorizan la agilidad en la conducción, la reducción de fricciones al abrir/cerrar la mochila y contar con pruebas digitales para deslindar responsabilidades frente a los clientes. Aunque abordan la logística desde distintas veredas, ambos buscan el mismo objetivo final: una entrega exitosa, rápida y sin disputas posteriores.

### 2.3.3. User Journey Mapping.

User Journey Mapping - Segmento Administrador de operaciones de delivery
<img src="./assets/Customer _journey_map_1.png">

User Journey Mapping - Segmento Operador de entrega
<img src="./assets/Customer_journey_map_2.png">

### 2.3.4. Empathy Mapping.

Segmento 1: Administradores de operaciones de delivery preocupados por la rentabilidad y la trazabilidad de los pedidos
<img src="./assets/Empathy_map.png">

Segmento 2: Operadores de entrega (motorizados) enfocados en la agilidad y en proteger sus ingresos de penalizaciones injustas
<img src="./assets/Empathy_map2.png">
## 2.4. Big Picture EventStorming.

<img src="./assets/EventStorming.jpg">

## 2.5. Ubiquitous Language.

| Term (English) | Término (Español) | Definition (Definición en español) |
| :--- | :--- | :--- |
| Smart Box | Caja Inteligente | Contenedor físico para delivery equipado con hardware IoT (ESP32, sensores y regulador) que mantiene la cadena de custodia. |
| Thermal Profile | Perfil Térmico | Configuración específica (modo Frío o Calor) asignada remotamente al ESP32 para regular la temperatura del interior. |
| Access Code / PIN | Código de Acceso | Clave numérica única generada por el sistema que el repartidor utiliza en su App para desbloquear la caja en el destino. |
| Dispatch Hub | Panel de Despacho | Interfaz web utilizada por el administrador para asignar pedidos, configurar la temperatura y monitorear la flota en tiempo real. |
| Telemetry | Telemetría | Datos de temperatura y estado de la batería enviados continuamente por el ESP32 hacia el servidor durante el trayecto. |
| Magnetic Sensor | Sensor Magnético | Componente de hardware (Reed Switch) que detecta el estado físico de la tapa de la caja (abierta/cerrada). |
| Infrared Sensor | Sensor Infrarrojo | Componente de hardware (TCRT5000) utilizado para detectar la presencia o ausencia del paquete dentro del contenedor. |
| Two-Level Security | Seguridad de Dos Niveles | Lógica del sistema que cruza los datos magnéticos e infrarrojos para distinguir entre una caja mal cerrada y una extracción real. |
| Preventive Alert | Alerta Preventiva | Notificación enviada al repartidor para que ajuste la tapa si la caja se desajusta accidentalmente sin extraerse el pedido. |
| Critical Alert | Alerta Crítica | Notificación enviada al administrador indicando que el pedido fue extraído de la caja en pleno tránsito, sugiriendo manipulación. |
| Delivery Evidence | Evidencia de Entrega | Fotografía obligatoria tomada por el repartidor desde la App tras abrir la caja, que certifica el estado del paquete al entregarlo. |
| Audit Report | Reporte de Auditoría | Registro inmutable de una entrega finalizada que incluye marcas de tiempo, gráfica térmica y evidencia fotográfica para resolver disputas. |
| Route Monitoring | Monitoreo en Ruta | Seguimiento GPS combinado con la telemetría térmica visible desde el panel de administración. |
| Delivery Courier | Operador de Entrega | Persona (motorizado o ciclista) encargada del transporte físico del contenedor desde el restaurante hasta el cliente. |

# Capítulo III: Requirements Specification

## 3.1. User Stories.

## 3.2. Impact Mapping.

## 3.3. Product Backlog.

# Capítulo IV: Solution Software Design

## 4.1. Strategic-Level Domain-Driven Design.

### 4.1.1. Design-Level EventStorming.

#### 4.1.1.1 Candidate Context Discovery.

#### 4.1.1.2 Domain Message Flows Modeling.

#### 4.1.1.3 Bounded Context Canvases.

### 4.1.2. Context Mapping.

### 4.1.3. Software Architecture.

#### 4.1.3.1. Software Architecture System Landscape Diagram.

#### 4.1.3.2. Software Architecture Context Level Diagrams.

#### 4.1.3.2. Software Architecture Container Level Diagrams.

#### 4.1.3.3. Software Architecture Deployment Diagrams.

## 4.2. Tactical-Level Domain-Driven Design

### 4.2.X. Bounded Context: <Bounded Context Name>

#### 4.2.X.1. Domain Layer.

#### 4.2.X.2. Interface Layer.

#### 4.2.X.3. Application Layer.

#### 4.2.X.4. Infrastructure Layer.

#### 4.2.X.5. Bounded Context Software Architecture Component Level Diagrams.

#### 4.2.X.6. Bounded Context Software Architecture Code Level Diagrams.

##### 4.2.X.6.1. Bounded Context Domain Layer Class Diagrams.

##### 4.2.X.6.2. Bounded Context Database Design Diagram.

# Capítulo V: Solution UI/UX Design

## 5.1. Style Guidelines.

### 5.1.1. General Style Guidelines.

### 5.1.2. Web, Mobile and IoT Style Guidelines.

## 5.2. Information Architecture.

### 5.2.1. Organization Systems.

### 5.2.2. Labeling Systems.

### 5.2.3. SEO Tags and Meta Tags

### 5.2.4. Searching Systems.

### 5.2.5. Navigation Systems.

## 5.3. Landing Page UI Design.

### 5.3.1. Landing Page Wireframe.

### 5.3.2. Landing Page Mock-up.

## 5.4. Applications UX/UI Design.

### 5.4.1. Applications Wireframes.

### 5.4.2. Applications Wireflow Diagrams.

### 5.4.2. Applications Mock-ups.

### 5.4.3. Applications User Flow Diagrams.

## 5.5. Applications Prototyping.

## 5.6. IoT Device Design.

# Capítulo VI: Product Implementation, Validation & Deployment

## 6.1. Software Configuration Management.

### 6.1.1. Software Development Environment Configuration.

### 6.1.2. Source Code Management.

### 6.1.3. Source Code Style Guide & Conventions.

### 6.1.4. Software Deployment Configuration.

## 6.2. Landing Page, Services & Applications Implementation.

### 6.2.X. Sprint n

#### 6.2.X.1. Sprint Planning n.

#### 6.2.X.2. Aspect Leaders and Collaborators.

#### 6.2.X.3. Sprint Backlog n.

#### 6.2.X.4. Development Evidence for Sprint Review.

#### 6.2.X.5. Testing Suite Evidence for Sprint Review.

#### 6.2.X.6. Execution Evidence for Sprint Review.

#### 6.2.X.7. Services Documentation Evidence for Sprint Review.

#### 6.2.X.8. Software Deployment Evidence for Sprint Review.

#### 6.2.X.9. Team Collaboration Insights during Sprint.

## 6.3. Validation Interviews.

### 6.3.1. Diseño de Entrevistas.

### 6.3.2. Registro de Entrevistas.

### 6.3.3. Evaluaciones según heurísticas.

## 6.4. Video About-the-Product.

# Conclusiones

## Conclusiones y recomendaciones.

# Video About-the-Team.

# Bibliografía

# Anexos
