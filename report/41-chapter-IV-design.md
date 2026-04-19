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
