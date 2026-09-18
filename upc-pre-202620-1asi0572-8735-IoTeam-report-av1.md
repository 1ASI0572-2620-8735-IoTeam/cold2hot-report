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

- [Registro de versiones del informe](#registro-de-versiones-del-informe)

- [Project Report Collaboration Insights](#project-report-collaboration-insights)

- [Contenido](#contenido)

- [Student Outcome](#student-outcome)

- [Capítulo I: Introducción](#capitulo-i-introduccion)
  - [1.1. Startup Profile](#11-startup-profile)
    - [1.1.1. Descripción de la Startup](#111-descripción-de-la-startup)
    - [1.1.2. Perfiles de integrantes del equipo](#112-perfiles-de-integrantes-del-equipo)
  - [1.2. Solution Profile](#12-solution-profile)
    - [1.2.1 Antecedentes y problemática](#121-antecedentes-y-problemática)
    - [1.2.2. Lean UX Process](#122-lean-ux-process)
      - [1.2.2.1. Lean UX Problem Statements](#1221-lean-ux-problem-statements)
      - [1.2.2.2. Lean UX Assumptions](#1222-lean-ux-assumptions)
      - [1.2.2.3. Lean UX Hypothesis Statements](#1223-lean-ux-hypothesis-statements)
      - [1.2.2.4. Lean UX Canvas](#1224-lean-ux-canvas)
  - [1.3. Segmentos objetivo](#13-segmentos-objetivo)

- [Capítulo II: Requirements Elicitation & Analysis](#capitulo-ii-requirements-elicitation--analysis)
  - [2.1. Competidores](#21-competidores)
    - [2.1.1. Análisis competitivo](#211-análisis-competitivo)
    - [2.1.2. Estrategias y tácticas frente a competidores](#212-estrategias-y-tácticas-frente-a-competidores)
  - [2.2. Entrevistas](#22-entrevistas)
    - [2.2.1. Diseño de entrevistas](#221-diseño-de-entrevistas)
    - [2.2.2. Registro de entrevistas](#222-registro-de-entrevistas)
    - [2.2.3. Análisis de entrevistas](#223-análisis-de-entrevistas)
  - [2.3. Needfinding](#23-needfinding)
    - [2.3.1. User Personas](#231-user-personas)
    - [2.3.2. User Task Matrix](#232-user-task-matrix)
    - [2.3.3. User Journey Mapping](#233-user-journey-mapping)
    - [2.3.4. Empathy Mapping](#234-empathy-mapping)
  - [2.4. Big Picture EventStorming](#24-big-picture-eventstorming)
  - [2.5. Ubiquitous Language](#25-ubiquitous-language)

- [Capítulo III: Requirements Specification](#capitulo-iii-requirements-specification)
  - [3.1. User Stories](#31-user-stories)
  - [3.2. Impact Mapping](#32-impact-mapping)
  - [3.3. Product Backlog](#33-product-backlog)

- [Capítulo IV: Solution Software Design](#capitulo-iv-solution-software-design)
  - [4.1. Strategic-Level Domain-Driven Design](#41-strategic-level-domain-driven-design)
    - [4.1.1. Design-Level EventStorming](#411-design-level-eventstorming)
      - [4.1.1.1 Candidate Context Discovery](#4111-candidate-context-discovery)
      - [4.1.1.2 Domain Message Flows Modeling](#4112-domain-message-flows-modeling)
      - [4.1.1.3 Bounded Context Canvases](#4113-bounded-context-canvases)
    - [4.1.2. Context Mapping](#412-context-mapping)
    - [4.1.3. Software Architecture](#413-software-architecture)
      - [4.1.3.1. Software Architecture System Landscape Diagram](#4131-software-architecture-system-landscape-diagram)
      - [4.1.3.2. Software Architecture Context Level Diagrams](#4132-software-architecture-context-level-diagrams)
      - [4.1.3.2. Software Architecture Container Level Diagrams](#4132-software-architecture-container-level-diagrams)
      - [4.1.3.3. Software Architecture Deployment Diagrams](#4133-software-architecture-deployment-diagrams)
  - [4.2. Tactical-Level Domain-Driven Design](#42-tactical-level-domain-driven-design)
    - [4.2.X. Bounded Context: \<Bounded Context Name\>](#42x-bounded-context-bounded-context-name)
      - [4.2.X.1. Domain Layer](#42x1-domain-layer)
      - [4.2.X.2. Interface Layer](#42x2-interface-layer)
      - [4.2.X.3. Application Layer](#42x3-application-layer)
      - [4.2.X.4. Infrastructure Layer](#42x4-infrastructure-layer)
      - [4.2.X.5. Bounded Context Software Architecture Component Level Diagrams](#42x5-bounded-context-software-architecture-component-level-diagrams)
      - [4.2.X.6. Bounded Context Software Architecture Code Level Diagrams](#42x6-bounded-context-software-architecture-code-level-diagrams)
        - [4.2.X.6.1. Bounded Context Domain Layer Class Diagrams](#42x61-bounded-context-domain-layer-class-diagrams)
        - [4.2.X.6.2. Bounded Context Database Design Diagram](#42x62-bounded-context-database-design-diagram)

- [Capítulo V: Solution UI/UX Design](#capitulo-v-solution-uiux-design)
  - [5.1. Style Guidelines](#51-style-guidelines)
    - [5.1.1. General Style Guidelines](#511-general-style-guidelines)
    - [5.1.2. Web, Mobile and IoT Style Guidelines](#512-web-mobile-and-iot-style-guidelines)
  - [5.2. Information Architecture](#52-information-architecture)
    - [5.2.1. Organization Systems](#521-organization-systems)
    - [5.2.2. Labeling Systems](#522-labeling-systems)
    - [5.2.3. SEO Tags and Meta Tags](#523-seo-tags-and-meta-tags)
    - [5.2.4. Searching Systems](#524-searching-systems)
    - [5.2.5. Navigation Systems](#525-navigation-systems)
  - [5.3. Landing Page UI Design](#53-landing-page-ui-design)
    - [5.3.1. Landing Page Wireframe](#531-landing-page-wireframe)
    - [5.3.2. Landing Page Mock-up](#532-landing-page-mock-up)
  - [5.4. Applications UX/UI Design](#54-applications-uxui-design)
    - [5.4.1. Applications Wireframes](#541-applications-wireframes)
    - [5.4.2. Applications Wireflow Diagrams](#542-applications-wireflow-diagrams)
    - [5.4.2. Applications Mock-ups](#542-applications-mock-ups)
    - [5.4.3. Applications User Flow Diagrams](#543-applications-user-flow-diagrams)
  - [5.5. Applications Prototyping](#55-applications-prototyping)
  - [5.6. IoT Device Design](#56-iot-device-design)

- [Capítulo VI: Product Implementation, Validation & Deployment](#capitulo-vi-product-implementation-validation--deployment)
  - [6.1. Software Configuration Management](#61-software-configuration-management)
    - [6.1.1. Software Development Environment Configuration](#611-software-development-environment-configuration)
    - [6.1.2. Source Code Management](#612-source-code-management)
    - [6.1.3. Source Code Style Guide & Conventions](#613-source-code-style-guide--conventions)
    - [6.1.4. Software Deployment Configuration](#614-software-deployment-configuration)
  - [6.2. Landing Page, Services & Applications Implementation](#62-landing-page-services--applications-implementation)
    - [6.2.X. Sprint n](#62x-sprint-n)
      - [6.2.X.1. Sprint Planning n](#62x1-sprint-planning-n)
      - [6.2.X.2. Aspect Leaders and Collaborators](#62x2-aspect-leaders-and-collaborators)
      - [6.2.X.3. Sprint Backlog n](#62x3-sprint-backlog-n)
      - [6.2.X.4. Development Evidence for Sprint Review](#62x4-development-evidence-for-sprint-review)
      - [6.2.X.5. Testing Suite Evidence for Sprint Review](#62x5-testing-suite-evidence-for-sprint-review)
      - [6.2.X.6. Execution Evidence for Sprint Review](#62x6-execution-evidence-for-sprint-review)
      - [6.2.X.7. Services Documentation Evidence for Sprint Review](#62x7-services-documentation-evidence-for-sprint-review)
      - [6.2.X.8. Software Deployment Evidence for Sprint Review](#62x8-software-deployment-evidence-for-sprint-review)
      - [6.2.X.9. Team Collaboration Insights during Sprint](#62x9-team-collaboration-insights-during-sprint)
  - [6.3. Validation Interviews](#63-validation-interviews)
    - [6.3.1. Diseño de Entrevistas](#631-diseño-de-entrevistas)
    - [6.3.2. Registro de Entrevistas](#632-registro-de-entrevistas)
    - [6.3.3. Evaluaciones según heurísticas](#633-evaluaciones-según-heurísticas)
  - [6.4. Video About-the-Product](#64-video-about-the-product)

- [Conclusiones](#conclusiones)
  - [Conclusiones y recomendaciones](#conclusiones-y-recomendaciones)

- [Video About-the-Team](#video-about-the-team)

- [Bibliografía](#bibliografía)

- [Anexos](#anexos)


# Student Outcome

# Capítulo I: Introducción

## 1.1. Startup Profile

### 1.1.1. Descripción de la Startup

IoTeam es una startup tecnológica que busca resolver un problema cotidiano y lograr que la comida a domicilio llegue en buenas condiciones. Para ello nos enfoncamos en crear una solución basada en Internet de las Cosas (IoT) para cuidar los pedidos durante su trayecto hasta llegar a la puerta del cliente.

* Misión: Que cada pedido de comida llegue tan bueno como salió del restaurante, cuidando su temperatura y seguridad durante todo el camino.
* Visión: Convertirnos en un referente en Latinoamérica para la tecnología con enfoque en IoT aplicada al delivery de comida, ayudando a que restaurantes y repartidores trabajen con más confianza.
* Valores: Innovación, calidad de servicio, cuidado del medio ambiente, seguridad y, sobre todo, pensar siempre en la experiencia del cliente final

### 1.1.2. Perfiles de integrantes del equipo

| Integrante | Descripcion de Carrera | Conocimientos y Habilidades a apuntar |
| --------------------------------| ----------------------| ------------------------------------ |
| ![Juan Carlos](./assets/foto-juan.jpg) <br> Alvarado De La Cruz, Juan Carlos | Ingeniería de Software <br>Universidad Peruana de Ciencias Aplicadas | Descripcion |
| ![Gonzalo Alonso](./assets/foto-gonzalo.jpg) <br> Carhuancote Dominguez, Gonzalo Alonso | Ingeniería de Software <br>Universidad Peruana de Ciencias Aplicadas | Estudiante de Ingeniería de Software con experiencia práctica en desarrollo backend y lógica de negocio. Posee dominio técnico en lenguajes como C++, Java, TypeScript y Python, aportando al diseño de arquitectura de software, implementación de servicios RESTful y configuración de entornos. |
| ![Adriana Maria](./assets/foto-adriana.jpg) <br> Diestra Zambrano, Adriana Maria | Ingeniería de Software <br>Universidad Peruana de Ciencias Aplicadas | Descripcion |
| ![Antonio Rodrigo](./assets/foto-rodrigo.png) <br> Duran Diaz, Antonio Rodrigo | Ingeniería de Software <br>Universidad Peruana de Ciencias Aplicadas | Soy estudiante de la carrera de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas. En este proyecto espero seguir mejorando mis habilidades y conocimientos, además de lograr un buen desempeño en el trabajo grupal |
| ![Marco Antonio](./assets/foto-marco.jpg) <br> Nakasone Gomes, Marco Antonio | Ingeniería de Software <br>Universidad Peruana de Ciencias Aplicadas | Descripcion |
| ![Carlos Joel](./assets/foto-carlos.jpg) <br> Shimabukuro Uku, Carlos Joel | Ingeniería de Software <br>Universidad Peruana de Ciencias Aplicadas | Descripcion |
| ![Joan Fernando](./assets/foto-joan.jpg) <br> Teves Samaniego, Joan Fernando | Ingeniería de Software <br>Universidad Peruana de Ciencias Aplicadas | Descripcion |

## 1.2. Solution Profile

Nuestra solución se denomina Cold2Hot, un sistema inteligente para cajas de delivery diseñado para proteger la calidad termica y la seguridad de los pedidos en trayecto.

### 1.2.1 Antecedentes y problemática

### Antecedentes
<div style="text-align: justify">

A esta situación se suma el riesgo de manipulación de los alimentos durante el trayecto. La falta de mecanismos de seguridad automatizados y de controles de acceso en los contenedores de reparto impide que los negocios o los clientes finales tengan la certeza de que el pedido no ha sido abierto sin autorización. La carencia de telemetría, evidencias fotográficas al momento de la entrega y sistemas de monitoreo en tiempo real crea un vacío de información operativo, donde el estado de la entrega es una incógnita hasta que llega a la puerta del cliente. Frente a esto, surge la necesidad de implementar soluciones de Internet de las Cosas (IoT) que permitan automatizar el control térmico y la seguridad, integrando sensores, actuadores y códigos de acceso conectados a plataformas digitales para asegurar una cadena de custodia transparente.

</div>

### Problemática

<div align="justify">
Para entender la necesidad del proyecto, se aplicó la técnica de las 5W's + 2H's:

### 5W's
### What (¿Cuál es el problema?):
La pérdida intempestiva de la temperatura ideal (caliente o fría) de los alimentos durante la ruta de reparto, sumada al riesgo de aperturas no autorizadas del contenedor, la falta de controles de acceso físico y la ausencia de un sistema de monitoreo y evidencia en tiempo real que garantice la cadena de custodia.

### When (¿Cuándo ocurre el problema?):
Durante el trayecto de envío urbano, especialmente en desplazamientos que superan los 15 minutos, en horas de alto tráfico o bajo condiciones climáticas adversas que aceleran la transferencia térmica.

### Where (¿Dónde ocurre el problema?):
En el espacio de transporte urbano (usualmente motocicletas o bicicletas) durante el tránsito desde el punto de despacho del restaurante hasta el domicilio del consumidor final.

### Who (¿A quién o quiénes afecta el problema?):
- A los administradores de operaciones de delivery, quienes asumen las pérdidas por reembolsos y el impacto negativo en la reputación de la marca al no contar con pruebas irrefutables de la entrega.

- A los repartidores, que se exponen a penalizaciones operativas o conflictos con los clientes debido a factores logísticos que escapan de su control.

- Al consumidor final, quien recibe un producto con calidad mermada o riesgos de salubridad.

### Why (¿Por qué sucede el problema?):
Porque el sector logístico tradicional de alimentos emplea mochilas y cajas pasivas que carecen de sistemas de regulación térmica activa, sensores de seguridad y conectividad. No existe un ecosistema tecnológico integrado que gestione permisos de apertura, alerte sobre desviaciones térmicas o manipulaciones, y registre el momento exacto de entrega con evidencias.

### 2H's
### How (¿Cómo aparece el problema?):
El problema se manifiesta a través de la disipación natural del calor o frío en contenedores sin aislamiento inteligente, a través de cierres mecánicos simples (como cremalleras o velcros) que pueden ser abiertos por cualquier persona en la ruta, y por la ausencia de registros de auditoría y fotografías al concretar la entrega.Inclusive las medidas de seguridad de los restaurantes al tratar de evitar aperturas no autorizadas usando cierres o etiquetas adhesivas se ven comprometidas porque estas pueden ser replicadas o rotas.

### How Much (¿Cuánto afecta el problema?):
Los reclamos por entregas frías o paquetes vulnerados representan una de las principales causas de pérdida de ventas recurrentes y clientes fidelizados para los restaurantes, impactando directamente en su rentabilidad mensual y generando altos costos operativos por la reposición y reembolso de pedidos dañados.

</div>

### 1.2.2 Lean UX Process.

#### 1.2.2.1. Lean UX Problem Statements.

<div style="text-align: justify">

Nuestro producto, Cold2Hot, abordará esta brecha mediante la implementación de una caja inteligente de delivery equipada con un microcontrolador ESP32 NodeMCU. Este sistema se integrará con un sensor de temperatura DS18B20, un actuador de ventilación, y un sistema de seguridad de dos niveles procesado mediante la lectura conjunta de un sensor magnético Reed Switch y un sensor infrarrojo TCRT5000. Los datos emitidos se sincronizarán con un panel de administración para empresas y una aplicación móvil para repartidores, habilitando la gestión de perfiles térmicos, bloqueos por código, y reportes de auditoría en tiempo real. Nuestro enfoque inicial será cadenas de restaurantes de tamaño pequeño y mediano, así como repartidores independientes en zonas urbanas.

Sabremos que hemos tenido éxito cuando observemos una reducción del 35% en quejas de clientes por alimentos en estado térmico deficiente, alcancemos una tasa del 90% de entregas sin alertas críticas de manipulación y logremos un aumento de al menos el 20% en la retención de clientes para los establecimientos afiliados mediante el uso de reportes de evidencia.

</div>

#### 1.2.2.2. Lean UX Assumptions.

**Business Assumptions:**

1. Creemos que los restaurantes están dispuestos a invertir en la adopción de cajas inteligentes IoT si el costo unitario de hardware se mantiene accesible y justifica el retorno de inversión.

2. Creemos que la oferta de una plataforma SaaS de monitoreo centralizado permitirá la monetización a través de suscripciones mensuales viables para los restaurantes o plataformas de delivery que quieran invertir y equipar a sus motorizados.

3. Creemos que la validación de entregas mediante códigos y fotografías reducirá drásticamente las devoluciones fraudulentas por parte de malos clientes.

4. Captaremos clientes mediante alianzas, referidos y estrategias digitales.

**User Assumptions:**
1. Creemos que los administradores de restaurantes necesitan un panel web centralizado para supervisar el despacho, configurar el tipo de temperatura de cada envío, y auditar los tiempos exactos de apertura de las cajas.

2. Creemos que los repartidores requieren una aplicación que los asista proactivamente, exigiéndoles mantener la conectividad (Bluetooth) y guiándolos en el proceso de entrega mediante códigos de apertura y toma de evidencias.

3. Creemos que los repartidores necesitan un sistema que diferencie entre un descuido (caja mal cerrada pero con el pedido dentro) y una manipulación real, emitiendo notificaciones proporcionales a la gravedad del evento.

**Business Outcome Assumptions:**
- Lograremos una reducción del 35% en reclamos y devoluciones por alimentos entregados fuera del rango térmico óptimo.
- Alcanzaremos un 90% de entregas monitoreadas sin incidencias de aperturas no autorizadas.
- Reduciremos en un 70% las disputas logísticas entre restaurantes, clientes y repartidores al contar con un historial auditable de tiempos de apertura y evidencias fotográficas.

**User Outcome Assumptions:**
- Los administradores de restaurante obtendrán visibilidad total, capacidad de definir perfiles térmicos antes del despacho, y evidencia digital irrefutable sobre el estado físico de los pedidos entregados.

- Los repartidores minimizarán penalizaciones injustas trabajando con mayor seguridad, recibiendo avisos preventivos para corregir cierres accidentales y demostrando la correcta entrega de los paquetes.

- Los clientes finales disfrutarán de una experiencia superior, recibiendo alimentos en temperatura ideal y con higiene garantizada.

**Features:**
- Regulador térmico automatizado operado por un ESP32 y un sensor DS18B20 cuya configuración modo frío o caliente es asignada remotamente desde el panel de la empresa al iniciar el despacho.

- Sistema de seguridad de dos niveles que cruza datos del sensor magnético y el infrarrojo para diferenciar entre aperturas accidentales con el paquete dentro emitiendo un aviso preventivo y extracciones reales del pedido emitiendo una alerta crítica.

- Sistema de control de acceso físico que mantiene el contenedor bloqueado hasta que el repartidor digite en su aplicación el código único de entrega generado por el restaurante.

- Aplicación móvil para repartidores que incluye recordatorio inicial de conexión Bluetooth, lectura de métricas de temperatura, recepción de alertas, y un flujo de cierre de entrega con captura de fotografía como evidencia.

- Panel de administración web/móvil para la empresa que permite generar códigos de acceso, configurar la temperatura, y visualizar reportes en tiempo real, tiempos exactos de apertura, estado de permanencia ocupado/desocupado, métricas térmicas y registro fotográfico.


#### 1.2.2.3. Lean UX Hypothesis Statements.

Para la elaboración de los Hypothesis Statements, se empleó la plantilla recomendada Lean UX:
We believe that [business outcome] will be achieved if [user] attains [benefit] with [feature].

#### Hipótesis 1
**Creemos que** la reducción del 35% en reclamos por alimentos en mal estado térmico **se logrará si** los administradores de restaurantes **obtienen** la capacidad de adaptar el entorno de la caja a cada pedido **con** una funcionalidad de configuración térmica remota (frío/caliente) integrada al ESP32 y al sensor DS18B20.

#### Hipótesis 2
**Creemos que** la reducción de fricción operativa y estrés en la conducción **se logrará si** los repartidores **obtienen** notificaciones precisas que eviten falsas alarmas **con** un sistema de seguridad de dos niveles que distingue entre una caja mal cerrada y una extracción real del pedido.

#### Hipótesis 3
**Creemos que** la erradicación de aperturas no autorizadas en ruta **se logrará si** los restaurantes y clientes **obtienen** garantía de inviolabilidad **con** un sistema de control de acceso físico que requiere la digitación de un código único para abrir el contenedor.

#### Hipótesis 4
**Creemos que** la disminución de penalizaciones injustas hacia los conductores **se logrará si** los repartidores **obtienen** una herramienta para registrar su desempeño **con** entregas seguras y confiables.

#### Hipótesis 5
**Creemos que** la reducción del 70% en disputas logísticas por reembolsos **se logrará si** los administradores de restaurantes **obtienen** visibilidad gerencial y auditoría total **con** un panel de administración que consolida reportes en tiempo real de temperatura, tiempos exactos de apertura, estado de ocupación del paquete y registro fotográfico.

#### 1.2.2.4. Lean UX Canvas

| Business Problem | Solutions | Business Outcomes |
|---|---|---|
| Los restaurantes sufren pérdidas económicas y de reputación por entregas frías, vulneradas o reportadas falsamente como no recibidas. Existe una nula visibilidad del estado de la caja de transporte, falta de controles de acceso en ruta y carencia de evidencias al momento de la entrega, lo que impide garantizar la calidad del servicio logístico. | Implementación de una caja de delivery inteligente (ESP32) con regulación térmica configurable, seguridad de dos niveles, control de apertura por código, y aplicaciones web/móviles para reportes en tiempo real, alertas preventivas y captura fotográfica de entrega | - Disminución del 35% en reclamos por temperatura inadecuada.<br>- Reducción del 90% en incidencias de manipulación.<br>- Mejora en la rentabilidad y fidelización del cliente. |

| Users and Customer | | User Outcomes & Benefits |
|---|---|---|
| Administradores de restaurantes: Requieren asegurar la cadena de custodia, controlar la temperatura remotamente y tener evidencia digital auditable.<br>Repartidores: Necesitan herramientas que avisen si la caja quedó mal cerrada sin emitir falsas alarmas, y poder demostrar que entregaron el pedido correctamente.<br>Consumidores: Buscan garantías de higiene y temperatura ideal. | | - Los restaurantes logran trazabilidad total del despacho en tiempo real, con marcas de tiempo precisas de apertura y fotos de entrega.<br>- Los repartidores reciben avisos preventivos para corregir descuidos, cuentan con recordatorios de conectividad y evitan sanciones mediante la evidencia fotográfica.<br>- Los consumidores disfrutan de alimentos protegidos. |

| Hypotheses | What is the most important thing we need to learn first? | What is the least amount of work we need to do to learn the next most important thing? |
|---|---|---|
| Creemos que dotar a los contenedores de telemetría activa, bloqueos por código, seguridad de dos niveles y un panel web de auditoría fotográfica reducirá las devoluciones un 35% y evitará manipulaciones en un 90%, blindando operativamente al restaurante y al repartidor. | Necesitamos validar si la interacción entre la generación del código en el restaurante y la digitación en la aplicación del repartidor para abrir la caja ocurre sin latencias que retrasen el proceso de entrega. | Desarrollar un flujo de interfaz y un prototipo físico del mecanismo de bloqueo, ejecutando pruebas de usabilidad cronometradas con repartidores ficticios ingresando códigos de apertura y tomando fotografías. |

## 1.3. Segmentos objetivo.

El modelo de negocio de Cold2Hot impacta en el ecosistema logístico urbano de última milla, dividiendo su enfoque en dos segmentos principales de usuarios directos:

### Segmento 1: Administradores de operaciones de delivery  
- **Descripcion:** Encargados de la operación y gerencia de establecimientos con alto volumen de despachos. Supervisan el proceso a través de un panel de administración web o móvil para asignar perfiles térmicos (frío/caliente), verificar el estado de la caja (abierta/cerrada), y visualizar los reportes en tiempo real. 
- **Sexo:** Masculino y femenino.
- **Edades:** Adultos jóvenes (25-40 años) y adultos de mediana edad (41-55 años).
- **Nivel socioeconómico**: Sectores B y A (media-alta y alta).
- **Necesidades**: Reducir drásticamente la tasa de pedidos reembolsados por quejas de calidad o reportes falsos de no entrega. Requieren un registro inmutable y auditable (incluyendo métricas, tiempos exactos de apertura y evidencias fotográficas) para deslindar responsabilidades frente a los servicios de entrega de terceros y proteger el prestigio de la marca.

### Segmento 2: Operadores de entrega
- **Descripcion:** Conductores de motocicletas o bicicletas, ya sean independientes (asociados a aplicativos) o en planilla fija del restaurante. Interactúan con la caja inteligente mediante una aplicación móvil que les exige mantener conectividad Bluetooth, les permite ingresar códigos de apertura y registrar fotografías del pedido entregado.
- **Sexo:** Masculino y femenino.
- **Edades:** Jóvenes y adultos (18-45 años).
- **Nivel socioeconómico**: Sectores C y D.
- **Necesidades**: Evitar mermas en sus ingresos provocadas por penalizaciones injustas. Buscan soluciones tecnológicas que les avisen de forma inteligente si olvidaron cerrar la caja y que les permitan resguardar su trabajo mediante pruebas irrefutables de entrega exitosa.

<div style="page-break-after: always;"></div>

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
