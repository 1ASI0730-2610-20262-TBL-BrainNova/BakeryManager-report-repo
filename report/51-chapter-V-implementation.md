# Capítulo V: Product Implementation, Validation & Deployment

## 5.1. Software Configuration Management

### 5.1.1. Software Development Environment Configuration

A continuación, se listan las herramientas y estándares adoptados por el equipo para el desarrollo colaborativo del sistema:

| Actividad | Herramienta / Guía  | Propósito                   | Tipo de Acceso / Ruta                                         |
| --------- |---------------------|-----------------------------|---------------------------------------------------------------|
| Project Management | Trello              | Seguimiento de backlog, tareas y sprints | [https://trello.com/](https://trello.com/)                         |
| Requirements Management | Gherkin Conventions | Escritura legible de requisitos con formato Given/When/Then | [https://cucumber.io/docs/gherkin/](https://cucumber.io/docs/gherkin/) |
| Product UX/UI Design | Figma               | Prototipos y diseño Responsive | [https://figma.com](https://figma.com)                        |
| Version Control | Git + GitHub        | Gestión colaborativa del código fuente | [https://github.com](https://github.com)                      |
| Software Deployment | Netlify             | Despliegue de Landing Pages | [https://www.netlify.com](https://www.netlify.com)            |

### 5.1.2. Source Code Management

En esta sección el equipo establece los medios y esquema de organización que aplicará para el seguimiento de modificaciones. Para ello se utilizará **GitHub** como plataforma y sistema de control de versiones.

A continuación se indican los URLs de los repositorios de GitHub para cada producto:

- **Business Web Page**: [https://github.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo](https://github.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo)

#### GitFlow Workflow

Se implementará el modelo de ramificación propuesto por Vincent Driessen en su artículo *“A successful Git branching model”*, conocido como **GitFlow**. Este modelo organiza el trabajo en las siguientes ramas:

- `main`: Rama principal, contiene siempre el código en producción.
- `develop`: Rama de desarrollo principal, donde se integran las funcionalidades antes de pasar a producción.
- `feature/*`: Ramas creadas a partir de `develop` para desarrollar nuevas funcionalidades.**Convención de nombres:** `feature/<nombre-corto-descriptivo>`_Ejemplo: `feature/login-auth`_
  **Convención de nombres:** `feature/<descripción-corta>`
  _Ejemplo: `feature/version-testing`_

#### Convenciones de Commits

Se utilizará el estándar de **Conventional Commits** para los mensajes de commits. Esto facilitará la automatización en los procesos de integración continua y generación de changelogs.

**Ejemplos:**

- `feat: add login functionality`
- `fix: correct null pointer exception on user service`
- `chore: update dependencies`
- `docs: add and update documents`

### 5.1.3. Source Code Style Guide & Conventions

### 5.1.4. Software Deployment Configuration

---

## 5.2. Landing Page, Services & Applications Implementation

### 5.2.1. Sprint 1

#### 5.2.1.1. Sprint Planning 1
El **sprint** es aquel periodo corto y de periodo fijo durante el cual es desarrollado un conjunto de tareas o actividades específicas en un proyecto, el cual está estrechamente relacionado con metodologías ágiles como **Scrum**.

El **Sprint #1** tiene como fecha de inicio el **07/04/2026** y plantea elaborar una **Landing Page** atractiva para **BakeryManager** que capte la atención de nuestros segmentos objetivos.

| Concepto | Detalle |
| :--- | :--- |
| **Sprint #** | Sprint 1 |
| **Sprint Planning Background** | |
| **Date** | 07/04/2026 |
| **Time** | 5:00 PM - 6:30 PM |
| **Location** | Google Meet |
| **Prepared by** | Molina Vásquez Manuel Alejandro |
| **Attendees** | • Molina Vásquez, Manuel Alejandro (u20221g231)<br>• Tufiño Argüelles, Luis Angel (U202216240)<br>• Céspedes Pillco, Jarod Jack (u202318588)<br>• Vidal Malaga, Jareth Beycker (u202316878)<br>• Chipana Huarancca, Emanuel (u202214074) |
| **Sprint 0 Review Summary** | Diseño y Desarrollo del Landing Page |
| **Sprint 0 Retrospective Summary** | Completar los diseños y estandarizar el lenguaje usado en el desarrollo y presentación del landing page. |
| **Sprint Goal & User Stories** | |
| **Sprint 1 Goal** | Elaborar, diseñar y desplegar una Landing Page atractiva e informativa para la aplicación **BakeryManager**. |
| **Sprint 1 Velocity** | 15 |
| **Sum of Story Point** | 18 |

#### 5.2.1.2. Aspect Leaders and Collaborators

#### 5.2.1.3. Sprint Backlog 1

#### 5.2.1.4. Development Evidence for Sprint Review

#### 5.2.1.5. Execution Evidence for Sprint Review

#### 5.2.1.6. Services Documentation Evidence for Sprint Review

#### 5.2.1.7. Software Deployment Evidence for Sprint Review

#### 5.2.1.8. Team Collaboration Insights during Sprint

