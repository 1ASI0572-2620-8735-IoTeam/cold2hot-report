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

### 2.3.2. User Task Matrix.

### 2.3.3. User Journey Mapping.

### 2.3.4. Empathy Mapping.

## 2.4. Big Picture EventStorming.

## 2.5. Ubiquitous Language.

# Capítulo III: Requirements Specification

## 3.1. User Stories.

## 3.2. Impact Mapping.

## 3.3. Product Backlog.

# Capítulo IV: Solution Software Design

## 4.1. Strategic-Level Domain-Driven Design.

El diseño de nivel estratégico nos permite descomponer el dominio del negocio de logística y custodia térmica de delivery en subdominios delimitados (Bounded Contexts), asegurando una separación clara de responsabilidades y un lenguaje ubicuo consistente.

### 4.1.1. Design-Level EventStorming.
#### 4.1.1.1. Candidate Context Discovery.

A partir del análisis del dominio y de los eventos, comandos y agregados identificados en el Design-Level EventStorming, se identificaron cinco Bounded Contexts candidatos para el ecosistema Cold2Hot: **IAM**, **Container & Device Management**, **Thermal Monitoring & Telemetry**, **Access & Security**, y **Orders & Audit**. 

Cada uno de estos contextos agrupa capacidades del negocio con lenguaje ubicuo, reglas y responsabilidades propias, lo que garantiza una alta cohesión interna y un bajo acoplamiento en la arquitectura del sistema.

| Candidate Bounded Context | Purpose |
| :--- | :--- |
| **IAM (Identity & Access Management)** | Gestiona la autenticación, autorización, perfiles de usuario (repartidores, administradores) y sesiones de acceso. |
| **Container & Device Management** | Gestiona el inventario, registro, estado operativo y vinculación de los contenedores térmicos inteligentes (*SmartBoxes*) y sus sensores IoT. |
| **Thermal Monitoring & Telemetry** | Gestiona la lectura en tiempo real de temperatura, generación de historiales térmicos y alertas de desviación de temperatura. |
| **Access & Security** | Gestiona la validación de contraseñas de un solo uso (OTP), el control físico de apertura del contenedor y la detección de riesgos de alteración o manipulaciones no autorizadas. |
| **Orders & Audit** | Gestiona el seguimiento de pedidos asignados al contenedor, el registro de evidencias fotográficas de entrega y la generación de reportes de auditoría para los restaurantes/clientes. |

<div align="center">
    <img src="assets/Candidate Context Discovery.jpg" alt="Candidate Context Discovery" style="margin: 10px 0;" width="80%"/>
</div>

#### 4.1.1.2. Domain Message Flows Modeling.

En esta sección se modelan los principales flujos de mensajes del dominio entre los Bounded Contexts identificados en Cold2Hot. El objetivo es representar cómo se coordinan las capacidades del negocio y los eventos de dominio sin entrar aún en detalles de implementación técnica.

Mediante la técnica **Domain Storytelling**, se definió el flujo de interacción principal para el proceso de *Despacho, Transporte Seguro y Entrega de Pedido*:

1. **Creación de Orden y Perfil Térmico:** El *Administrador de Restaurante* crea la orden e indica las condiciones térmicas requeridas (Frío o Caliente). El contexto **Ordering & Dispatch** registra la orden y emite el evento `OrderDispatched`.
2. **Generación de OTP y Sincronización:** **Ordering & Dispatch** solicita al contexto **Access & Security** la generación de un código único de entrega (OTP). Este PIN se sincroniza localmente con el dispositivo IoT (**Edge / ESP32 Device**).
3. **Validación y Apertura en Destino:** Al llegar a la ubicación del cliente, el *Repartidor* ingresa el OTP en la **Delivery Operator App**, la cual valida el PIN con **Access & Security** (vía Bluetooth o API REST) para autorizar el desbloqueo físico del contenedor.
4. **Telemetría y Monitoreo Continuo:** De forma paralela, el contexto **IoT Telemetry** recibe la lectura continua de sensores (temperatura, Reed Switch, TCRT5000). Si detecta aperturas no autorizadas o desviaciones de temperatura, emite una alerta crítica hacia el sistema.
5. **Cierre de Entrega y Auditoría:** Una vez abierto el contenedor y entregado el pedido, el *Repartidor* captura la fotografía de evidencia desde la aplicación. El contexto **Auditing & Evidence** consolida las fotos, historiales térmicos y eventos de seguridad para dar por completada la orden

<div align="center">
    <img src="assets/Domain Message Flows Modeling.png" alt="Domain Message Flows Modeling" style="margin: 10px 0;" width="80%"/>
</div>

#### 4.1.1.3. Bounded Context Canvases.

A continuación se presentan los Bounded Context Canvases para cada uno de los cinco contextos delimitados identificados en el ecosistema Cold2Hot. Estos lienzos definen formalmente el propósito, el lenguaje ubicuo, las responsabilidades y los límites operacionales de cada módulo.

---

### 1. IAM (Identity & Access Management) Bounded Context

| Atributo | Descripción |
| :--- | :--- |
| **Name** | IAM (Identity & Access Management) |
| **Purpose** | Gestionar la autenticación, autorización, perfiles de usuarios (administradores, operadores/repartidores) y la emisión de tokens de acceso seguros. |
| **Domain Classification** | Supporting Subdomain |
| **Ubiquitous Language** | `User`, `Credentials`, `Role`, `JWT Token`, `Authentication`, `Permission`, `Operator Profile`. |
| **Inbound Messages / Commands** | `RegisterUser`, `AuthenticateUser`, `AssignRole`, `ValidateToken`. |
| **Outbound Messages / Events** | `UserRegistered`, `UserAuthenticated`, `RoleAssigned`. |
| **Aggregates & Entities** | **Aggregate Root:** `User` <br> **Entities:** `Role`, `Permission` <br> **Value Objects:** `UserId`, `Email`, `HashedPassword`, `RoleType`. |

---

### 2. Container & Device Management Bounded Context

| Atributo | Descripción |
| :--- | :--- |
| **Name** | Container & Device Management |
| **Purpose** | Administrar el ciclo de vida, registro, emparejamiento de sensores/actuadores y estado operativo de las cajas térmicas (*SmartBoxes*) y dispositivos ESP32. |
| **Domain Classification** | Supporting Subdomain |
| **Ubiquitous Language** | `SmartBox`, `ESP32 Device`, `Sensor Pairing`, `Actuator Calibration`, `Device State`, `Lock Mechanism`. |
| **Inbound Messages / Commands** | `RegisterSmartBox`, `PairSensor`, `UpdateDeviceStatus`, `CalibrateActuator`. |
| **Outbound Messages / Events** | `SmartBoxRegistered`, `SensorPaired`, `DeviceStatusUpdated`. |
| **Aggregates & Entities** | **Aggregate Root:** `SmartBox` <br> **Entities:** `DeviceSensor`, `Actuator` <br> **Value Objects:** `BoxId`, `MACAddress`, `FirmwareVersion`, `BoxStatus` (*Available, InTransit, Maintenance*). |

---

### 3. Thermal Monitoring & Telemetry Bounded Context

| Atributo | Descripción |
| :--- | :--- |
| **Name** | Thermal Monitoring & Telemetry |
| **Purpose** | Procesar en tiempo real la telemetría de temperatura transmitida por el hardware IoT, verificar rangos térmicos configurados y gatillar alertas de desviación. |
| **Domain Classification** | Core Subdomain |
| **Ubiquitous Language** | `Telemetry Stream`, `Thermal Profile`, `Temperature Reading`, `Threshold`, `Thermal Breach Alert`, `Historical Log`. |
| **Inbound Messages / Commands** | `IngestTelemetryData`, `SetThermalProfile`, `ProcessTemperatureReading`. |
| **Outbound Messages / Events** | `TelemetryIngested`, `ThermalProfileConfigured`, `ThermalBreachDetected`. |
| **Aggregates & Entities** | **Aggregate Root:** `ThermalProfile` <br> **Entities:** `TelemetryLog` <br> **Value Objects:** `TemperatureValue`, `CelsiusUnit`, `Timestamp`, `ThresholdRange`. |

---

### 4. Access & Security Bounded Context

| Atributo | Descripción |
| :--- | :--- |
| **Name** | Access & Security |
| **Purpose** | Generar y validar las claves OTP de un solo uso para la apertura del contenedor en destino, evaluar riesgos de manipulación indebida (*Tampering*) y controlar el mecanismo físico de bloqueo. |
| **Domain Classification** | Core Subdomain |
| **Ubiquitous Language** | `OTP (One-Time Password)`, `PIN Generation`, `Unlock Request`, `Tamper Detection`, `Reed Switch Alert`, `Security Event`. |
| **Inbound Messages / Commands** | `GenerateOTP`, `ValidateOTP`, `EvaluateTamperRisk`, `UnlockContainer`. |
| **Outbound Messages / Events** | `OTPGenerated`, `ContainerUnlocked`, `SecurityBreachDetected`, `InvalidOTPAttempted`. |
| **Aggregates & Entities** | **Aggregate Root:** `SecurityPasscode` <br> **Entities:** `AccessAttempt`, `SecurityLog` <br> **Value Objects:** `OTPCode`, `ExpirationTime`, `TamperStatus`, `UnlockResult`. |

---

### 5. Orders & Audit Bounded Context

| Atributo | Descripción |
| :--- | :--- |
| **Name** | Orders & Audit |
| **Purpose** | Orquestar la vinculación de pedidos con contenedores térmicos, consolidar la evidencia fotográfica de entrega y estructurar los reportes de auditoría de custodia térmica. |
| **Domain Classification** | Core Subdomain |
| **Ubiquitous Language** | `Order`, `Thermal Custody`, `Delivery Evidence`, `Proof of Delivery`, `Audit Report`, `Dispatch`. |
| **Inbound Messages / Commands** | `AssignOrderToBox`, `CaptureDeliveryEvidence`, `UploadDeliveryPhoto`, `GenerateAuditReport`. |
| **Outbound Messages / Events** | `OrderDispatched`, `EvidenceUploaded`, `AuditReportGenerated`, `OrderCompleted`. |
| **Aggregates & Entities** | **Aggregate Root:** `Order` <br> **Entities:** `DeliveryEvidence`, `AuditReport` <br> **Value Objects:** `OrderId`, `PhotoUrl`, `CustodyStatus`, `CompletionTimestamp`. |

### 4.1.2. Context Mapping.

El Context Map de Cold2Hot representa la arquitectura y las interacciones entre los Bounded Contexts identificados en el dominio del sistema de monitoreo térmico y de dispositivos. Esta vista describe las responsabilidades específicas de cada contexto y las relaciones de dependencia (Upstream/Downstream) necesarias para la comunicación entre subsistemas.

En esta arquitectura, el contexto IAM (Identity & Access Management) actúa como proveedor principal de identidades y autenticación para todo el sistema. Por su parte, Thermal Monitoring & Telemetry consume información crítica de dispositivos y accesos para registrar datos biométricos o de temperatura en tiempo real.

<div align="center">
    <img src="assets/Context Mapping.png" alt="Context Mapping" style="margin: 10px 0;" width="80%"/>
</div>

### 4.1.3. Software Architecture.

#### 4.1.3.1. Software Architecture System Landscape Diagram.

El diagrama de panorama del sistema (System Landscape Diagram) ilustra el ecosistema tecnológico y operativo completo dentro del cual opera la startup IoTeam. Permite visualizar la interacción entre los diferentes actores humanos, el sistema central y las plataformas satélites que intervienen en la cadena logística de entrega de comida a domicilio.

En este nivel macro, el proceso inicia cuando el End Customer realiza una solicitud de pedido mediante los canales comerciales del restaurante aliado. El Restaurant Branch Manager registra y despacha la comanda a través del Restaurant POS & ERP System, el cual se comunica con Cold2Hot IoT Platform para transferir la orden y definir los requerimientos térmicos de conservación (modo frío o caliente).

A partir de ese instante, la plataforma coordina la operación con el Delivery Courier, quien recibe la ruta optimizada mediante el servicio de cartografía libre OpenStreetMap & OSRM API. El repartidor interactúa mecánicamente con el dispositivo físico SmartBox IoT Physical Device, introduciendo el pedido en el compartimento térmico. Durante el trayecto, la plataforma Cold2Hot mantiene comunicación constante con el hardware para recibir telemetría continua y detectar cualquier eventualidad. En caso de identificar una apertura no autorizada o un desvío de temperatura crítico, la plataforma dispara alertas en tiempo real al teléfono del repartidor y al panel del administrador mediante Firebase Cloud Messaging (FCM). Finalmente, la evidencia fotográfica capturada al concretar la entrega se comprime y almacena de forma segura en Cloudinary Free Tier.

<div align="center">
    <img src="assets/SystemLandscape-diagram.png" alt="Sytem Landscape Diagram" style="margin: 10px 0;" width="80%"/>
</div>

#### 4.1.3.2. Software Architecture Context Level Diagrams.

El diagrama de contexto (Context Diagram) delimita formalmente la frontera perimetral del software de Cold2Hot IoT Platform System, representándolo como una caja negra central e identificando exclusivamente a sus usuarios directos y a los sistemas con los que establece enlaces de comunicación síncrona o asíncrona.

A diferencia del panorama global, en esta vista el foco se concentra en el sistema de software desarrollado por IoTeam:

- Delivery Operations Administrator: Interactúa con la plataforma a través de canales seguros HTTPS/TLS para configurar rangos térmicos admisibles, monitorear la ubicación de la flota y auditar incidentes o aperturas registradas durante los envíos.

- Delivery Operator: Se autentica en el sistema mediante su dispositivo móvil para sincronizar órdenes asignadas, validar códigos de apertura de un solo uso (OTP) y enviar las fotografías que acreditan la entrega exitosa del paquete.

- SmartBox IoT Hardware Enclosure: Representa el entorno ciberfísico en ruta (microcontrolador ESP32 NodeMCU, bus One-Wire con sensor DS18B20, entradas digitales para Reed Switch y TCRT5000, actuador de ventilación y cerrojo mecánico solenoide). Este dispositivo actúa como un sistema externo que transmite flujos continuos de telemetría y eventos de intrusión vía serial o Bluetooth Low Energy (BLE), y recibe órdenes de desbloqueo físico emitidas por el software.

- Sistemas Externos de Soporte: El sistema delega responsabilidades no troncales consumiendo las APIs REST gratuitas de OpenStreetMap & OSRM para la geolocalización, Firebase Cloud Messaging para la emisión de notificaciones push prioritarias, y Cloudinary para la persistencia y distribución de archivos multimedia de auditoría.

<div align="center">
    <img src="assets/Contex-diagram.png" alt="Context Diagram" style="margin: 10px 0;" width="80%"/>
</div>

#### 4.1.3.2. Software Architecture Container Level Diagrams.

El diagrama de contenedores descompone el sistema Cold2Hot en sus unidades fundamentales de ejecución y despliegue desacopladas, definiendo las responsabilidades funcionales, las tecnologías seleccionadas y los protocolos de integración entre cada bloque:

- Landing Page: Sitio web estático desarrollado con HTML5, CSS3 y JavaScript vanilla. Su función principal es exponer la propuesta de valor comercial de IoTeam, planes de suscripción para restaurantes y enlaces de redirección hacia las aplicaciones operativas. 

- Delivery Admin Web Application: Aplicación web cliente desarrollada con Angular y TypeScript, estructurada bajo el sistema de diseño Material Design mediante la biblioteca Angular Material. Proporciona a los administradores un panel de control interactivo para la gestión de despachos, visualización de métricas térmicas y auditoría de incidentes.

- Delivery Operator Mobile Application: Aplicación móvil multiplataforma desarrollada con Flutter y Dart. Permite al conductor autenticarse, enlazarse vía Bluetooth Low Energy (BLE) con la SmartBox más cercana, digitar el PIN OTP de apertura y tomar la fotografía de comprobación física.

- Cloud Core RESTful API: Servicio backend empresarial desarrollado sobre el marco de trabajo Spring Boot en Java. Centraliza las reglas de negocio globales, gestiona la persistencia de datos, valida accesos e identidades (IAM) y orquesta la comunicación con los servicios externos gratuitos (FCM, Cloudinary, OSRM).

- Cloud Relational Database: Instancia de base de datos relacional PostgreSQL que almacena los registros de usuarios, configuraciones de cajas térmicas, historiales de pedidos y eventos de auditoría.

- Edge Service: Microservicio intermedio desarrollado en Python utilizando el microframework Flask y Peewee ORM. Se ejecuta en el hardware del contenedor para procesar señales analíticas locales, evaluar discrepancias inmediatas de seguridad y garantizar la operación de desbloqueo incluso en escenarios con pérdida total de conectividad a internet.

- Edge Local Database: Base de datos relacional ligera basada en SQLite que almacena en caché local las claves temporales activas y los últimos registros de telemetría pendientes de sincronización con la nube.

<div align="center">
    <img src="assets/Containers-diagram.png" alt="Containers Diagram" style="margin: 10px 0;" width="80%"/>
</div>

#### 4.1.3.3. Software Architecture Deployment Diagrams.

El diagrama de despliegue detalla la topología de infraestructura física y en la nube donde residen los contenedores de software en un entorno de producción, garantizando alta disponibilidad con costes controlados mediante esquemas Free Tier:

- Estación de Trabajo del Administrador (Hardware de Escritorio): Los administradores acceden a través de navegadores web estándar (Chrome, Firefox, Safari o Edge) a la Landing Page y a la Delivery Admin Web Application, las cuales son servidas de manera estática y con certificados SSL activos mediante la plataforma PaaS gratuita de Vercel o GitHub Pages.

- Dispositivo Móvil del Repartidor (Smartphone Android/iOS): Aloja localmente la Delivery Operator Mobile Application instalada. El teléfono se comunica simultáneamente con la nube mediante HTTPS/4G-5G y con la SmartBox a través de su antena Bluetooth Low Energy (BLE).

- Gabinete Físico SmartBox (Entorno Edge e IoT en Vehículo): Compuesto por un computador de placa reducida (SoC Linux) que hospeda el Edge Service y la base de datos SQLite, interconectado por comunicación serial UART/GPIO al microcontrolador ESP32 NodeMCU, el cual gestiona directamente los pines de los sensores DS18B20, TCRT5000, Reed Switch y el relé de apertura.

- Infraestructura Cloud Gratuita (PaaS / BaaS):

    - El Cloud Core RESTful API opera en un contenedor virtualizado dentro de los servicios gratuitos de Render Free Web Service.   

    - La persistencia transaccional reside en una base de datos gestionada PostgreSQL provista por el nivel gratuito de Supabase.

    - El repositorio multimedia de evidencias opera bajo la capa gratuita de Cloudinary, la cual almacena las capturas optimizadas sin consumo de disco en el servidor principal. 

<div align="center">
    <img src="assets/ProductionDeployment-Diagram.png" alt="Deployment Diagram" style="margin: 10px 0;" width="80%"/>
</div>

## 4.2. Tactical-Level Domain-Driven Design

### 4.2.1. Bounded Context: Identity & Access (IAM)

El contexto delimitado IAM gestiona integralmente el registro, autenticación, autorización y emisión de credenciales criptográficas para todos los actores que interactúan con la plataforma Cold2Hot. Asegura la separación de privilegios entre los administradores de operaciones del restaurante y los operadores de entrega (repartidores), garantizando un acceso restringido y trazable a los recursos del sistema.

#### 4.2.1.1. Domain Layer.

#### 4.2.1.2. Interface Layer.

#### 4.2.1.3. Application Layer.

#### 4.2.1.4. Infrastructure Layer.

#### 4.2.1.5. Bounded Context Software Architecture Component Level Diagrams.

El diagrama de componentes (C4 Nivel 3) ilustra la organización estructural interna del contenedor backend Cloud Core RESTful API para dar soporte al contexto IAM. Refleja el flujo de llamadas desde las aplicaciones cliente hacia los controladores REST, la delegación hacia los manejadores de comandos de la capa de aplicación, la invocación de las entidades del modelo de dominio y la resolución técnica de persistencia ejecutada por los repositorios hacia la base de datos relacional MySQL.

<div align="center">
    <img src="assets/IAM_Component_Diagram.png" alt="IAM Components diagram" style="margin: 10px 0;" width="80%"/>
</div>

#### 4.2.1.6. Bounded Context Software Architecture Code Level Diagrams.

##### 4.2.1.6.1. Bounded Context Domain Layer Class Diagrams.

##### 4.2.1.6.2. Bounded Context Database Design Diagram.

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
