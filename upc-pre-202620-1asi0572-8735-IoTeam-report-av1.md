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
| ![Juan Carlos](./assets/foto-juan.jpeg) <br> Alvarado De La Cruz, Juan Carlos | Ingeniería de Software <br>Universidad Peruana de Ciencias Aplicadas | Estudiante de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas. Cuento con conocimientos en desarrollo de aplicaciones y bases de datos, y me interesa el trabajo con dispositivos IoT. En este proyecto busco aportar al desarrollo de la solución y fortalecer mis habilidades de trabajo en equipo, cumpliendo con los plazos establecidos. |
| ![Gonzalo Alonso](./assets/foto-gonzalo.jpg) <br> Carhuancote Dominguez, Gonzalo Alonso | Ingeniería de Software <br>Universidad Peruana de Ciencias Aplicadas | Estudiante de Ingeniería de Software con experiencia práctica en desarrollo backend y lógica de negocio. Posee dominio técnico en lenguajes como C++, Java, TypeScript y Python, aportando al diseño de arquitectura de software, implementación de servicios RESTful y configuración de entornos. |
| ![Adriana Maria](./assets/foto-adriana.jpg) <br> Diestra Zambrano, Adriana Maria | Ingeniería de Software <br>Universidad Peruana de Ciencias Aplicadas | Estudiante de Ingeniería de Software con un enfoque práctico en el desarrollo frontend y backend. Cuento con conocimientos en Vue 3, Node.js, Kotlin y Docker, orientados a la creación de interfaces, la estructuración de servicios y la gestión de entornos de desarrollo. Me motiva colaborar de forma activa en equipos dinámicos, aportando soluciones creativas y asegurando que cada proyecto alcance sus objetivos a tiempo. |
| ![Antonio Rodrigo](./assets/foto-rodrigo.png) <br> Duran Diaz, Antonio Rodrigo | Ingeniería de Software <br>Universidad Peruana de Ciencias Aplicadas | Soy estudiante de la carrera de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas. En este proyecto espero seguir mejorando mis habilidades y conocimientos, además de lograr un buen desempeño en el trabajo grupal |
| ![Marco Antonio](./assets/foto-marco.png) <br> Nakasone Gomes, Marco Antonio | Ingeniería de Software <br>Universidad Peruana de Ciencias Aplicadas | Tengo 22 años y estoy cursando el 9vo ciclo de la carrera de Ingeniería de Software. Considero que soy bueno trabajando de manera grupal y cumplo con todas las tareas a tiempo. Me gusta aportar con ideas buenas y óptimas para poder mejorar el trabajo. |
| ![Carlos Joel](./assets/foto-carlos.jpg) <br> Shimabukuro Uku, Carlos Joel | Ingeniería de Software <br>Universidad Peruana de Ciencias Aplicadas | Estudiante de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas. Con experiencia en C++, además de tener conocimientos en HTML, CSS y JavaScript. En este proyecto, mi objetivo es aplicar los conocimientos adquiridos hasta ahora y obtener una comprensión más profunda sobre mi futuro rol como profesional en esta área. |
| ![Joan Fernando](./assets/foto-joan.jpeg) <br> Teves Samaniego, Joan Fernando | Ingeniería de Software <br>Universidad Peruana de Ciencias Aplicadas | Estudiante de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas. Cuento con conocimientos en programación y en el manejo de herramientas de desarrollo, con interés en la integración de hardware y software. En este proyecto espero contribuir en la implementación de la solución y seguir desarrollando mis habilidades técnicas y de colaboración en equipo. |

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
En el mercado actual de logística urbana y reparto de última milla, la entrega de alimentos y productos sensibles a la temperatura enfrenta constantes desafíos vinculados con la pérdida de calidad térmica y la vulnerabilidad física de los paquetes en ruta. Para comprender a cabalidad el entorno competitivo de **Cold2Hot** (desarrollado por la startup **IoTeam**), se identificaron tres competidores clave con ofertas directas e indirectas en el rubro de logística y transporte de temperatura controlada:

1. **Thermotecnica (Mochilas y Cajas Térmicas Pasivas):** Principal referente en la provisión de mochilas térmicas tradicionales para repartidores independientes y operadores de última milla (Rappi, PedidosYa). Su enfoque es enteramente analógico y pasivo, recurriendo a aislamiento con poliestireno expandido o mantas térmicas convencionales.
2. **Controlant:** Empresa global especializada en soluciones de cadena de frío y trazabilidad en tiempo real basadas en IoT. Aunque su público objetivo primario es el sector farmacéutico y la macro-logística de distribución médica o perecibles a gran escala, representa el estándar de monitoreo telemático y telemetría de temperatura en la nube.
3. **Peli BioThermal (Smart Packaging & Credo ProEnvision):** Líder en soluciones térmicas avanzadas y embalajes reutilizables para el transporte especializado de productos de alto valor con control de temperatura, combinando materiales de cambio de fase (PCM) e indicadores de seguridad, enfocado en logística corporativa y distribución B2B.

---

### 2.1.1. Análisis competitivo.

A continuación, se desarrolla el **Competitive Analysis Landscape** para contrastar la propuesta de valor integral de **Cold2Hot** frente a las alternativas del mercado:

### Competitive Analysis Landscape

| ¿Por qué llevar a cabo este análisis? | El objetivo de este análisis competitivo es identificar las brechas existentes en el mercado de entrega urbana de última milla de alimentos, evaluando las carencias telemáticas y de seguridad física en las soluciones convencionales frente a las herramientas corporativas de cadena de frío, con el fin de consolidar la diferenciación y viabilidad operativa de **Cold2Hot**. |
| :--- | :--- |

| Dimensiones | Nuestra Startup: **Cold2Hot (IoTeam)** | Competidor 1: **Thermotecnica** | Competidor 2: **Controlant** | Competidor 3: **Peli BioThermal** |
| :--- | :--- | :--- | :--- | :--- |
| **Logotipo / Identidad** | | <div align="center"><img src="assets/thermotecnica-logo.png" alt="Thermotecnica" width="90"></div> | <div align="center"><img src="assets/controlant-logo.png" alt="Controlant" width="90"></div> | <div align="center"><img src="assets/peli-biothermal-logo.jpg" alt="Peli BioThermal" width="90"></div> |
| **Perfil (Overview)** | Solución integral IoT para delivery urbano que combina una caja inteligente con regulación térmica activa (ESP32, DS18B20), seguridad física con desbloqueo por código OTP (Reed Switch + TCRT5000), telemetría continua y captura de evidencias fotográficas. | Fabricante y comercializador de mochilas, bolsas y cajas térmicas pasivas con aislamiento estándar, diseñadas para mensajería y entrega tradicional de comida rápida en bicicletas y motocicletas. | Empresa de monitoreo digital de cadena de frío que ofrece registradores de datos IoT celulares/cloud en tiempo real y software de análisis de visibilidad logística a gran escala. | Fabricante de soluciones avanzadas de embalaje pasivo y semi-activo con aislamiento de alta densidad y monitoreo de temperatura para transporte de insumos biológicos y perecibles de alta exigencia. |
| **Ventaja competitiva** | Trazabilidad integral en última milla: regulación térmica activa, bloqueo físico desarmable únicamente mediante OTP en destino, prevención de manipulaciones mediante seguridad de dos niveles y generación automática de reportes de auditoría con evidencia fotográfica. | Muy bajo costo de adquisición inicial, ligereza de transporte, amplia disponibilidad comercial y nulo requerimiento de mantenimiento tecnológico o energético. | Plataforma en la nube de alta confiabilidad con cobertura telemática global continua (redes celulares IoT/GPS) y cumplimiento de estándares internacionales de auditoría (FDA, GMP). | Embalajes térmicos reutilizables con materiales de cambio de fase (PCM) de altísima eficiencia pasiva (hasta 120 horas de estabilidad térmica) sin consumo de batería. |
| **Perfil de Marketing: Mercado objetivo** | Restaurantes medianos y pequeños, cadenas de comida rápida con flota propia o tercerizada, y repartidores urbanos que requieren certificar la entrega higiénica y la temperatura del alimento. | Repartidores independientes de aplicaciones móviles de delivery (Rappi, PedidosYa, Uber Eats) y pequeños negocios gastronómicos locales. | Corporaciones farmacéuticas multinacionales, distribuidores de vacunas y grandes empresas de logística de perecibles a gran escala (B2B industrial). | Laboratorios clínicos, sector biotecnológico, farmacias hospitalarias y servicios de catering gourmet/médico corporativo de alto presupuesto. |
| **Perfil de Marketing: Estrategias de marketing** | Venta directa B2B a cadenas de restaurantes, planes de suscripción SaaS mensual para el uso del software de gestión y auditoría, alianzas con asociaciones gastronómicas locales y demos funcionales. | Venta por catálogo físico, presencia en distribuidores de accesorios para motos/bicicletas, marketplaces de comercio electrónico y compras corporativas directas por volumen. | Venta consultiva corporativa B2B de ciclo largo, presencia en ferias internacionales de supply chain/farma, marketing de contenidos sobre regulaciones y modelos PaaS (Product as a Service). | Venta técnica B2B mediante representantes comerciales autorizados, certificaciones internacionales de calidad y contratos corporativos de leasing/retorno de contenedores. |
| **Perfil de Producto: Productos & Servicios** | - Caja inteligente *SmartBox* con microcontrolador ESP32.<br>- Panel web centralizado de despacho y auditoría para restaurantes.<br>- Aplicación móvil para repartidores (control BLE, desbloqueo OTP, captura de fotos).<br>- Reportes inmutables de cadena de custodia térmica. | - Mochilas térmicas de lona oxford con aislante de espuma.<br>- Bolsas de mano térmicas.<br>- Cajas rígidas de fibra de vidrio sin componentes electrónicos ni sensores. | - Dispositivos registradores IoT (Saga Card / Pods) con conectividad celular/IoT.<br>- Plataforma en la nube *Controlant Cloud* para trazabilidad en tiempo real.<br>- Servicios de alertas automáticas 24/7 y analítica de datos. | - Cajas y contenedores rígidos con tecnología de cambio de fase (Credo Cube).<br>- Sensores pasivos/registradores de temperatura USB/RF.<br>- Software de seguimiento de inventario térmico y calibración. |
| **Precios & Costos** | Hardware accesible de costo moderado (orientado a ensamble ágil y componentes estandarizados) complementado con una suscripción de software SaaS mensual accesible para pymes gastronómicas. | Costo único muy bajo por mochila/caja (aprox. $25 - $60 USD), sin costos recurrentes ni tarifas de software. | Alto costo operativo; modelo de suscripción por viaje o por dispositivo anual de alto valor (centenas o miles de dólares por contrato corporativo). | Costo unitario elevado por contenedor térmico ($150 - $500+ USD) sumado a costos de recertificación y reposición de geles/placas PCM. |
| **Canales de distribución** | Plataforma Web oficial (Landing Page institucional), venta corporativa directa y distribución de aplicaciones móviles vía Google Play Store y Apple App Store. | Puntos de venta retail especializados, tiendas de motociclismo, plataformas de e-commerce (MercadoLibre, Amazon) y convenios directos con apps de delivery. | Canal corporativo directo B2B a través de oficinas regionales y red global de socios tecnológicos y logísticos. | Red de distribuidores técnicos certificados, representantes comerciales B2B y despacho logístico programado. |
| **Análisis SWOT: Fortalezas** | - Solución diseñada a la medida del dolor de la última milla gastronómica.<br>- Seguridad física inviolable por OTP que erradica la apertura no autorizada.<br>- Seguridad de dos niveles (Reed Switch + TCRT5000) para descartar falsas alarmas.<br>- Plataforma de software integral (Web + Móvil + Edge IoT). | - Marca reconocida y posicionada en el sector de repartidores independientes.<br>- Precios altamente competitivos y sin barreras tecnológicas de entrada.<br>- Alta durabilidad mecánica y facilidad de reemplazo inmediato. | - Plataforma de software madura, escalable y con alta reputación internacional.<br>- Conectividad global y acuerdos con operadores de telecomunicaciones.<br>- Infraestructura en la nube con soporte 24/7 y analítica predictiva. | - Aislamiento térmico pasivo de ingeniería avanzada y de larga duración.<br>- Estructuras sólidas y de máxima durabilidad reutilizable.<br>- Amplio cumplimiento normativo para transporte sensible. |
| **Análisis SWOT: Debilidades** | - Startup en etapa de introducción y validación inicial.<br>- Dependencia de la recarga de batería del dispositivo IoT en la jornada diaria.<br>- Necesidad de capacitar al repartidor en el uso de la aplicación móvil y el flujo de entrega. | - Nula tecnología: carece de telemetría, sensores, alertas y controles de acceso.<br>- Imposibilidad de acreditar la cadena de custodia o demostrar adulteraciones.<br>- La temperatura decae progresivamente sin aviso ni control activo. | - Modelo de precios inviable para el sector de restaurantes y entrega de comida rápida.<br>- Dispositivos no integrados a mecanismos físicos de apertura o cerradura de cajas.<br>- No contempla la captura de evidencias fotográficas de entrega ni apps operativas para couriers de comida. | - No cuenta con conectividad nativa en tiempo real para última milla urbana.<br>- Operación pesada que requiere acondicionamiento previo de placas PCM.<br>- Costo unitario prohibitivo para la gran mayoría de restaurantes y repartidores independientes. |
| **Análisis SWOT: Oportunidades** | - Crecimiento sostenido del delivery de comida gourmet y productos frescos que exigen control térmico.<br>- Alta tasa de reclamos por comida fría o paquetes vulnerados en plataformas de delivery.<br>- Demanda de soluciones que reduzcan las pérdidas por devoluciones injustas en restaurantes. | - Posibilidad de añadir cierres de combinación mecánicos económicos.<br>- Creciente número de trabajadores de delivery en las principales ciudades de la región. | - Expansión de sus servicios hacia la logística urbana de última milla para farmacias o alimentos ultra frescos.<br>- Alianzas con flotas de transporte terrestre. | - Adaptación de modelos más compactos y económicos orientados a catering corporativo o delivery prémium. |
| **Análisis SWOT: Amenazas** | - Resistencia de algunos repartidores a adoptar controles más estrictos de apertura y fotografía.<br>- Competidores tradicionales que incorporen precintos de seguridad mecánicos económicos.<br>- Subida en los costos de adquisición de microcontroladores y sensores electrónicos. | - Penetración de cajas inteligentes que vuelvan obsoletas las mochilas térmicas convencionales.<br>- Mayores regulaciones municipales y sanitarias sobre el transporte de alimentos preparados. | - Nuevos competidores de telemetría IoT low-cost que ingresen al mercado con tarifas agresivas. | - Entrada de fabricantes asiáticos que comercialicen contenedores con materiales aislantes avanzados a bajo costo. |

---

### 2.1.2. Estrategias y tácticas frente a competidores.

A partir del análisis del panorama competitivo y la matriz FODA, **IoTeam** define un conjunto de estrategias y tácticas comerciales, de producto y operativas para consolidar la entrada y el posicionamiento de **Cold2Hot**:

#### 1. Estrategia de Enfoque en el Nicho de Última Milla Gastronómica (Frente a Thermotecnica y competidores pasivos)
* **Objetivo:** Demostrar que el costo de una caja pasiva convencional es en realidad más alto a largo plazo debido a los reembolsos por comida fría y las disputas por manipulación del paquete.
* **Tácticas:**
  * **Cálculo de Retorno de Inversión (ROI):** Proveer a los administradores de restaurantes una calculadora de pérdidas operativas en el Landing Page de Cold2Hot, evidenciando cómo una reducción del 35% en reclamos amortiza rápidamente el costo de la tecnología.
  * **Diferenciación por Seguridad Activa:** Posicionar el mecanismo de bloqueo por código OTP como una garantía de higiene e inviolabilidad del pedido ante el comensal final, convirtiendo la caja en un argumento de marketing para el propio restaurante.
  * **Adopción Simple y Guiada:** Diseñar la aplicación móvil del repartidor con una curva de aprendizaje mínima (diseño UX intuitivo y compatible con Bluetooth de bajo consumo), facilitando que los repartidores la perciban como un escudo contra penalizaciones injustas y no como una carga de trabajo.

#### 2. Estrategia de Liderazgo en Costos Tecnológicos y Modelo SaaS Accesible (Frente a Controlant)
* **Objetivo:** Ofrecer las ventajas de la telemetría en tiempo real y la trazabilidad en la nube sin los precios corporativos prohibitivos del sector farmacéutico.
* **Tácticas:**
  * **Arquitectura IoT Eficiente:** Basar el hardware en componentes de código abierto y alta confiabilidad (microcontrolador ESP32 NodeMCU, sensor DS18B20, sensores TCRT5000 y Reed Switch), optimizando los costos de manufactura del prototipo.
  * **Esquema de Suscripción Modular (SaaS):** Estructurar planes mensuales adaptados al tamaño de la flota del restaurante (p. ej., cobro por caja activa monitoreada al mes), evitando pagos iniciales millonarios por licenciamiento.
  * **Integración de Flujos de Cierre de Entrega:** Incluir dentro de la misma solución el registro fotográfico obligatorio (Proof of Delivery), funcionalidad que los proveedores globales de trazabilidad industrial no ofrecen al estar desligados de la interacción directa con el consumidor final.

#### 3. Estrategia de Conectividad y Automatización Activa (Frente a Peli BioThermal)
* **Objetivo:** Superar la rigidez de los sistemas pasivos avanzados que requieren acondicionamientos químicos previos y carecen de comunicación telemática en ruta.
* **Tácticas:**
  * **Ajuste Dinámico de Perfiles Térmicos:** Permitir al administrador configurar perfiles de frío o calor desde el panel web de despacho en segundos, activando automáticamente la regulación del contenedor inteligente sin necesidad de cambiar placas físicas de enfriamiento.
  * **Seguridad de Dos Niveles contra Manipulaciones:** Implementar la lógica de discriminación entre una apertura accidental (alerta preventiva al operador para que ajuste la tapa) y una extracción real del paquete (alerta crítica inmediata al restaurante), protegiendo la carga en todo momento mediante telemetría continua.
  * **Generación Inmutable de Reportes de Auditoría:** Consolidar en un único reporte digital la gráfica térmica de todo el viaje, los tiempos exactos de desbloqueo y la fotografía tomada en destino, permitiendo deslindar responsabilidades de inmediato ante cualquier queja del cliente.

## 2.2. Entrevistas.

### 2.2.1. Diseño de entrevistas.

**Segmento 1: Administradores de operaciones de delivery**

1. ¿Cuál es tu rol y cuánto tiempo llevas gestionando las operaciones de delivery en este local?
2. ¿Cuáles son los principales problemas logísticos que enfrentan desde que el pedido sale de la cocina hasta que llega al cliente?
3. ¿Con qué frecuencia reciben reclamos por pedidos fríos, derramados o manipulados, y cómo impactan económicamente a fin de mes?
4. Ante el reporte de un paquete abierto, ¿cómo determinan actualmente si fue culpa del motorizado o si es un reclamo falso del cliente?
5. ¿Qué medidas de seguridad (cintas, sellos, etc.) utilizan actualmente en sus empaques y qué tan efectivas resultan en la ruta?
6. ¿Qué valor le aportaría a su gestión diaria poder monitorear la temperatura exacta de la caja de reparto en tiempo real?
7. ¿Qué opina de un sistema donde la caja de transporte se bloquee físicamente en el local y solo se abra con un PIN único en el destino?
8. ¿Qué tan útil le resultaría recibir un reporte automático con la foto de entrega y la hora exacta de apertura para resolver disputas con las apps de delivery?

**Segmento 2: Operadores de entrega (repartidores)**

1. ¿Cuánto tiempo llevas trabajando como repartidor y con qué aplicaciones trabajas con mayor frecuencia?
2. ¿Qué problemas de temperatura, cierres o seguridad presentan las mochilas que usas actualmente para transportar los alimentos?
3. ¿Alguna vez te han penalizado o descontado dinero injustamente por un pedido que llegó frío o maltratado por el tráfico?
4. ¿Has tenido experiencias con clientes que reportan falsamente entregas incompletas? ¿Cómo te defiendes ante la aplicación?
5. ¿Cómo te ayudaría en tu trabajo si tu caja regulara la temperatura (frío/calor) automáticamente durante el trayecto sin que te preocupes?
6. ¿Qué te parece la idea de recibir una alerta preventiva en tu celular si olvidas asegurar bien la tapa antes de arrancar la moto?
7. Si la caja se mantiene bloqueada hasta que ingresas un PIN en el destino, ¿crees que te ayudaría a demostrar que no manipulaste el paquete?
8. ¿Estarías dispuesto a tomar una foto obligatoria del paquete entregado usando nuestra app si eso te garantiza que no te pondrán multas injustas?

### 2.2.2. Registro de entrevistas.

A continuación, se presenta el registro de las entrevistas realizadas a los representantes de nuestros dos segmentos objetivo. Estas sesiones se llevaron a cabo de forma virtual/presencial con el fin de validar nuestras hipótesis de negocio y entender a profundidad sus necesidades.

**Entrevista 1**
* **Nombres y Apellidos:** Roberto Fernández
* **Segmento Objetivo:** Segmento 1 - Administrador de operaciones de delivery
* **Edad:** 35 años
* **Fecha de Entrevista:** 15/09/2026
* **Duración:** 18 minutos

**Entrevista 2**
* **Nombres y Apellidos:** Katia Torres
* **Segmento Objetivo:** Segmento 2 - Operador de entrega (Repartidor)
* **Edad:** 26 años
* **Fecha de Entrevista:** 16/09/2026
* **Duración:** 15 minutos
<img src="./assets/Entrevista1.png">

https://upcedupe-my.sharepoint.com/:v:/g/personal/u202117303_upc_edu_pe/IQCw2iS8WZqYSpyTqV73I-zyAV2gmtetVbyAsgyOkBEmwIM
---

### 2.2.3. Análisis de entrevistas.

Tras procesar las respuestas obtenidas en las entrevistas, se identificaron patrones de comportamiento, dolores recurrentes (pains) y expectativas (gains) que validan directamente la necesidad de la solución **Cold2Hot**. A continuación, se detallan los hallazgos principales por segmento:

**Hallazgos del Segmento 1 (Administradores de operaciones de delivery):**
1. **La ceguera operativa es el mayor dolor financiero:** Los administradores confirmaron que, una vez que el pedido sale del local, pierden el control total sobre la cadena de frío y la manipulación. Esto se traduce en pérdidas económicas constantes debido a que las plataformas de delivery suelen priorizar el reclamo del cliente y aplicar reembolsos automáticos descontados al restaurante.
2. **Las medidas de seguridad actuales son insuficientes:** El uso de cintas adhesivas o grapas en las bolsas es visto como una medida paliativa que no evita aperturas no autorizadas y no ofrece ninguna prueba técnica en caso de disputas.
3. **Alta disposición a la adopción tecnológica:** La funcionalidad de un registro de auditoría (timestamp de apertura por PIN + evidencia fotográfica) fue identificada como la característica de mayor valor. Los administradores ven este panel no solo como una herramienta de calidad, sino como un mecanismo de defensa contra el fraude de clientes malintencionados.

**Hallazgos del Segmento 2 (Operadores de entrega / Repartidores):**
1. **Fricción física y deterioro de herramientas:** Las mochilas térmicas tradicionales se desgastan rápidamente (velcros y cierres), lo que propicia aperturas accidentales por el viento, baches o la prisa, derivando en pedidos fríos.
2. **Vulnerabilidad ante penalizaciones injustas:** Los repartidores (como Katia) sienten una profunda frustración al recibir descuentos económicos y bajas calificaciones por factores que escapan de su control (mal empaque desde el restaurante, tráfico, clima o clientes que reportan entregas incompletas falsamente). 
3. **Recepción positiva de la automatización:** La idea de una caja inteligente que regule la temperatura de manera autónoma fue percibida como un gran alivio que reduce el estrés al conducir.
4. **La seguridad como "seguro laboral":** Contrario a lo que se podría asumir (que un PIN o tomar una foto genera pérdida de tiempo), los motorizados ven el mecanismo de bloqueo y la captura fotográfica obligatoria como un beneficio. Lo consideran una herramienta que los deslinda de responsabilidad y los protege frente al soporte técnico de las aplicaciones.

**Conclusión General y Validación de Hipótesis:**
Las entrevistas validan rotundamente las hipótesis planteadas en nuestro *Lean UX Canvas*. Ambos segmentos sufren las consecuencias de la falta de trazabilidad y seguridad en la última milla, pero desde perspectivas distintas (el administrador pierde dinero por mermas; el repartidor pierde dinero por penalizaciones). La implementación de la caja inteligente **Cold2Hot** con bi-direccionalidad de datos (PIN de apertura y registro fotográfico) resuelve el dolor principal de ambos actores: **elimina las disputas logísticas al proveer una fuente de verdad única, automatizada e inmutable.**
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
