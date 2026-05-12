# Capítulo I: Introducción
## 1.1. Startup Profile
### 1.1.1. Descripción de la Startup

Somos Brainova, un equipo de estudiantes de la Universidad Peruana de Ciencias Aplicadas comprometidos con el desarrollo de soluciones tecnológicas innovadoras para optimizar la gestión de negocios como panaderías, pastelerías y otros emprendimientos en crecimiento. Nuestra propuesta consiste en una plataforma web que permite mejorar la eficiencia operativa, automatizar procesos y facilitar la toma de decisiones mediante el uso de tecnología.

Para que el producto BakeryManager, una solución enfocada en negocios de panadería que integra el control de producción, monitoreo de maquinaria y supervisión de condiciones operativas mediante sensores IoT, permitiendo una gestión más eficiente, centralizada y en tiempo real de sus operaciones, especialmente en
entornos multisede.

**Misión:**  
Nuestra misión es desarrollar soluciones digitales que optimicen la gestión operativa de panaderías en crecimiento, mediante el monitoreo en tiempo real de sus procesos productivos y equipos a través de tecnología IoT. Buscamos mejorar la eficiencia, reducir pérdidas y facilitar la supervisión de múltiples sedes a través de una plataforma centralizada.

**Visión:**  
Nuestra visión es ser una solución tecnológica líder en la digitalización del sector panadero, destacando por integrar monitoreo inteligente mediante IoT y gestión operativa en una sola plataforma, contribuyendo al crecimiento sostenible y a la modernización de las panaderías MYPES.
## 1.1.2. Perfiles de integrantes del equipo

## 1.1.2.1 Integrantes del Equipo

| Foto                                                     | Nombre | Código | Descripción |
|----------------------------------------------------------|--------|--------|-------------|
| <img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/feature/Chapter1/Report/assets/LuisTufino.png" alt="Luis Tufiño" width="100%">                 | **Tufiño Argüelles Luis Angel** | U202216240 | Elegí la carrera de Ingeniería de Software motivado por mi interés en comprender cómo funcionan los programas. Durante la pandemia, comencé a modificar juegos sencillos, iniciando así mi camino en la programación. Tengo conocimientos en C++, Python y JavaScript, además de experiencia en desarrollo web con HTML y CSS y en la creación de bots usando Python. También desarrollé una aplicación web para el negocio familiar, aplicando conceptos de bases de datos y diseño UX/UI. Considero que mi creatividad y capacidad de trabajo en equipo aportan positivamente al desarrollo de este proyecto. |
| <img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/feature/Chapter1/Report/assets/ManuelMolina.jpg" alt="Manuel Molina" width="100%">        | **Molina Vásquez Manuel Alejandro** | U20221G231 | Escogí la carrera de Ingeniería de Software porque me interesa comprender el funcionamiento de diversos programas y los algoritmos utilizados en ellos. Tengo conocimientos en C#, C++, Python, HTML y CSS, además de experiencia en el desarrollo de aplicaciones web y manejo de bases de datos. Considero que una de mis principales fortalezas es mi capacidad de trabajo en equipo, lo cual contribuye al cumplimiento de los objetivos del proyecto. |
| <img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/feature/Chapter1/Report/assets/JarodCespedes.png" alt="Jarod Cespedes" width="100%"> | **Cespedes Pillco, Jarod Jack** | U202318588 | Elegí la carrera de Ingeniería de Software por el interés mío de entender cómo los videojuegos y programas en general funcionaban y cómo eran creados. Tengo experiencia con los lenguajes de programación C++, C#, Visual Basic, Python y Java, además tengo habilidad en el desarrollo de interfaces web con el lenguaje de tipado HTML y CSS. Considero que soy una persona creativa y colaborativa, siempre listo para aportar ideas a mi equipo. |
|<img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/feature/Chapter1/Report/assets/EmanuelChipana.png" alt="Emanuel Chipana" width="100%"> | **Chipana Huarancca, Emanuel Wilfredo** | U202214074 | Decidí estudiar Ingeniería de Software motivado por mi pasión de unir el diseño visual con la lógica de programación para crear soluciones útiles. Tengo sólidos conocimientos en C++, Python y JavaScript. Además, destaco en el diseño de interfaces y experiencia de usuario (UI/UX), con un fuerte dominio de Figma para la creación de prototipos interactivos y wireframes. Disfruto conceptualizar ideas y asegurar una navegación fluida antes de pasar al código. Me considero proactivo y colaborativo; habilidades que aportaré para que nuestro sistema sea tan intuitivo como funcional. |
| <img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/feature/Chapter1/Report/assets/JarethVidal.jpeg" alt="Jareth Vidal" width="100%"> | **Vidal Malaga, Jareth Beycker** | U202316878 |Decidí estudiar Ingeniería de Software para transformar desafíos en soluciones digitales, combinando mi base técnica en C++, Python y JavaScript con una mentalidad analítica. Como estudiante de sexto ciclo, destaco por mi adaptabilidad y responsabilidad, valores que refuerzo a través de la disciplina del deporte y un aprendizaje constante. Mi enfoque se centra en trabajar de manera colaborativa para crear software que no solo sea funcional, sino también eficiente y orientado a resultados. |

## 1.2. Solution Profile
### 1.2.1 Antecedentes y problemática

#### Contexto del mercado y oportunidad

En el mercado peruano, las micro y pequeñas empresas cumplen un rol estratégico dentro de la economía. Según el Ministerio de la Producción, al cierre del 2024 el Perú registró 2 346 592 empresas formales, de las cuales el 99,1 % correspondía a micro y pequeñas empresas, aportando el 20,2 % del PBI nacional. Además, las MYPE emplearon el 86,5 % del empleo total del sector privado, lo que evidencia su relevancia económica y social.

Dentro de este ecosistema, las panaderías representan negocios con alta rotación de productos, dependencia de procesos productivos diarios y necesidad constante de controlar calidad, tiempos, insumos y equipos. Sin embargo, muchas de estas empresas aún gestionan sus operaciones mediante procesos manuales, hojas de cálculo o sistemas aislados, lo que limita su capacidad para escalar de forma eficiente.

Actualmente, existe una oportunidad de mercado para soluciones digitales enfocadas en la transformación operativa de las MYPE. PRODUCE impulsa la línea “Mype Digital”, orientada a acompañar a las empresas en su proceso de digitalización mediante asesoría, servicios tecnológicos, capacitación y automatización de procesos productivos clave. Esto confirma que la digitalización ya no es solo una mejora tecnológica, sino una necesidad competitiva para que las pequeñas empresas sean más productivas, sostenibles y escalables.

No obstante, en el caso específico de las panaderías, muchas soluciones disponibles se concentran en funciones generales como ventas, caja, facturación o inventario básico. Estas herramientas no siempre resuelven el problema operativo central: la falta de visibilidad en tiempo real sobre la producción, el estado de la maquinaria y las condiciones críticas que afectan directamente la calidad del producto. Esta brecha representa una oportunidad para BakeryManager, una solución especializada que integra gestión operativa con sensores IoT para mejorar la supervisión, reducir riesgos y facilitar la toma de decisiones basada en datos.

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


### Descripción consolidada de la problemática
Las panaderías MYPE en el Perú enfrentan dificultades para gestionar sus operaciones de manera eficiente, ya que dependen de procesos manuales y herramientas no integradas, lo que limita el control sobre la producción y el monitoreo en tiempo real de los equipos. Esto afecta la calidad del producto, aumenta los costos operativos y dificulta la expansión, especialmente cuando se gestionan múltiples sedes.

La solución **BakeryManager** busca centralizar la gestión operativa mediante sensores IoT y un dashboard en tiempo real, optimizando la eficiencia, reduciendo desperdicios y mejorando la calidad del producto. Esta plataforma permitirá la gestión eficiente de múltiples sedes, garantizando un crecimiento escalable y sostenible para las panaderías.

## 1.2.2. Lean UX Process

### 1.2.2.1. Lean UX Problem Statements

**Problem Statement 1 — Propietarios y Administradores de Panaderías**

BakeryManager fue diseñado para lograr una gestión operativa centralizada y en tiempo real para los propietarios y administradores de panaderías que gestionan una o más sedes. Hemos observado que el producto no está satisfaciendo la necesidad de visibilidad continua sobre el estado de los equipos críticos y las condiciones de producción, lo cual está causando pérdidas económicas por fallas no detectadas en equipos, desperdicio de insumos y baja eficiencia operativa entre los propietarios y administradores de micro y pequeñas panaderías en zonas urbanas del Perú. ¿Cómo podríamos mejorar BakeryManager para que nuestros clientes sean más exitosos en base a una reducción del 30% en incidentes operativos no detectados y una mejora medible en la capacidad de supervisión de múltiples sedes?


**Problem Statement 2 — Personal Operativo**

BakeryManager fue diseñado para lograr el monitoreo automatizado y en tiempo real de las condiciones de producción y el estado de los equipos para el personal operativo que trabaja en las áreas de producción de panaderías. Hemos observado que el producto no está satisfaciendo la necesidad de detección inmediata de anomalías y alertas automáticas, lo cual está causando respuestas tardías ante incidentes críticos como el sobrecalentamiento de hornos o fallas en refrigeración, generando productos defectuosos y pérdidas en la producción entre panaderos, asistentes de producción y encargados de turno en panaderías MYPE. ¿Cómo podríamos mejorar BakeryManager para que nuestros clientes sean más exitosos en base a una reducción del tiempo promedio de respuesta ante incidentes de 15 a menos de 10 minutos y una disminución del 25% en productos defectuosos durante los primeros 6 meses de uso?


### 1.2.2.2. Lean UX Assumptions

#### Supuestos de Negocio

1. Creemos que nuestros clientes necesitan una plataforma centralizada que integre monitoreo IoT y gestión operativa para reducir pérdidas y mejorar la eficiencia en sus panaderías.
2. Creemos que el valor principal que un cliente quiere obtener de BakeryManager es la capacidad de detectar fallas en equipos críticos antes de que impacten la producción y generen pérdidas económicas.
3. Creemos que los clientes pueden adquirir BakeryManager mediante un modelo de suscripción mensual escalable según el número de sedes y sensores conectados.
4. Creemos que generaremos ingresos principalmente a través de planes de suscripción (Starter S/89, Business S/199, Enterprise S/399) y servicios de instalación de sensores IoT.
5. Creemos que nuestra mayor competencia son soluciones genéricas como Odoo y Loyverse POS que no cubren el monitoreo IoT especializado para panaderías MYPE.
6. Creemos que nuestra mayor ventaja competitiva es la combinación de monitoreo IoT en tiempo real con gestión operativa en una sola plataforma orientada específicamente a panaderías MYPE en crecimiento.
7. Creemos que si los propietarios no evidencian una reducción de pérdidas operativas durante los primeros 3 meses de uso, perderemos su confianza y no renovarán su suscripción.
8. Creemos que la mayoría de panaderías MYPE objetivo en Lima Metropolitana cuentan con conexión a internet suficiente para sincronizar datos operativos en tiempo real desde la plataforma.

#### Supuestos de Usuario

1. **¿Quién es el usuario?**
   Propietarios y administradores de panaderías MYPE con una o más sedes en Lima Metropolitana, y el personal operativo (panaderos, asistentes de producción y encargados de turno) que ejecuta las actividades productivas diarias.

2. **¿Dónde encaja nuestro producto en su trabajo o vida?**
   En la gestión diaria de la panadería: para los propietarios, en la supervisión remota del estado operativo de sus sedes; para el personal operativo, en el monitoreo de equipos y condiciones de producción durante la jornada laboral.

3. **¿Qué problemas resuelve nuestro producto?**
   La falta de visibilidad en tiempo real sobre el estado de equipos críticos, la detección tardía de fallas en hornos y cámaras frigoríficas, la dificultad para gestionar múltiples sedes sin presencia física constante y la ausencia de alertas automáticas ante condiciones anómalas.

4. **¿Cuándo y cómo se usa nuestro producto?**
   Durante toda la jornada operativa, tanto desde dispositivos móviles como desde computadoras, accediendo al dashboard centralizado, revisando el estado de los sensores y respondiendo a alertas automáticas en tiempo real.

5. **¿Qué características son indispensables?**
   Dashboard en tiempo real con estado de sensores IoT, alertas automáticas ante anomalías, historial de incidentes, gestión multisede y reportes de tendencias de producción.

6. **¿Cómo debe verse y comportarse el producto?**
   Con una interfaz simple, clara y con codificación visual por colores (verde/amarillo/rojo) que permita al personal interpretar el estado operativo en segundos, sin necesidad de capacitación técnica extensa, y accesible desde cualquier dispositivo con conexión a internet.


### 1.2.2.3. Lean UX Hypothesis Statements

**Hipótesis 1**

Creemos que lograremos **[una reducción significativa en las pérdidas económicas por fallas en equipos]**
Si **[los propietarios y administradores de panaderías]**
Alcanzan **[la capacidad de detectar anomalías en equipos críticos antes de que impacten la producción]**
Con **[el sistema de monitoreo IoT en tiempo real y alertas automáticas de BakeryManager]**

> Sabremos que esto es verdad cuando observemos una reducción del 30% en incidentes operativos no detectados durante los primeros 3 meses de uso.


**Hipótesis 2**

Creemos que lograremos **[una reducción del tiempo promedio de respuesta ante incidentes de 15 a menos de 10 minutos]**
Si **[el personal operativo, panaderos y encargados de turno]**
Alcanzan **[la capacidad de recibir alertas automáticas inmediatas cuando hornos o cámaras frigoríficas operan fuera de los parámetros normales]**
Con **[el módulo de monitoreo IoT en tiempo real y el sistema de notificaciones de BakeryManager]**

> Sabremos que esto es verdad cuando el tiempo promedio de respuesta ante incidentes se reduzca en un 33% durante el primer mes de uso activo.


**Hipótesis 3**

Creemos que lograremos **[una gestión multisede más eficiente y centralizada]**
Si **[los propietarios de panaderías con más de una sede]**
Alcanzan **[visibilidad completa del estado operativo de todas sus sedes desde una sola plataforma]**
Con **[el dashboard centralizado multisede de BakeryManager]**

> Sabremos que esto es verdad cuando el 90% de los usuarios con más de una sede accedan al dashboard al menos una vez al día durante el primer mes de uso.


**Hipótesis 4**

Creemos que lograremos **[una adopción rápida del producto con mínima capacitación]**
Si **[el personal operativo con nivel tecnológico básico a intermedio]**
Alcanzan **[la capacidad de interpretar el estado de los equipos y responder a alertas sin asistencia técnica adicional]**
Con **[la interfaz visual simplificada y la codificación por colores de BakeryManager]**

> Sabremos que esto es verdad cuando el 85% de los nuevos usuarios completen tareas básicas de monitoreo sin asistencia en su primera semana de uso, con menos de 30 minutos de capacitación inicial.


**Hipótesis 5**

Creemos que lograremos **[altas tasas de renovación de suscripción, 70% o más al finalizar el primer trimestre]**
Si **[los propietarios de panaderías]**
Alcanzan **[evidencia clara y medible de reducción en productos defectuosos y pérdidas operativas]**
Con **[el módulo de reportes históricos y analítica de tendencias de producción de BakeryManager]**

> Sabremos que esto es verdad cuando el 70% de los usuarios suscritos renueven su plan al finalizar el primer trimestre de uso.

### 1.2.2.4 Lean UX Canvas

<img src="https://raw.githubusercontent.com/1ASI0730-2610-20262-TBL-BrainNova/BakeryManager-report-repo/feature/Chapter1/Report/assets/lean-ux-canva.jpg" alt="Lean UX Canvas" width="100%">

Enlace al Lean UX Canvas en Miro : https://miro.com/app/board/uXjVGg5xObY=/

## 1.3. Segmentos objetivo

En el presente proyecto se identifican dos segmentos principales de usuarios, directamente vinculados con el dominio del problema: los propietarios y administradores de panaderías en proceso de crecimiento, y el personal operativo encargado de la ejecución diaria de las actividades del negocio. A continuación, se describen ambos perfiles.

---

### Propietarios y Administradores de Panaderías

Este segmento corresponde a personas naturales o jurídicas responsables de la gestión integral de panaderías y negocios afines, como pastelerías y minimarkets, quienes buscan optimizar sus operaciones y expandir sus actividades mediante la apertura de nuevas sedes.

#### Características demográficas

- **Ubicación:** Zonas urbanas y comerciales con alta demanda de productos de consumo diario.
- **Edad promedio:** Entre 30 y 55 años.
- **Nivel socioeconómico:** Medio.
- **Tipo de negocio:** Micro y pequeñas empresas, en muchos casos de carácter familiar..

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
