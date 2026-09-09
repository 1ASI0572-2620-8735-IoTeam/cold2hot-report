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

IoTeam es una startup tecnológica dedicada al desarrollo de soluciones basadas en Internet de las Cosas orientadas a la logística urbana y a la preservación de la cadena de custodia en el delivery de alimentos.

* Misión: Garantizar la calidad, seguridad e integridad de los pedidos de comida durante su transporte mediante sistemas inteligentes de monitoreo ambiental y control térmico automatizado.
* Visión: Posicionarse como la startup referente en Latinoamérica en tecnología IoT aplicada a la logística de última milla para el sector gastronómico.
* Valores: Innovación constante, calidad de servicio, eficiencia energética, seguridad operacional y compromiso con la satisfacción del cliente final.

### 1.1.2. Perfiles de integrantes del equipo

El equipo de IoTeam está conformado por 7 estudiantes de la carrera de Ingeniería de Software de la Universidad Peruana de Ciencias Aplicadas:

* Alvarado De La Cruz, Juan Carlos - U202216150
* Carhuancote Dominguez, Gonzalo Alonso - U202210720
* Diestra Zambrano, Adriana Maria - U202218110
* Duran Diaz, Antonio Rodrigo - U202215721
* Nakasone Gomes, Marco Antonio - U202210790
* Shimabukuro Uku, Carlos Joel - U201912407
* Teves Samaniego, Joan Fernando - U202117303

## 1.2. Solution Profile

El producto desarrollado es Cold2Hot, un sistema inteligente de monitoreo térmico y seguridad integral diseñado para cajas de delivery de alimentos.

### 1.2.1 Antecedentes y problemática

En la industria actual de delivery de alimentos, uno de los mayores desafíos logísticos es garantizar que los pedidos lleguen al consumidor en óptimas condiciones térmicas y de salubridad. Para un análisis detallado de la problemática se aplica la técnica 5W2H:

* Who: Empresas y restaurantes de delivery de comida preparada, repartidores de última milla y los consumidores finales que reciben alimentos en mal estado térmico o manipulados.
* What: Pérdida intempestiva de la temperatura ideal ya sea caliente y/o frío de los platillos en ruta, aperturas no autorizadas o mal cierre de la caja de transporte, y la falta de un sistema de monitoreo automatizado e higiénico.
* Where: Durante el transporte urbano en motocicleta o bicicleta desde la salida del restaurante hasta el punto de entrega al cliente final.
* When: Durante el trayecto de envío, especialmente en desplazamientos superiores a los 15 minutos o en condiciones climáticas adversas.
* Why: Las cajas de delivery convencionales son recipientes pasivos de aislamiento limitado, sin sensores de temperatura, sin actuadores de ventilación ni alertas de seguridad ante aperturas.
* How: Mediante un dispositivo embebido IoT impulsado por el microcontrolador ESP32, equipado con un sensor térmico de sonda metálica DS18B20, un sensor magnético Reed Switch, un infrarrojo TCRT5000, un actuador de ventilación vía Módulo Relé de 1 canal y un Buzzer activo, interconectados a aplicaciones web y móviles.
* How Much: Los reclamos por entregas frías o dañadas representan pérdidas de hasta el 15% en ventas recurrentes para los restaurantes. La solución IoT propone un costo de hardware altamente accesible por caja inteligente.

### 1.2.2 Lean UX Process.

#### 1.2.2.1. Lean UX Problem Statements.

En el contexto actual de la logística de reparto de comida, los principales afectados son los gerentes de restaurantes, los repartidores y los clientes finales. Estos grupos enfrentan problemas como la pérdida de temperatura de los alimentos, la apertura no autorizada de los contenedores y la falta de monitoreo de rutas en tiempo real. Las soluciones existentes no abordan la ausencia de un sistema automatizado de control térmico activo ni de telemetría de seguridad del contenedor en tiempo real integrada con plataformas móviles y web. Nuestro producto, Cold2Hot, cubrirá esta carencia combinando un dispositivo IoT embebido basado en ESP32 equipado con una sonda de temperatura DS18B20, un sensor magnético de puerta Reed Switch, un sensor infrarrojo TCRT5000, un actuador de ventilador mediante relé de un canal y un zumbador activo con aplicaciones de monitoreo web y móvil en tiempo real. Nos dirigiremos inicialmente a cadenas de restaurantes de pequeño y mediano tamaño y a repartidores independientes que operen en zonas urbanas. Consideraremos que hemos tenido éxito cuando observemos una reducción del 35 % en las quejas de los clientes por comida fría, una tasa de finalización de entregas del 90 % sin aperturas no autorizadas de los contenedores y un aumento de al menos el 20 % en la retención de clientes para los restaurantes participantes.

#### 1.2.2.2. Lean UX Assumptions.

1. Business Assumptions:
* Creemos que los restaurantes están dispuestos a adoptar cajas de delivery IoT si el costo del hardware se mantiene accesible por unidad.
* Creemos que ofrecer una plataforma de monitoreo en tiempo real permitirá cobrar una suscripción mensual accesible a los restaurantes por el servicio SaaS.
* Creemos que reducir las pérdidas por comida fría incrementará la lealtad y recompra de los usuarios finales.

2. Business Outcome Assumptions:
* Lograremos una reducción del 35% en reclamos por alimentos entregados a temperatura inadecuada.
* Lograremos que el 90% de los envíos monitoreados registren cero aperturas no autorizadas durante el trayecto.
* Reduciremos en un 50% las disputas de reembolso entre restaurantes y repartidores mediante registros térmicos auditables.

3. User Assumptions:
* Creemos que los administradores de restaurantes necesitan un panel web centralizado para supervisar múltiples despachos activos simultáneamente.
* Creemos que los repartidores necesitan un sistema completamente automatizado que regule la temperatura y emita alertas audibles sin requerir interacción manual mientras conducen.
* Creemos que los clientes finales desean recibir confirmación de que su pedido se mantuvo protegido en todo momento.

4. User Outcome and Benefit Assumptions:
* Los administradores de restaurante obtendrán tranquilidad y visibilidad total de la cadena de custodia de sus despachos.
* Los repartidores evitarán penalizaciones por comida entregada a destiempo o en mala temperatura.
* Los clientes finales disfrutarán de comida caliente, preservada y segura en su domicilio.

5. Feature Assumptions:
* Feature 1: Regulador térmico automatizado que activa el ventilador vía relé de 1 canal procesado por el ESP32 cuando el sensor DS18B20 detecta temperaturas fuera del umbral establecido.
* Feature 2: Sistema de seguridad para la tapa de la caja que acciona el Buzzer local y notifica a la app móvil del repartidor ante aperturas no autorizadas mediante el sensor Reed Switch.
* Feature 3: Detector de presencia física del paquete en el compartimento mediante el sensor infrarrojo TCRT5000 para iniciar y cerrar automáticamente el seguimiento del despacho en la aplicación web.

#### 1.2.2.3. Lean UX Hypothesis Statements.

Siguiendo la plantilla oficial de Lean UX, se definen las siguientes hipótesis:

* Declaración de Hipótesis 1: Creemos que lograremos una reducción del 35% en reclamos por comida fría si los administradores de restaurantes y repartidores obtienen regulación térmica automatizada y conservación óptima de la temperatura interna de la caja con el microcontrolador ESP32 integrado a la sonda de temperatura DS18B20 y el sistema de control de ventilador por relé de 1 canal.
* Declaración de Hipótesis 2: Creemos que lograremos una tasa del 90% de entregas completadas sin aperturas no autorizadas si los repartidores y supervisores del restaurante obtienen notificación inmediata local y móvil de aperturas inesperadas de la tapa de la caja con el sensor magnético Reed Switch junto al Buzzer activo y notificaciones push móviles.
* Declaración de Hipótesis 3: Creemos que lograremos una tasa de sesiones de monitoreo falsas menor al 5% si los despachadores del restaurante obtienen inicio y cierre automático de sesión sincronizado con la colocación del paquete con el sensor infrarrojo TCRT5000 integrado al panel web.

#### 1.2.2.4. Lean UX Canvas

| Business Problem | Solutions | Business Outcomes |
|---|---|---|
| Los restaurantes y empresas de delivery pierden clientes y dinero debido a entregas de comida que llegan frías, derramadas o manipuladas durante el trayecto, sin contar con herramientas para supervisar el estado de la caja de transporte en tiempo real. | Implementación de una caja inteligente de delivery impulsada por el microcontrolador ESP32, integrada con sensor térmico DS18B20 con sonda metálica, sensor magnético de puerta Reed Switch, sensor infrarrojo de presencia TCRT5000, sistema de ventilación impulsado por relé de 1 canal y alarma sonora con Buzzer activo, sincronizados en tiempo real con una aplicación móvil y una plataforma web. | - Reducción del 35% en reclamos por alimentos entregados a temperatura inadecuada.<br>- Reducción del 90% en incidencias de manipulación o aperturas no autorizadas de la caja.<br>- Incremento en la satisfacción y retención del cliente final. |

| Users and Customer | | User Outcomes & Benefits |
|---|---|---|
| Administradores de restaurantes: Necesitan garantizar la cadena de custodia de sus pedidos y reducir pérdidas por reembolsos.<br>Repartidores de delivery: Requieren alertas automáticas audibles y móviles que no interfieran con la conducción.<br>Consumidores finales: Exigen alimentos en temperatura óptima e higiene garantizada. | | - Los restaurantes obtienen visibilidad y control del estado de los despachos en tiempo real.<br>- Los repartidores reciben alertas instantáneas en su móvil y audibles ante variaciones térmicas o aperturas.<br>- Los clientes finales disfrutan de comida caliente, preservada y segura en su domicilio. |

| Hypotheses | What is the most important thing we need to learn first? | What is the least amount of work we need to do to learn the next most important thing? |
|---|---|---|
| Creemos que la regulación térmica automática con ESP32, sensor DS18B20 y relé con ventilador, junto al sistema de seguridad con Reed Switch y Buzzer activo, garantizará entregas seguras y a temperatura ideal, reduciendo reclamos por comida fría en un 35% y aperturas no autorizadas en un 90%. | Determinar si la combinación del microcontrolador ESP32 con el sensor DS18B20 y el relé de ventilación reacciona con suficiente velocidad para estabilizar la temperatura interna de la caja durante trayectos urbanos reales. | Construir un prototipo físico funcional de la caja con el circuito ESP32 y realizar pruebas de simulación de ruta de 20 minutos midiendo la respuesta de temperatura y el funcionamiento de alarmas y notificaciones. |

## 1.3. Segmentos objetivo.

Cold2Hot está dirigido a tres segmentos clave dentro del ecosistema de entregas a domicilio en Lima Metropolitana y principales ciudades urbanas del Perú:

1. Restaurantes y Empresas de Catering o Delivery:
   * Perfil Demográfico y Operativo: Establecimientos gastronómicos de tamaño mediano y pequeño dedicados a la venta de alimentos preparados en zonas urbanas con alto flujo de despacho a domicilio.
   * Sustento Estadístico: Según la Cámara de Comercio de Lima, el sector de restaurantes y delivery creció más del 25% en el último trienio, representando más del 30% del volumen total de ventas en hora pico.
   * Necesidad Principal: Garantizar la calidad percibida del platillo entregado, disminuir la tasa de reembolsos por entregas frías y contar con un registro auditable del despacho.

2. Repartidores de Delivery:
   * Perfil Demográfico y Operativo: Hombres y mujeres de 18 a 45 años, trabajadores independientes o en plantilla de restaurantes, que transitan en motocicletas o bicicletas de 6 a 10 horas diarias.
   * Sustento Estadístico: En Lima operan más de 45000 repartidores activos en servicios de delivery. Aproximadamente el 65% realiza trayectos que superan los 12 minutos de duración por viaje.
   * Necesidad Principal: Sistemas automatizados que no demanden manipulación continua mientras conducen, y avisos sonoros o móviles inmediatos ante la apertura no deseada de la mochila o caja de carga.

3. Consumidores Finales:
   * Perfil Demográfico: Hombres y mujeres de 18 a 60 años de los niveles socioeconómicos A, B y C1 que habitan en zonas urbanas y solicitan delivery de comida de 2 a 4 veces por semana.
   * Sustento Estadístico: Reportes del INEI indican que el 58% de los usuarios de delivery han experimentado al menos una mala experiencia por recibir comida tibia o fría en los últimos 6 meses.
   * Necesidad Principal: Disfrutar de sus platillos en la temperatura adecuada de consumo, con la certeza de que la caja se mantuvo sellada e higiénica durante todo el traslado.


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
