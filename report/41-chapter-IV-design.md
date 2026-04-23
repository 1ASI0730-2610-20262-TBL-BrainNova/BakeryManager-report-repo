# Capítulo IV: Product Design
## 4.1 Style Guidelines
### 4.1.1 General Style Guidelines
En esta sección se detallan las decisiones de diseño y las referencias visuales que constituyen la identidad de **BakeryManager**. El estilo ha sido diseñado para evocar la calidez del sector artesanal de la panadería, integrada con la precisión técnica de una plataforma IoT.

#### **A. Branding & Visual Concept**
La identidad visual se centra en el concepto de **"Panadería Inteligente"**. El branding utiliza una combinación de colores tierra que remiten al proceso de horneado (trigo, corteza, café), contrastando con una interfaz moderna y limpia que simboliza la tecnología de sensores. El objetivo es transmitir que la tradición y la eficiencia tecnológica pueden coexistir para optimizar la rentabilidad de las PYMES peruanas.

#### **B. Typography**
Se ha implementado una jerarquía tipográfica dual para equilibrar elegancia y funcionalidad, utilizando fuentes de Google Fonts:

* **Display / Headings (Playfair Display):** Se utiliza esta fuente *Serif* para los títulos principales. Su diseño clásico, con remates pronunciados y grosores variables, comunica la calidad artesanal y la herencia de la industria panadera.
* **Body / UI (DM Sans):** Para el cuerpo de texto, descripciones de módulos y datos del dashboard, se utiliza esta fuente *Sans Serif* moderna. Se seleccionó por su excelente legibilidad en pantallas digitales, permitiendo que los usuarios lean rápidamente las métricas de los sensores sin fatiga visual.

#### **C. Colors (Color Palette)**
La paleta de colores es el pilar de la identidad visual, gestionada mediante variables CSS para asegurar la consistencia en toda la plataforma:

* **Paleta Base (Warm tones):**
    * `Cream` (#F9F4EC): Utilizado como fondo principal para dar una sensación de limpieza y amplitud.
    * `Wheat` (#E8D5B0): Color secundario para fondos de secciones y divisiones.
* **Colores de Acción y Énfasis:**
    * `Caramel` (#C4862B) y `Accent` (#D4691E): Utilizados en botones (CTAs) y estados destacados, evocando el color del pan recién horneado.
    * `Espresso` (#2C1A0E): Color de contraste para textos principales y navegación.
* **Colores de Estado (Feedback):**
    * `Success` (#5A8A5F): Utilizado para indicar que los sensores están operativos y dentro de los rangos normales.
    * `Alert/Critical`: Se reservan tonos anaranjados y rojizos oscuros para incidencias de seguridad (humo, gas, temperatura crítica).

#### **D. Spacing & Dimensions**
Se ha adoptado un sistema de diseño basado en la suavidad y la profundidad:
* **Radios de Curvatura (Radius):** Se aplica un `border-radius: 14px` de forma consistente en tarjetas (cards) y botones. Esto elimina la rigidez de la interfaz y la hace más amigable para el usuario.
* **Profundidad (Shadows):** Se utiliza una sombra personalizada (`0 8px 40px rgba(44,26,14,0.12)`) que otorga una elevación visual a los paneles de monitoreo, permitiendo que la información crítica sobresalga del fondo.
* **Grid System:** El diseño emplea un sistema de rejilla adaptable (*Responsive Grid*) que asegura que los paneles de sensores se reorganicen de forma fluida desde monitores de escritorio hasta dispositivos móviles.

#### **E. Tone of Communication & Language**
El tono de comunicación se ha definido bajo tres dimensiones principales:
* **Respetuoso y Humano:** La plataforma utiliza un lenguaje cercano (ej. *"Manage your bakery with real intelligence"*) y toques emocionales (ej. *"Hecho con 🍞 en Lima"*), reconociendo el esfuerzo del emprendedor panadero.
* **Directo y Accionable:** En los paneles operativos, el lenguaje es conciso para facilitar respuestas rápidas ante incidencias (ej. *"Check Oven 2"* o *"Active"*).
* **Bilingüismo:** Al estar implementada con un sistema de traducción dinámica (i18n), la comunicación es inclusiva para usuarios que prefieran el entorno en Inglés o Español, manteniendo la precisión técnica en ambos idiomas.

#### **F. Design System Reference**
Aunque el diseño es una propuesta original de **Brainova**, toma como referencia los principios de **Atomic Design** para la construcción de componentes reutilizables (botones, chips de estado, formularios), garantizando que la interfaz sea escalable conforme se agreguen nuevos tipos de sensores IoT.

### 4.1.2 Web Style Guidelines
En esta sección se definen los estándares de interacción y adaptabilidad de la interfaz web de **BakeryManager**, garantizando una experiencia de usuario fluida y coherente en diversos navegadores y dispositivos.

#### **A. Estrategia de Responsive Design**
La plataforma utiliza un enfoque de diseño fluido basado en **CSS Flexbox** y **CSS Grid**, permitiendo que la arquitectura de información se reorganice mediante *breakpoints* específicos definidos en la hoja de estilos:

* **Desktop (> 1100px):** Disposición multi-columna (grid de 3 a 4 columnas) para maximizar la visualización de datos de sensores y analíticas en paneles extendidos.
* **Tablet (900px - 1100px):** Se ajusta el padding de los contenedores a `1.5rem` y las rejillas de tarjetas de sensores se fuerzan a un máximo de 2 columnas (`grid-template-columns: 1fr 1fr`) para mantener la legibilidad de las métricas.
* **Mobile (< 900px):** La interfaz transita a una disposición de columna única (`1fr`). Se ocultan elementos visuales secundarios (`.hero-visual { display: none }`) para priorizar la lectura de alertas y estados operativos del sistema IoT en pantallas pequeñas.

#### **B. Interacción y Feedback Visual**
Se han implementado estándares de micro-interacciones para mejorar la respuesta del sistema ante las acciones del usuario:

* **Comportamiento de Scroll:** Se aplica `scroll-behavior: smooth` de forma global en el documento HTML, asegurando transiciones suaves al navegar entre las secciones de la Landing Page.
* **Estados de Interacción (Hover):** Los elementos clicables (botones, enlaces y tarjetas) presentan transiciones de opacidad y color suaves (`0.6s ease`).
* **Tipografía Adaptable:** Se utiliza la función `clamp(14px, 1.1vw, 17px)` para el tamaño de fuente base, permitiendo que el texto escale de forma armónica según el tamaño de la ventana del navegador.

#### **C. Animaciones y Carga Progresiva**
Para reducir la carga cognitiva y guiar la atención del usuario hacia la información relevante, se utiliza la técnica de **Intersection Observer** en JavaScript:

* **Clase `.fade-up`:** Los componentes clave (secciones de características y planes) aparecen con una transición de opacidad y un desplazamiento vertical de `28px`.
* **Sustento:** Esta animación asegura que los elementos se presenten de forma ordenada conforme el usuario realiza el scroll, evitando que la interfaz se sienta saturada desde el primer contacto.

#### **D. Estándares de Componentes Web**
* **Navegación (Navbar):** Se mantiene un diseño minimalista con soporte para **internacionalización (i18n)**. La navegación permite el cambio dinámico entre inglés y español sin recarga de página, utilizando atributos `data-i18n` para actualizar el DOM en tiempo real.
* **Tarjetas de Datos (Cards):** Utilizan un radio de borde de `14px` y sombras profundas para jerarquizar la información de los sensores. Cada tarjeta incluye etiquetas de estado dinámicas que facilitan el monitoreo rápido.

#### **E. Accesibilidad y Rendimiento**
* **Optimización de Carga:** Se utiliza la precarga de fuentes de Google Fonts y la organización de recursos mediante enlaces críticos en el `<head>`.
* **Semántica HTML5:** Se emplean etiquetas estructurales (`<header>`, `<section>`, `<footer>`) para asegurar que la jerarquía de la página sea comprensible tanto para usuarios como para motores de búsqueda (SEO).

## 4.2 Information Architecture
### 4.2.1 Organization Systems

En esta sección se definen las estrategias para agrupar y presentar la información en **BakeryManager**, asegurando que tanto el dueño de la panadería como el personal operativo encuentren los datos de manera intuitiva y eficiente.

### A. Sistemas de Organización Visual

El equipo ha determinado el uso de tres estructuras principales según el contexto de la información:

#### 1. Organización Jerárquica (Visual Hierarchy)

- **Aplicación:**  
  Se aplica en el *Dashboard* principal y en las secciones de presentación del producto. Se utilizan variaciones de tamaño y peso tipográfico (fuente *Playfair Display* para títulos y *DM Sans* para datos) para dirigir la atención del usuario primero a las alertas críticas y luego a las métricas secundarias.

- **Sustento:**  
  Permite que un administrador identifique problemas (ej. una fuga de gas) en milisegundos antes de revisar los reportes históricos.

#### 2. Organización Secuencial (Step-by-step)

- **Aplicación:**  
  Se utiliza en el flujo de registro de nuevos sensores y en el proceso de solución de incidentes.

- **Sustento:**  
  Guía al usuario a través de pasos lógicos (ej.  
  1. Detectar alerta
  2. Confirmar recepción  
  3. Cerrar incidente),  
  reduciendo la posibilidad de error humano en tareas críticas.

#### 3. Organización Matricial

- **Aplicación:**  
  Se emplea en la sección de analíticas y en el inventario de sensores (*Registered Sensors*).

- **Sustento:**  
  Permite cruzar múltiples dimensiones de datos, como comparar la temperatura de diferentes hornos frente a distintas franjas horarias.

### B. Esquemas de Categorización de Contenido

Para facilitar el acceso a la información, se han implementado los siguientes esquemas:

#### 1. Categorización por Tópicos (Temática)

- **Uso:**  
  La funcionalidad de la plataforma se divide en cuatro módulos o “épicas” principales: Producción, Gestión de Incidentes, Analítica y Gestión de Sensores.

- **Sustento:**  
  Ayuda a los usuarios a localizar herramientas específicas según el área operativa que deseen atender.

#### 2. Categorización según Audiencia (Grupos de Usuarios)

- **Uso:**  
  La información se filtra y presenta de forma diferenciada para tres roles:  
  - Owner/Manager (visión global)  
  - Branch Manager (control operativo)  
  - Master Baker (monitoreo de producción)

- **Sustento:**  
  Evita la sobrecarga de información, entregando a cada perfil solo los datos necesarios para su responsabilidad específica.

#### 3. Categorización Cronológica

- **Uso:**  
  Aplicado estrictamente en el historial de incidentes (*Incident Panel*) y en los gráficos de tendencias de temperatura.

- **Sustento:**  
  Es vital para identificar patrones de fallas en los equipos a lo largo del tiempo y evaluar la eficiencia de los turnos de trabajo.
### 4.2.2 Labeling Systems

En esta sección se detallan las convenciones de etiquetado utilizadas en **BakeryManager**. El objetivo es reducir la carga cognitiva del usuario mediante el uso de términos breves, precisos y consistentes que faciliten la gestión operativa bajo condiciones de alta presión.

### A. Estándares de Etiquetado

Para garantizar la simplicidad, el equipo ha definido tres principios de representación:

#### 1. Etiquetas de Navegación (Menu Labels)

- **Aplicación:**  
  Se utilizan términos de una sola palabra para las secciones principales de la plataforma, visibles en el encabezado y pie de página.

  - Features (Funcionalidades)  
  - About (Nosotros)  
  - Pricing (Planes)  
  - Segments (Roles)

- **Sustento:**  
  El uso de términos simples evita la confusión y permite una navegación rápida en dispositivos móviles donde el espacio es limitado.

#### 2. Etiquetas de Estado y Alerta (Status Labels)

- **Aplicación:**  
  Los datos provenientes de los sensores IoT se representan con etiquetas de estado binarias o de prioridad, asociadas a colores semánticos.

  - **Active / Operational:** Funcionamiento normal  
  - **Check / Warning:** Requiere atención preventiva  
  - **Critical / Emergency:** Incidencia grave (fugas, incendios)

- **Sustento:**  
  La asociación entre el texto mínimo y el color permite que el personal operativo tome decisiones de seguridad sin necesidad de leer manuales complejos.

#### 3. Etiquetas de Identificación de Datos (Data Labels)

- **Aplicación:**  
  En las tablas de analítica y gestión de dispositivos, se utilizan etiquetas técnicas estandarizadas:

  - **ID:** Identificador único del sensor  
  - **Type:** Categoría del dispositivo (Temperatura, Humedad, Gas)  
  - **Equipment:** Máquina asociada (Horno 1, Cámara Fría)  
  - **Status:** Estado actual de la conexión

- **Sustento:**  
  La brevedad de estas etiquetas permite que las tablas sean legibles en interfaces responsivas sin necesidad de realizar *scroll* horizontal excesivo.

### B. Asociaciones de Información

Las etiquetas se agrupan para crear relaciones lógicas inmediatas:

#### 1. Asociación Sensor–Ubicación

- **Representación:**  
  `[Nombre del Equipo] — [Valor de Métrica] · [Estado]`

- **Ejemplo:**  
  `Oven 1 — 220°C · Active`

- **Propósito:**  
  Brinda el contexto completo de una operación en una sola línea de texto.

#### 2. Asociación de Planes y Beneficios

- **Representación:**  
  `[Nombre del Plan] / [Precio] + Lista de beneficios con checkmarks`

- **Ejemplo:**  
  `Starter / S/89`

- **Propósito:**  
  Facilita la comparación rápida de costos y capacidades mediante una estructura visual repetitiva.
  
### 4.2.3 SEO Tags and Meta Tags
Los SEO Tags y Meta Tags optimizan la visibilidad de BakeryManager en motores de búsqueda. Se definen específicamente para el Landing Page (sitio estático) para maximizar la captación de clientes, utilizando etiquetas claras que resaltan el valor de la integración IoT en panaderías.
##### Landing Page
```html
<title>BakeryManager – Brainova | Smart Bakery Management Platform</title>
<meta name="description" content="BakeryManager is an IoT-powered web platform for bakeries and SMEs. Monitor ovens, fermentation and refrigeration in real time with automatic alerts and historical analytics.">
<meta name="keywords" content="bakery management, IoT sensors, bakery software, incident management, analytics, ERP SME, Peru">
<meta name="author" content="Brainova – UPC">
<meta name="robots" content="index, follow">
<meta property="og:title" content="BakeryManager – Smart Bakery Management Platform">
<meta property="og:description" content="Connect IoT sensors to your bakery and monitor everything in real time — with automatic alerts, incident management and historical analytics.">
<meta property="og:type" content="website">
<meta property="og:image" content="https://bakery-manager-51fa66.netlify.app/images/LOGO-Bake.jpeg">
<meta property="og:url" content="https://bakery-manager-51fa66.netlify.app">
```
### 4.2.4 Searching Systems

En esta sección se explican los medios que **BakeryManager** ofrece para que el usuario localice información específica rápidamente, evitando que se pierda entre los datos generados por los sensores.


### A. Opciones de Búsqueda y Filtros

Se han implementado herramientas de búsqueda directa y filtros avanzados en los módulos críticos:

#### 1. Búsqueda de Dispositivos e Incidentes

- **Opciones:**  
  Barra de búsqueda con autocompletado en el inventario de sensores y en el historial de incidentes.

- **Filtros:**  
  - **Por Tipo:** Temperatura, Humedad, Gas  
  - **Por Estado:** Activo, Alerta, Crítico  
  - **Por Fecha:** Filtro cronológico para reportes históricos  

#### 2. Filtros de Gestión Operativa

- **Opciones:**  
  Menús desplegables para filtrar datos según la sede o el equipo específico (ej. Horno 1, Almacén).

- **Filtros:**  
  - **Prioridad:** Alta, Media, Baja  
  - **Asignado:** Búsqueda por el responsable del turno  

### B. Visualización de Resultados

La forma en que se muestran los datos tras una búsqueda sigue los principios de claridad del sistema:

- **Formato de Lista:**  
  Los resultados se presentan en tablas limpias o tarjetas (*cards*) que resaltan el estado actual con colores semánticos (verde, amarillo, rojo).

- **Gráficos Dinámicos:**  
  Al buscar datos históricos, el sistema genera automáticamente un gráfico de líneas para visualizar la tendencia de la métrica consultada.

### 4.2.5 Navigation Systems

Los sistemas de navegación guían a los usuarios a través del **Landing Page** y la **Web Application**, asegurando que cumplan sus objetivos (monitorear sensores, gestionar incidentes) con el mínimo esfuerzo y máxima claridad operativa.


### A. Landing Page Navigation

El Landing Page utiliza un diseño limpio con un menú fijo superior para facilitar el acceso rápido a la información comercial.

- **Menú Superior:**  
  Incluye accesos directos a *Features*, *Pricing*, *About* y *Segments*.

- **Scroll Suave:**  
  Transiciones fluidas mediante *smooth scroll* para conectar secciones, con anclas que dirigen al usuario a los planes o beneficios específicos.

- **Enlaces Internos:**  
  Botones de **"Get Started"** vinculan directamente a la web.

#### Flujo

1. Los usuarios llegan al Landing Page y exploran la propuesta de valor IoT.  
2. Los botones de acción (*CTAs*) distribuidos en la página llevan al proceso de registro.  
3. El menú persistente permite saltar entre la comparativa de precios y las funcionalidades técnicas sin perder el hilo de la navegación.  

### B. Web Application Navigation

La navegación se personaliza mediante un menú lateral dinámico que cambia según el rol del usuario autenticado, asegurando que cada perfil acceda solo a las herramientas que le corresponden.

- **Menú Lateral:**  
  Acceso a módulos según rol. En dispositivos móviles, se integra en un menú tipo hamburguesa.

- **Barra Superior de Notificaciones:**  
  Ícono de campana con alertas críticas de sensores (Gas, Fuego, Temperatura), accesible desde cualquier vista.

- **Breadcrumbs y Títulos:**  
  Indicadores visuales que muestran la ubicación actual del usuario dentro de la jerarquía de la aplicación.

### C. Flujo para Owner / Manager

1. **Dashboard:**  
   Resumen ejecutivo y métricas globales de rentabilidad y producción.

2. **Organization:**  
   Gestión de múltiples sedes y suscripción.

3. **Analytics:**  
   Reportes avanzados y proyecciones.

### D. Flujo para Branch Manager

1. **Dashboard:**  
   Control operativo de su sede específica.

2. **Inventory:**  
   Gestión de stock de insumos y productos terminados.

3. **Staff:**  
   Supervisión del personal y turnos de trabajo.

### E. Flujo para Master Baker

1. **Monitor:**  
   Vista en tiempo real de hornos y cámaras de fermentación.

2. **Incident Panel:**  
   Recepción y resolución de alertas técnicas.

3. **Device Setup:**  
   Calibración y estado de conexión de los sensores IoT.
   
## 4.3 Landing Page UI Design
### 4.3.1 Landing Page Wireframe
<img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/feature/Chapter4/report/assets/Hero.png" alt="BakeryManager Hero" width="100%">
<img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/feature/Chapter4/report/assets/About%20Brainova.png" alt="About Brainova" width="100%">
<img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/feature/Chapter4/report/assets/Pain%20points.png" alt="Pain Points" width="100%">
<img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/feature/Chapter4/report/assets/FEATURES1.PNG" alt="Features Part 1" width="100%">
<img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/feature/Chapter4/report/assets/FEATURES2.PNG" alt="Features Part 2" width="100%">
<img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/feature/Chapter4/report/assets/Segmentos%20(roles).png" alt="Segmentos y Roles" width="100%">
<img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/feature/Chapter4/report/assets/Pricing.png" alt="Pricing Section" width="100%">
<img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/feature/Chapter4/report/assets/Footer.png" alt="Footer Section" width="100%">

### 4.3.2 Landing Page Mock-up
## 4.4 Web Applications UX/UI Design
### 4.4.1 Web Applications Wireframes
### 4.4.2 Web Applications Wireflow Diagrams
### 4.4.3 Web Applications Mock-ups
### 4.4.4 Web Applications User Flow Diagrams
## 4.5 Web Applications Prototyping
## 4.6 Domain-Driven Software Architecture
### 4.6.1 Design-Level Event Storming
### 4.6.2 Software Architecture Context Diagram

El siguiente diagrama de contexto  presenta una vista de alto nivel de BakeryManager como sistema central, mostrando sus interacciones con los actores y sistemas externos que forman parte de su entorno. El sistema es utilizado por dos tipos de usuarios: el Propietario/Administrador, quien supervisa múltiples sedes, monitorea equipos y consulta dashboards en tiempo real, y el Personal Operativo, quien gestiona el inventario y recibe alertas operativas. A nivel de sistemas externos, BakeryManager se integra con una Plataforma IoT en la Nube (AWS IoT Core / Firebase), la cual recibe y procesa los datos enviados por los Dispositivos IoT / Sensores instalados en los equipos críticos de las panaderías, como hornos y cámaras frigoríficas.

<img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/refs/heads/feature/Chapter4/report/assets/ContextDiagram-V1.PNG" alt="Context Diagram" width="800">


### 4.6.3 Software Architecture Container Diagrams

El siguiente diagrama de contenedores  descompone BakeryManager en sus principales bloques tecnológicos, mostrando cómo se distribuyen las responsabilidades y cómo se comunican entre sí. La solución está conformada por un Landing Page estático desplegado en Netlify (HTML5, CSS3, JavaScript), una Frontend Web Application desarrollada en Angular 17 y desplegada en Firebase Hosting, y cuatro RESTful APIs desarrolladas con Spring Boot (Java) y desplegadas en Azure mediante Docker: Identity & Access Management API, IoT Monitoring API, Inventory API y Production Monitoring API. Todas las APIs comparten una base de datos relacional PostgreSQL alojada en Azure Database for PostgreSQL. La comunicación entre el frontend y las APIs se realiza mediante REST sobre HTTPS, mientras que los datos de sensores llegan desde la Plataforma IoT en la Nube vía REST API, y los sensores físicos envían datos a dicha plataforma mediante el protocolo MQTT/TLS.

<img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/refs/heads/feature/Chapter4/report/assets/ContainerDiagram-V2.png" alt="Container Diagram" width="800">


### 4.6.4 Software Architecture Components Diagrams

Los siguientes diagramas de componentes  descomponen cada uno de los contenedores del backend, identificando los bloques estructurales internos, sus responsabilidades y las tecnologías utilizadas. Cada API sigue el patrón Controller → Service → Repository → Domain Model, propio del desarrollo con Spring Boot, lo que garantiza una separación clara de responsabilidades y facilita el mantenimiento y escalabilidad del sistema.

**Identity & Access Management API**

Gestiona la autenticación, autorización y control de acceso basado en roles. Sus componentes principales son el Auth Controller y User Controller como puntos de entrada REST, el Auth Service y User Service como capa de lógica de negocio, el User Repository para la persistencia, el User Domain Model con las entidades User, Role y Permission, y el Security Configuration que define las políticas de seguridad mediante Spring Security y JWT.

<img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/refs/heads/feature/Chapter4/report/assets/IdentityAPIComponents-dark.png" alt="Identity API Component Diagram" width="800">

**Inventory API**

Gestiona el inventario de insumos y el control de stock de la panadería. Sus componentes incluyen el Inventory Controller y Stock Controller como endpoints REST, el Inventory Service y Stock Service como capa de negocio encargada del seguimiento de movimientos y detección de bajo stock, los repositorios correspondientes para persistencia, y el Inventory Domain Model con las entidades Inventory, Stock y StockMovement.

<img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/refs/heads/feature/Chapter4/report/assets/InventoryAPIComponents-dark.png" alt="Inventory API Component Diagram" width="800">

**IoT Monitoring API**

Procesa en tiempo real los datos provenientes de los sensores IoT, gestiona incidentes y genera alertas automáticas. Sus componentes incluyen el Sensor Controller, Incident Controller y Alert Controller como puntos de entrada REST y WebSocket, los servicios correspondientes que implementan la lógica de detección de anomalías y ciclo de vida de incidentes, los repositorios de persistencia, el IoT Domain Model con las entidades Sensor, Incident, Alert y EventHistory, y el IoT Platform Client encargado de consumir datos desde la plataforma IoT externa.

<img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/refs/heads/feature/Chapter4/report/assets/IoTAPIComponents-dark.png" alt="IoT API Component Diagram" width="800">

**Production Monitoring API**

Gestiona el control de producción y la supervisión de múltiples sedes. Sus componentes incluyen el Production Controller y Branch Controller como endpoints REST, el Production Service y Branch Service como capa de negocio para la gestión de lotes de producción y sedes, los repositorios de persistencia correspondientes, y el Production Domain Model con las entidades ProductionBatch, Branch, Oven y RefrigerationChamber.

<img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/refs/heads/feature/Chapter4/report/assets/ProductionAPIComponents-dark.png" alt="Production API Component Diagram" width="800">

### 4.7.1 Class Diagrams

A continuación se presentan los Class Diagrams de UML para cada uno de los bounded contexts identificados en BakeryManager. Cada diagrama incluye clases, interfaces, enumeraciones, atributos con su scope (private, public, protected), métodos y relaciones con nombre, dirección y multiplicidad.


#### Identity & Access Management

Este diagrama representa el bounded context encargado de la autenticación, autorización y control de acceso basado en roles. La clase central es `User`, que se asocia con `Role` (relación muchos a uno) para determinar el nivel de acceso del usuario dentro del sistema. A su vez, `Role` se compone de múltiples instancias de `Permission` a través de la tabla intermedia `RolePermission`, permitiendo una gestión granular de permisos. La clase `Session` registra los tokens JWT activos asociados a cada usuario autenticado. Las enumeraciones `RoleType` y `PermissionType` garantizan la integridad de los valores permitidos para roles y permisos respectivamente. El `AuthService` gestiona el ciclo de vida de la autenticación, incluyendo login, logout y validación de tokens.

<img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/refs/heads/feature/Chapter4/report/assets/IAM%20DIAGRAM.jpeg" alt="Identity & Access Management Class Diagram" width="800">

#### Inventory Management

Este diagrama representa el bounded context responsable de la gestión de insumos y control de stock de la panadería. La clase `Inventory` agrupa múltiples instancias de `InventoryItem` (relación uno a muchos), donde cada ítem representa un insumo específico con su unidad de medida y nivel mínimo de stock. Cada `InventoryItem` está asociado a exactamente una instancia de `Stock` (relación uno a uno), que mantiene el nivel actual y el estado del stock. Los movimientos de entrada, salida y ajuste quedan registrados en `StockMovement` (relación uno a muchos con `Stock`). La enumeración `MovementType` define los tipos de movimiento permitidos y `StockStatus` refleja el estado actual del stock. El `InventoryService` y `StockService` implementan la lógica de negocio para la gestión y detección de bajo stock.

<img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/refs/heads/feature/Chapter4/report/assets/INVENTORY%20DIAGRAM.jpeg" alt="Inventory Management Class Diagram" width="800">


#### IoT Monitoring

Este diagrama representa el bounded context encargado del monitoreo en tiempo real de los sensores instalados en los equipos críticos de la panadería. La clase `Sensor` es el elemento central, registrando lecturas continuas mediante `SensorReading` (relación uno a muchos). Cuando una lectura supera los umbrales configurados, el sistema genera un `Incident` (relación uno a muchos con `Sensor`), el cual a su vez produce una `Alert` (relación uno a uno) y registra eventos en `EventHistory` (relación uno a muchos). Las enumeraciones `SensorType`, `SensorStatus`, `IncidentStatus` y `AlertSeverity` garantizan la consistencia de los valores en el sistema. El `SensorService`, `IncidentService` y `AlertService` orquestan el flujo de detección, gestión de incidentes y despacho de alertas en tiempo real mediante WebSocket.

<img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/refs/heads/feature/Chapter4/report/assets/IOT%20DIAGRAM.jpeg" alt="IoT Monitoring Class Diagram" width="800">


#### Production Monitoring

Este diagrama representa el bounded context responsable de la gestión de la producción y supervisión de múltiples sedes. La clase `Branch` es el elemento central, agrupando el equipamiento (`Equipment`) y los lotes de producción (`ProductionBatch`). La clase `Equipment` es extendida por `Oven` y `RefrigerationChamber`, representando los equipos específicos monitoreados mediante herencia. Cada `ProductionBatch` se asocia con una `Branch`, un `Oven` y un `InventoryItem` del bounded context de inventario, reflejando el consumo de insumos durante la producción. La enumeración `BatchStatus` controla el ciclo de vida de cada lote y `EquipmentStatus` refleja el estado operativo de los equipos. El `ProductionService` y `BranchService` implementan la lógica de negocio para la gestión de lotes y sedes respectivamente.

<img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/refs/heads/feature/Chapter4/report/assets/PRODUCTION%20DIAGRAM.jpeg" alt="Production Monitoring Class Diagram" width="800">

## 4.8 Database Design
### 4.8.1 Database Diagrams
