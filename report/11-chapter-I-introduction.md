# Capítulo I: Introducción
## 1.1. Startup Profile
### 1.1.1. Descripción de la Startup

Somos Brainova, un equipo de estudiantes de la Universidad Peruana de Ciencias Aplicadas comprometidos con el desarrollo de soluciones tecnológicas innovadoras para optimizar la gestión de negocios como panaderías, pastelerías y otros emprendimientos en crecimiento. Nuestra propuesta consiste en una plataforma web que permite mejorar la eficiencia operativa, automatizar procesos y facilitar la toma de decisiones mediante el uso de tecnología.

Para ello, uno de nuestros productos es **BakeryManager**, una solución enfocada en negocios de panadería que integra el control de producción, monitoreo de maquinaria y supervisión de condiciones operativas mediante sensores IoT, permitiendo una gestión más eficiente, centralizada y en tiempo real de sus operaciones, especialmente en entornos multisede.

**Misión:**  
Nuestra misión es desarrollar soluciones digitales que optimicen la gestión operativa de panaderías en crecimiento, mediante el monitoreo en tiempo real de sus procesos productivos y equipos a través de tecnología IoT. Buscamos mejorar la eficiencia, reducir pérdidas y facilitar la supervisión de múltiples sedes a través de una plataforma centralizada.

**Visión:**  
Nuestra visión es ser una solución tecnológica líder en la digitalización del sector panadero, destacando por integrar monitoreo inteligente mediante IoT y gestión operativa en una sola plataforma, contribuyendo al crecimiento sostenible y a la modernización de las panaderías MYPES.
## 1.1.2. Perfiles de integrantes del equipo

## 1.1.2.1 Integrantes del Equipo

| Foto                                                     | Nombre | Código | Descripción |
|----------------------------------------------------------|--------|--------|-------------|
| ![Integrante](./assets/LuisTufino.png)                   | **Tufiño Argüelles Luis Angel** | U202216240 | Elegí la carrera de Ingeniería de Software motivado por mi interés en comprender cómo funcionan los programas. Durante la pandemia, comencé a modificar juegos sencillos, iniciando así mi camino en la programación. Tengo conocimientos en C++, Python y JavaScript, además de experiencia en desarrollo web con HTML y CSS y en la creación de bots usando Python. También desarrollé una aplicación web para el negocio familiar, aplicando conceptos de bases de datos y diseño UX/UI. Considero que mi creatividad y capacidad de trabajo en equipo aportan positivamente al desarrollo de este proyecto. |
| ![Integrante](./assets/ManuelMolina.jpg)                 | **Molina Vásquez Manuel Alejandro** | U20221G231 | Escogí la carrera de Ingeniería de Software porque me interesa comprender el funcionamiento de diversos programas y los algoritmos utilizados en ellos. Tengo conocimientos en C#, C++, Python, HTML y CSS, además de experiencia en el desarrollo de aplicaciones web y manejo de bases de datos. Considero que una de mis principales fortalezas es mi capacidad de trabajo en equipo, lo cual contribuye al cumplimiento de los objetivos del proyecto. |
| ![Integrante-Jarod-Cespedes](./assets/JarodCespedes.png) | **Cespedes Pillco, Jarod Jack** | U202318588 | Elegí la carrera de Ingeniería de Software por el interés mío de entender cómo los videojuegos y programas en general funcionaban y cómo eran creados. Tengo experiencia con los lenguajes de programación C++, C#, Visual Basic, Python y Java, además tengo habilidad en el desarrollo de interfaces web con el lenguaje de tipado HTML y CSS. Considero que soy una persona creativa y colaborativa, siempre listo para aportar ideas a mi equipo. |
| ![Integrante-Jarod-Cespedes](./assets/EmanuelChipana.png) | **Chipana Huarancca, Emanuel Wilfredo** | U202214074 | Decidí estudiar Ingeniería de Software motivado por mi pasión de unir el diseño visual con la lógica de programación para crear soluciones útiles. Tengo sólidos conocimientos en C++, Python y JavaScript. Además, destaco en el diseño de interfaces y experiencia de usuario (UI/UX), con un fuerte dominio de Figma para la creación de prototipos interactivos y wireframes. Disfruto conceptualizar ideas y asegurar una navegación fluida antes de pasar al código. Me considero proactivo y colaborativo; habilidades que aportaré para que nuestro sistema sea tan intuitivo como funcional. |
| ![Integrante-Jareth-Vidal](./assets/JarethVidal.jpeg) | **Vidal Malaga, Jareth Beycker** | U202316878 |Decidí estudiar Ingeniería de Software para transformar desafíos en soluciones digitales, combinando mi base técnica en C++, Python y JavaScript con una mentalidad analítica. Como estudiante de sexto ciclo, destaco por mi adaptabilidad y responsabilidad, valores que refuerzo a través de la disciplina del deporte y un aprendizaje constante. Mi enfoque se centra en trabajar de manera colaborativa para crear software que no solo sea funcional, sino también eficiente y orientado a resultados. |

## 1.2. Solution Profile
### 1.2.1 Antecedentes y problemática

#### Contexto del mercado y oportunidad

En el panorama económico actual, la industria de la panificación en el Perú se ha visto sometida a una presión financiera sin precedentes debido a la volatilidad en el precio de los commodities, especialmente el trigo, que representa hasta el 40% de los costos de producción de una panadería tradicional (BCRP, 2024). Según el Ministerio de la Producción (2024), el sector manufactura, donde se incluye la panificación, presenta una brecha tecnológica significativa, donde más del 60% de las microempresas operan sin herramientas digitales de gestión, dependiendo de procesos manuales y conocimientos empíricos. Esta falta de control técnico deriva en ineficiencias operativas que elevan la merma de insumos. De acuerdo con el INEI (2024). Esta falta de control técnico no solo incrementa la merma operativa hasta en un 15% por errores de producción, sino que limita la capacidad de respuesta de los dueños ante las fluctuaciones del mercado (Ministerio de la Producción, 2024). Es en este contexto de necesidad de eficiencia y optimización de recursos donde surge BrainNova, una propuesta tecnológica diseñada para cerrar la brecha digital en el sector panadero mediante el monitoreo en tiempo real y la gestión inteligente de datos.

A pesar de la importancia cultural y económica del pan en la dieta peruana, la sostenibilidad de las panaderías artesanales se ve amenazada por cuellos de botella que trascienden la simple preparación del producto. Para identificar las raíces de estas ineficiencias, se ha elaborado el siguiente diagrama de Ishikawa, el cual permite visualizar de manera sistémica cómo la carencia de herramientas tecnológicas afecta la maquinaria, los métodos y la rentabilidad final del negocio (Vásquez, 2024):

El análisis sistémico a través del diagrama de Ishikawa revela que la vulnerabilidad de las panaderías ante la crisis de costos (BCRP, 2024) se debe principalmente a la ausencia de un ecosistema digital que conecte la maquinaria con la gestión de materiales. Mientras los métodos sigan siendo manuales y el monitoreo de la maquinaria sea visual, la merma del 15% seguirá erosionando los márgenes de ganancia. BrainNova interviene precisamente en los ejes de Maquinaria y Medida, transformando datos en tiempo real en herramientas de ahorro directo para el microempresario panadero.

---

#### Who — ¿Quiénes son los involucrados?

Los principales involucrados son los propietarios y administradores de panaderías MYPE que buscan optimizar sus operaciones, controlar costos y sostener el crecimiento del negocio. Este grupo toma decisiones estratégicas relacionadas con producción, compras, mantenimiento, personal y apertura de nuevas sedes.

También forman parte del entorno del problema los encargados de producción, operarios y responsables de tienda, quienes necesitan información clara y oportuna para controlar hornos, cámaras frigoríficas, insumos, tiempos de preparación y estado de los equipos. Su desempeño impacta directamente en la calidad del producto final y en la eficiencia del negocio.

---

#### What — ¿Qué se necesita?

Se necesita una solución tecnológica integrada que centralice la gestión de producción, el monitoreo de maquinaria, el control de condiciones operativas y la supervisión de múltiples sedes. Esta solución debe permitir que los responsables del negocio accedan a información en tiempo real sobre variables críticas como temperatura, humedad, estado de hornos, cámaras frigoríficas, alertas de fallas y avance de la producción.

Desde una perspectiva de negocio, la solución debe contribuir a mejorar la eficiencia operativa, reducir pérdidas por fallas o desperdicio de insumos, aumentar la trazabilidad de los procesos y facilitar decisiones gerenciales basadas en datos.

---

#### Where — ¿Dónde ocurre el problema?

El problema se presenta principalmente en panaderías ubicadas en zonas urbanas y comerciales, donde existe una alta demanda diaria de productos panificados y una necesidad constante de producción eficiente. También se intensifica en panaderías que operan más de una sede, ya que la supervisión descentralizada exige mayor coordinación, control y visibilidad operativa.

---

#### When — ¿Cuándo surge esta necesidad?

La necesidad surge cuando la panadería incrementa su volumen de producción, amplía su cartera de productos o abre nuevas sedes. En esta etapa, los métodos manuales dejan de ser suficientes porque el negocio requiere mayor control, estandarización de procesos y monitoreo continuo.

También aparece en situaciones críticas, como fallas de hornos, pérdida de refrigeración, inconsistencias en la cocción, retrasos en la producción o desperdicio de insumos. Estos eventos afectan directamente la rentabilidad y la experiencia del cliente.

---

#### Why — ¿Por qué existe esta necesidad?

Esta necesidad existe porque las panaderías dependen de procesos productivos sensibles al tiempo, la temperatura, la humedad y el correcto funcionamiento de sus equipos. Cuando estas variables no se monitorean de manera constante, se incrementa el riesgo de errores operativos, productos defectuosos, pérdida de insumos y baja productividad.

Además, la falta de integración entre producción, inventario, mantenimiento y supervisión impide tener una visión completa del negocio. Esto limita la capacidad del propietario o administrador para identificar cuellos de botella, anticipar fallas, controlar costos y tomar decisiones estratégicas.

---

#### How — ¿Cómo se manifiesta el problema?

El problema se manifiesta a través de procesos manuales, comunicación informal entre trabajadores, registros incompletos y falta de alertas tempranas. Por ejemplo, el administrador puede no detectar a tiempo que un horno está operando fuera del rango adecuado de temperatura o que una cámara frigorífica presenta una falla que compromete los insumos.

También se evidencia cuando el negocio tiene varias sedes y no cuenta con una plataforma centralizada para supervisar la producción de cada local. Esto genera pérdida de control, duplicidad de tareas, baja trazabilidad y dificultad para mantener estándares uniformes de calidad.

---

#### How Much — ¿Qué magnitud tiene el problema?

La magnitud del problema es alta porque impacta directamente en indicadores clave del negocio, como costos operativos, desperdicio de insumos, productividad del personal, calidad del producto, continuidad operativa y rentabilidad.

Aunque la magnitud exacta debe validarse mediante entrevistas y pruebas con usuarios, se identifican como métricas críticas: reducción de mermas, disminución de fallas no detectadas, mejora en tiempos de producción, reducción de productos defectuosos, aumento de la visibilidad operativa y mejora en la capacidad de supervisar múltiples sedes.

---

### Descripción consolidada de la problemática
Las panaderías MYPE en el Perú enfrentan dificultades para gestionar sus operaciones de manera eficiente, ya que dependen de procesos manuales y herramientas no integradas, lo que limita el control sobre la producción y el monitoreo en tiempo real de los equipos. Esto afecta la calidad del producto, aumenta los costos operativos y dificulta la expansión, especialmente cuando se gestionan múltiples sedes.

La solución **BakeryManager** busca centralizar la gestión operativa mediante sensores IoT y un dashboard en tiempo real, optimizando la eficiencia, reduciendo desperdicios y mejorando la calidad del producto. Esta plataforma permitirá la gestión eficiente de múltiples sedes, garantizando un crecimiento escalable y sostenible para las panaderías.

## 1.2.2. Lean UX Process
### 1.2.2.1. Lean UX Problem Statements

Los dueños y trabajadores de panaderías que gestionan operaciones en una o varias sedes enfrentan dificultades para supervisar en tiempo real la producción y el estado de los equipos, debido al uso de procesos manuales y sistemas no digitalizados. Esto genera falta de visibilidad operativa, detección tardía de incidentes como fallas en hornos, fugas de gas o problemas de refrigeración, y dificultades en la coordinación del personal, lo que afecta la eficiencia, la
seguridad y la continuidad de la producción diaria.
Las soluciones actuales no integran tecnología IoT junto con una aplicación web centralizada que permita monitorear en tiempo real los equipos críticos ni generar alertas automáticas basadas en datos de sensores, lo que limita la
capacidad de prevención y respuesta ante riesgos operativos.
Nuestra solución abordará este problema mediante BakeryManager, una aplicación web con tecnología IoT que conectará sensores instalados en equipos como hornos, cámaras de refrigeración y áreas de producción para recopilar datos en tiempo real (temperatura, estado de máquinas, gas y humo). Esta información será visualizada en un
dashboard web centralizado, permitiendo a los usuarios supervisar múltiples sedes desde cualquier dispositivo, recibir alertas automáticas ante anomalías y optimizar la gestión operativa. Inicialmente, el enfoque estará en panaderías
multisede en ciudades como Lima Metropolitana.


### 1.2.2.2. Lean UX Assumptions

#### **Sobre los usuarios: propietarios, administradores y encargados de producción**

- **Asumimos** que los propietarios y administradores de panaderías MYPE buscan optimizar la eficiencia operativa y mantener altos estándares de calidad en sus productos, por lo que priorizan el monitoreo de condiciones críticas como temperatura, humedad, conservación de masas y estado de los equipos.  
  **Métrica de éxito:** Reducir las fallas operativas en un 30% mediante la integración de un sistema de monitoreo en tiempo real.  
  **Definition of Done:** El sistema asegura que el 95% de las condiciones operativas sean monitoreadas en tiempo real, con alertas automáticas sobre variaciones críticas.  
  **Objetivos del grupo objetivo:** Minimizar el riesgo de productos defectuosos, mejorar la eficiencia operativa y garantizar la calidad del producto.  
  **Características de la solución:** Integración de sensores IoT para monitorear temperatura, humedad y estado de los equipos, además de alertas automáticas en caso de anomalías.

- **Asumimos** que los encargados de producción necesitan información en tiempo real sobre el estado de los equipos y las condiciones operativas para tomar decisiones rápidas y garantizar la calidad del producto.  
  **Métrica de éxito:** Reducir el tiempo de respuesta ante alertas críticas en un 30%, pasando de 15 a 10 minutos mediante el uso de alertas automáticas.  
  **Definition of Done:** El sistema permite la recepción de alertas en tiempo real y facilita que los encargados tomen decisiones correctivas de manera oportuna.  
  **Objetivos del grupo objetivo:** Minimizar el impacto de variaciones operativas en la calidad del producto y optimizar los tiempos de producción.  
  **Características de la solución:** Dashboard centralizado para visualización en tiempo real, accesible para los encargados de producción.

- **Asumimos** que los usuarios valoran soluciones fáciles de usar debido a la carga operativa diaria, por lo que la interfaz debe ser intuitiva y sencilla de implementar.  
  **Métrica de éxito:** El 85% de los usuarios deben ser capaces de utilizar la solución de manera efectiva con menos de 30 minutos de capacitación inicial.  
  **Definition of Done:** La solución se considera implementada cuando al menos el 85% de los usuarios activos completan tareas básicas sin asistencia adicional.  
  **Objetivos del grupo objetivo:** Mejorar la eficiencia operativa diaria sin añadir complejidad al trabajo del personal.  
  **Características de la solución:** Interfaz intuitiva, diseño simple y accesibilidad desde dispositivos móviles y computadoras.

- **Asumimos** que los usuarios consideran importante recibir alertas inmediatas ante cualquier variación crítica en las condiciones operativas para mitigar riesgos y prevenir pérdidas.  
  **Métrica de éxito:** El 95% de las alertas deben ser gestionadas de forma efectiva dentro del tiempo estipulado.  
  **Definition of Done:** El sistema estará completo cuando el 95% de las alertas generen una respuesta de acción dentro de un tiempo máximo de 30 minutos desde su emisión.  
  **Objetivos del grupo objetivo:** Minimizar el riesgo de deterioro de masas, pasteles, insumos o productos terminados mediante la rápida identificación de problemas.  
  **Características de la solución:** Sistema de alertas automáticas basado en condiciones predefinidas, con opción de personalización de umbrales.

---

#### **Sobre las panaderías y sus operaciones**

- **Asumimos** que muchas panaderías MYPE gestionan sus operaciones con procesos manuales o sistemas no integrados, lo que dificulta el control y la trazabilidad de la producción.  
  **Métrica de éxito:** Implementar el sistema en al menos el 60% de las panaderías MYPE objetivo dentro de los primeros 12 meses.  
  **Definition of Done:** El sistema se considera implementado cuando el 60% de las panaderías objetivo gestionan sus operaciones con una plataforma digital centralizada.  
  **Objetivos del grupo objetivo:** Mejorar la trazabilidad de la producción y optimizar el control operativo del negocio.  
  **Características de la solución:** Plataforma centralizada para monitorear producción, equipos, condiciones críticas y datos históricos.

- **Asumimos** que las panaderías carecen de sistemas automatizados de monitoreo continuo de condiciones operativas.  
  **Métrica de éxito:** Automatizar el monitoreo en tiempo real en el 80% de las panaderías usuarias durante los primeros 6 meses de implementación.  
  **Definition of Done:** El sistema se considera completamente implementado cuando el 80% de las panaderías usuarias tienen conectados sus equipos críticos a la plataforma de monitoreo en tiempo real.  
  **Objetivos del grupo objetivo:** Mejorar la eficiencia operativa, reducir riesgos de fallas y garantizar la calidad del producto.  
  **Características de la solución:** Sensores IoT integrados para monitoreo continuo de hornos, cámaras frigoríficas, conservadoras de masa y cajas de fermentación.

- **Asumimos** que las panaderías necesitan mantener estándares de calidad e inocuidad en la producción de alimentos para reducir reclamos, pérdidas y riesgos operativos.  
  **Métrica de éxito:** Reducir en un 25% los incidentes asociados a productos defectuosos durante los primeros 6 meses de uso.  
  **Definition of Done:** El sistema se considera exitoso cuando permite registrar, monitorear y alertar sobre condiciones críticas que puedan afectar la calidad de panes, masas, pasteles e insumos refrigerados.  
  **Objetivos del grupo objetivo:** Garantizar productos más consistentes, reducir reclamos y mantener estándares adecuados de calidad.  
  **Características de la solución:** Reportes automáticos de condiciones operativas, historial de eventos y alertas por desviaciones en temperatura, humedad, gas, humo o estado de equipos.

---

#### **Sobre comportamiento y riesgos**

- **Asumimos** que la falta de monitoreo en tiempo real incrementa el riesgo de productos defectuosos, desperdicio de insumos y fallas operativas no detectadas.  
  **Métrica de éxito:** Reducir el riesgo de productos defectuosos en un 30% mediante monitoreo en tiempo real y alertas preventivas.  
  **Definition of Done:** El sistema se considerará exitoso cuando el 90% de los incidentes operativos registrados sean detectados antes de afectar la producción final.  
  **Objetivos del grupo objetivo:** Prevenir pérdidas económicas, proteger la calidad del producto y mejorar la continuidad operativa.  
  **Características de la solución:** Sistema de monitoreo en tiempo real con alertas automáticas que permitan tomar acciones correctivas antes de que los productos sean afectados.

- **Asumimos** que la falta de supervisión centralizada dificulta la gestión de múltiples sedes y reduce la capacidad de respuesta de los administradores.  
  **Métrica de éxito:** Lograr que el 90% de las sedes conectadas puedan ser supervisadas desde un dashboard centralizado.  
  **Definition of Done:** El sistema se considera completo cuando los administradores pueden visualizar el estado operativo de cada sede desde una sola plataforma.  
  **Objetivos del grupo objetivo:** Facilitar la supervisión remota, mejorar la coordinación entre sedes y tomar decisiones basadas en datos.  
  **Características de la solución:** Dashboard multisede con indicadores de producción, estado de equipos, alertas activas e historial de incidentes.

---

#### **Sobre tecnología y datos**

- **Asumimos** que las panaderías están dispuestas a implementar sensores IoT si estos mejoran el control de condiciones operativas y reducen riesgos en la producción.  
  **Métrica de éxito:** Implementar sensores IoT en el 80% de los equipos críticos definidos durante el primer año.  
  **Definition of Done:** El sistema se considera completo cuando el 80% de los equipos críticos seleccionados cuentan con sensores conectados a la plataforma.  
  **Objetivos del grupo objetivo:** Aumentar la precisión del monitoreo y mejorar la seguridad del proceso productivo.  
  **Características de la solución:** Sensores IoT para recolección de datos en tiempo real, integrados a una plataforma web accesible.

- **Asumimos** que existe disponibilidad de conexión a internet en la mayoría de panaderías urbanas objetivo, lo que facilita la implementación de una solución basada en la nube.  
  **Métrica de éxito:** El 95% de las panaderías objetivo deben contar con conexión a internet suficiente para sincronizar datos operativos en tiempo real.  
  **Definition of Done:** El sistema se considera implementado cuando el 95% de las panaderías conectadas pueden enviar y visualizar datos desde la plataforma sin interrupciones críticas.  
  **Objetivos del grupo objetivo:** Facilitar el monitoreo remoto, centralizar información y mantener continuidad en la supervisión operativa.  
  **Características de la solución:** Plataforma web basada en la nube, acceso remoto, sincronización continua de datos y visualización desde diferentes dispositivos.

### 1.2.2.3. Lean UX Hypothesis Statements

**Hipótesis 1:**

Si implementamos un sistema de monitoreo en tiempo real que utilice sensores IoT para medir condiciones clave como la temperatura y la humedad de los hornos y las conservadoras de masa, entonces los encargados de producción podrán actuar rápidamente ante cualquier desviación de los parámetros ideales, evitando productos defectuosos y mejorando la eficiencia operativa.

- **Usuarios:** Encargados de producción, operarios.
- **User Outcome:** Mejorar la toma de decisiones en tiempo real, asegurando la calidad del producto y la eficiencia operativa.
- **Feature:** Plataforma web con sensores IoT integrados para monitoreo continuo y alertas automáticas sobre variaciones críticas.

---

**Hipótesis 2:**

Si los encargados de producción reciben alertas automáticas en tiempo real sobre variaciones en las condiciones operativas de los equipos, como hornos o cámaras de refrigeración, entonces podrán reducir el tiempo de respuesta ante incidencias críticas, optimizando los tiempos de producción y garantizando que la calidad del producto no se vea afectada.

- **Usuarios:** Encargados de producción, operarios.
- **User Outcome:** Minimizar el impacto de variaciones operativas en la calidad del producto y optimizar los tiempos de producción.
- **Feature:** Sistema de alertas automáticas con un dashboard accesible para monitoreo en tiempo real.

---

**Hipótesis 3:**

Si implementamos una plataforma intuitiva y fácil de usar que permita a los usuarios acceder a información operativa clave con mínima capacitación, entonces la adopción de la solución será rápida, mejorando la eficiencia operativa sin añadir complejidad al trabajo diario del personal.

- **Usuarios:** Propietarios de panaderías, administradores, operarios.
- **User Outcome:** Mejorar la eficiencia operativa diaria sin aumentar la carga operativa ni la complejidad.
- **Feature:** Interfaz de usuario intuitiva, diseño simple, fácil de usar con menos de 30 minutos de capacitación inicial.

---

**Hipótesis 4:**

Si se integra un sistema centralizado para monitorear la producción y el estado de los equipos en tiempo real a través de múltiples sedes, entonces los administradores podrán gestionar la operación de varias ubicaciones desde una sola plataforma, lo que optimizará los recursos, reducirá los costos y mejorará la eficiencia general de las panaderías.

- **Usuarios:** Propietarios de panaderías, administradores, responsables de operaciones multisede.
- **User Outcome:** Mejorar la gestión de recursos y la eficiencia operativa en panaderías con múltiples sedes.
- **Feature:** Plataforma centralizada para monitoreo en tiempo real de las condiciones operativas de múltiples sedes.

### 1.2.2.4 Lean UX Canvas
![Lean UX Canvas](./assets/lean-ux-canva.jpg)

## 1.3. Segmentos objetivo

En el presente proyecto se identifican dos segmentos principales de usuarios, directamente vinculados con el dominio del problema: los propietarios y administradores de panaderías en proceso de crecimiento, y el personal operativo encargado de la ejecución diaria de las actividades del negocio. A continuación, se describen ambos perfiles.

---

### Propietarios y Administradores de Panaderías

Este segmento corresponde a personas naturales o jurídicas responsables de la gestión integral de panaderías y negocios afines, como pastelerías y minimarkets, quienes buscan optimizar sus operaciones y expandir sus actividades mediante la apertura de nuevas sedes.

#### Características demográficas

- **Ubicación:** Zonas urbanas y comerciales con alta demanda de productos de consumo diario.
- **Edad promedio:** Entre 30 y 55 años.
- **Nivel socioeconómico:** Medio.
- **Tipo de negocio:** Micro y pequeñas empresas, en muchos casos de carácter familiar.

#### Datos relevantes

- El sector panadero en el Perú está conformado por miles de unidades productivas a nivel nacional, en su mayoría micro y pequeñas empresas, lo que evidencia su alta representatividad dentro de la economía.
- La industria panadera ha registrado pérdidas económicas significativas, lo que pone en evidencia deficiencias en la gestión operativa, el control de recursos y la toma de decisiones dentro del sector.
- Durante campañas estacionales, como la Navidad, se proyecta la producción de millones de unidades de productos, lo que evidencia un incremento significativo en la demanda y en la carga operativa, exigiendo mayor capacidad de planificación y control.

#### Necesidades clave

- Centralización de la información operativa, incluyendo ventas, inventarios y producción, en una única plataforma.
- Monitoreo en tiempo real del estado de las sedes y maquinaria mediante tecnologías IoT.
- Control eficiente del flujo de ventas y gestión financiera básica.
- Supervisión y administración de múltiples locales de manera integrada.
- Reducción de pérdidas operativas a través de una gestión optimizada de recursos.

---

### Personal Operativo

Este segmento está conformado por los trabajadores responsables de la ejecución de las actividades productivas y el monitoreo básico de las condiciones operativas del negocio. Son usuarios clave del sistema, ya que interactúan directamente con Bakery Manager durante la jornada laboral.

#### Características demográficas

- **Edad:** Entre 20 y 45 años.
- **Nivel educativo:** Secundaria completa o formación técnica.
- **Ocupación:** Panaderos, asistentes de producción y encargados de turno.
- **Nivel de experiencia:** Variable, con predominio de aprendizaje práctico en el entorno laboral.
- **Nivel tecnológico:** Básico a intermedio.

#### Datos relevantes

- En muchas panaderías, los procesos de producción se gestionan de forma manual, lo que incrementa errores en tiempos de horneado, control de lotes y uso de insumos.
- La supervisión de condiciones críticas (temperatura, humedad, estado de equipos) suele ser limitada o no sistematizada.
- La detección de incidentes depende frecuentemente de la observación humana, lo que retrasa la reacción ante fallas o riesgos.
- En periodos de alta demanda, la presión operativa incrementa la probabilidad de errores y reduce la capacidad de respuesta ante incidencias.

#### Necesidades clave

- Monitoreo en tiempo real de variables críticas como temperatura, humedad y estado de maquinaria.
- Recepción de alertas inmediatas ante condiciones anómalas o posibles incidentes (por ejemplo, sobrecalentamiento o riesgo de incendio).
- Interfaces simples que permitan interpretar rápidamente la información del sistema.
- Reducción de la dependencia de la supervisión manual mediante automatización basada en sensores IoT.
- Apoyo en la toma de decisiones operativas durante la producción (ajustes, pausas, revisión de equipos).
- Mejora en la coordinación con administradores ante incidentes, sin necesidad de reportes manuales.  
