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
### 4.2.2 Labeling Systems
### 4.2.3 SEO Tags and Meta Tags
### 4.2.4 Searching Systems
### 4.2.5 Navigation Systems
## 4.3 Landing Page UI Design
### 4.3.1 Landing Page Wireframe
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
### 4.6.3 Software Architecture Container Diagrams
### 4.6.4 Software Architecture Components Diagrams
## 4.7 Software Object-Oriented Design
### 4.7.1 Class Diagrams
## 4.8 Database Design
### 4.8.1 Database Diagrams
