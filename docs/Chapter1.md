# Capítulo I: Introducción

## 1.1. Startup Profile

### 1.1.1. Descripción de la Startup

Nexum Devs es una startup tecnológica enfocada en el desarrollo de soluciones para el turismo de aventura en el Perú, orientada a mejorar la seguridad, trazabilidad y gestión operativa en entornos de baja conectividad. Surge para cubrir la falta de sistemas de alerta temprana que permitan detectar oportunamente anomalías en turistas que recorren zonas remotas sin cobertura celular.

Su producto principal, VitalTrek, es una plataforma web que centraliza la gestión de tours, permitiendo a las agencias supervisar la ubicación, estado y progreso de sus grupos mediante dashboards y alertas ante anomalías. A su vez, los turistas acceden a herramientas de navegación offline, registro de su experiencia y visualización de información contextual del recorrido. El enfoque del producto está en la operación y seguridad durante el tour, no en la reserva ni en la difusión abierta de reseñas de rutas: las notas de ruta (puntos críticos, condiciones del terreno) son cargadas por la propia agencia/guía que opera esa ruta, no por cualquier usuario.

A nivel técnico, VitalTrek integra un ecosistema IoT con dispositivos wearables y checkpoints Bluetooth que capturan datos de geolocalización y signos vitales. Estos se sincronizan de forma asincrónica cada vez que el turista pasa por un punto de control, asegurando operatividad incluso sin conexión continua, lo que permite un sistema de alertas tempranas escalable, resiliente y orientado a la prevención de riesgos.

### 1.1.2. Perfiles de integrantes del equipo

| Foto                                                        | Integrante                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
|-------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <br>![Foto](../assets/images/members/milenko_foto.jpeg)<br> | **Cayanchi Avila, Milenko Rubén**<br><br>Código de Estudiante: U202312566<br>Estudiante de Ingeniería de Software, enfocado en el desarrollo de soluciones tecnológicas innovadoras para la mejora de la calidad de vida. Poseo conocimientos básicos en Python y conocimientos básicos/intermedios en C++. Mi objetivo es adquirir conocimientos avanzados en inteligencia artificial y desarrollo de aplicaciones de salud, con el fin de mejorar mis habilidades y contribuir en el campo de la salud tecnológica.                                                                                                                                                                                        |
| <br>![Foto](../assets/images/members/jorge_foto.jpeg)<br>   | **León Naupari, Jorge Mateo**<br><br>Código de Estudiante: U202422549<br>Soy Jorge Mateo León Naupari, tengo 19 años y soy estudiante de la carrera de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas (UPC). Actualmente me encuentro cursando el cuarto ciclo de la carrera. Tengo conocimientos en el lenguaje de programación C++ y un gran interés por seguir desarrollando mis habilidades en el ámbito tecnológico. Mi objetivo es aplicar mis conocimientos en proyectos que me permitan crecer profesionalmente, aportar soluciones innovadoras y adquirir experiencia en el desarrollo de software.                                                                         |
| <br>![Foto](../assets/images/members/Ariel_foto.jpg)<br>    | **Mendoza Blanco, Ariel Roberto**<br><br>Código de Estudiante: U202419667<br>Hola a todos, soy Ariel Mendoza, estudiante de Ingeniería de Software. En el ámbito técnico, me especializo en el desarrollo backend, diseño de bases de datos y arquitectura de sistemas. Dentro del proyecto VitalTrek, mi rol está enfocado en la integración de datos telemétricos y la lógica de negocio, asegurando que la sincronización de checkpoints y la detección de alertas de signos vitales funcionen de forma consistente. Mi objetivo es construir una solución técnica sólida que convierta datos de campo en respuestas operativas inmediatas para la seguridad del turista.                                 |
| <br>![Foto](../assets/images/members/Miler_foto.jpeg)<br>   | **Rodriguez Rojas, Miler Alexander**<br><br>Código de Estudiante: U20241A827<br><br>Soy estudiante de Ingeniería de Software y actualmente curso el sexto ciclo. Cuento con conocimientos en C++, SQL Server Management, HTML, CSS, JavaScript, Python y TypeScript a nivel básico, principalmente orientados al desarrollo de software y aplicaciones web. Me encuentro en un proceso de desarrollo y aprendizaje continuo, buscando fortalecer mis conocimientos técnicos, adquirir experiencia y crecer profesionalmente. Mi objetivo es aplicar lo aprendido en proyectos que me permitan aportar soluciones innovadoras, trabajar en equipo y afrontar nuevos desafíos dentro del ámbito tecnológico.   |
|                                                             | **[Apellidos, Nombres]**<br><br>Código de Estudiante: [código]<br><br>[Descripción personal — completar]                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |

---

## 1.2. Solution Profile

### 1.2.1. Antecedentes y problemática

En los últimos años, el turismo de aventura en el Perú ha presentado un crecimiento constante debido al interés de turistas nacionales e internacionales por actividades como trekking, montañismo y exploración en zonas naturales. El Ministerio de Comercio Exterior y Turismo ([MINCETUR](https://www.gob.pe/institucion/mincetur/noticias/563063-se-aprueban-veintidos-modalidades-de-turismo-de-aventura)) reconoce al turismo de aventura como un segmento importante dentro de la actividad turística nacional y ha aprobado diversas modalidades para fortalecer su desarrollo y regulación.

Muchas de estas actividades se desarrollan en áreas alejadas de centros urbanos, donde la cobertura de red móvil es limitada o inexistente debido a las condiciones geográficas del territorio peruano. Según reportes del Organismo Supervisor de Inversión Privada en Telecomunicaciones ([OSIPTEL](https://www.osiptel.gob.pe/portal-del-usuario/noticias/checa-tu-senal-asi-puedes-verificar-la-cobertura-movil-en-tu-distrito/)), todavía existen zonas del país con limitaciones de cobertura móvil y variaciones en la calidad del servicio, especialmente en áreas rurales y de difícil acceso.

Actualmente, las agencias de turismo y los guías dependen principalmente de teléfonos móviles y aplicaciones convencionales de comunicación y geolocalización para coordinar recorridos y mantener contacto con los grupos. Sin embargo, estas herramientas presentan limitaciones en zonas sin señal, generando dificultades para el monitoreo continuo de los turistas y la atención oportuna ante situaciones de emergencia. Esta problemática evidencia la necesidad de implementar soluciones tecnológicas adaptadas al contexto geográfico y operativo del turismo de aventura en el país.

| Pregunta      | Formulación                   | Respuesta                                                                                                                                                                                                                                                                                                                                                                                                                  |
| ------------- | ----------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Who?**      | ¿Quiénes son los afectados?   | Las agencias de turismo de aventura, los guías turísticos y los turistas nacionales e internacionales que realizan expediciones en zonas remotas del Perú, donde la limitada cobertura móvil dificulta el monitoreo y la comunicación durante el recorrido.                                                                                                                                                                |
| **What?**     | ¿Cuál es el problema?         | La falta de un sistema de alertas tempranas basado en el monitoreo periódico de ubicación y signos vitales limita la capacidad de respuesta ante emergencias y reduce la seguridad de los turistas durante actividades de aventura en zonas sin cobertura de red.                                                                                                                                                          |
| **Where?**    | ¿Dónde ocurre?                | El problema se presenta en rutas de turismo de aventura ubicadas en zonas remotas del Perú, especialmente en circuitos de trekking de los Andes, selva alta y áreas naturales con geografía compleja y cobertura móvil limitada o inexistente.                                                                                                                                                                             |
| **When?**     | ¿Cuándo se hace más evidente? | Durante el desarrollo de las expediciones, principalmente en situaciones de separación de grupos, cambios climáticos bruscos, recorridos de alta dificultad o ante emergencias médicas como fatiga extrema, deshidratación o mal de altura.                                                                                                                                                                                |
| **Why?**      | ¿Por qué ocurre?              | Debido a que las herramientas de comunicación y geolocalización utilizadas actualmente dependen de conexión móvil o internet para funcionar correctamente. En zonas remotas del Perú, la cobertura es limitada o inexistente, lo que genera pérdida de comunicación y dificultades para detectar oportunamente anomalías durante el recorrido.                                                                             |
| **How?**      | ¿Cómo se manifiesta?          | Se manifiesta mediante pérdida de comunicación entre integrantes del grupo, dificultades para ubicar turistas de forma oportuna, retrasos en la atención de emergencias y dependencia de aplicaciones móviles que dejan de funcionar correctamente en zonas sin cobertura.                                                                                                                                                 |
| **How Much?** | ¿Cuánta es la magnitud?       | El crecimiento sostenido del turismo de aventura en el Perú ha incrementado la cantidad de expediciones realizadas en zonas de difícil acceso. Sin embargo, gran parte de estas áreas presenta limitaciones de conectividad, lo que incrementa los riesgos de accidentes, extravíos y retrasos en la respuesta ante emergencias, afectando tanto la seguridad de los turistas como la capacidad operativa de las agencias. |

### 1.2.2. Lean UX Process

#### 1.2.2.1. Lean UX Problem Statements

#### 1.2.2.2. Lean UX Assumptions

#### 1.2.2.3. Lean UX Hypothesis Statements

#### 1.2.2.4. Lean UX Canvas

El **Lean UX Canvas** de VitalTrek sintetiza las decisiones estratégicas y de diseño del proyecto en un modelo visual iterativo. A continuación, se detallan los ocho recuadros estructurados para guiar el desarrollo del MVP:

| Recuadro del Canvas | Descripción y Contenido |
| :--- | :--- |
| **1. Business Problem**<br>*(Problema del Negocio)* | Las agencias de turismo de aventura (MYPEs) y guías en rutas de trekking aisladas (Cusco, Áncash, Arequipa, Puno) pierden total visibilidad operativa al ingresar a zonas sin cobertura celular, dependiendo de radios VHF/UHF sin trazabilidad automatizada o reportes manuales que retrasan la atención de incidentes. |
| **2. Business Outcomes**<br>*(Resultados del Negocio)* | • **Reducción del 40%** en el tiempo promedio de detección de retrasos o anomalías.<br>• **95% de registros exitosos** en checkpoints configurados (pérdida de datos < 5%).<br>• **Reducción del 40%** en el tiempo promedio de gestión de incidencias.<br>• **Conversión del 25%** de agencias piloto a suscripciones anuales pagadas.<br>• **85% de percepción de seguridad** calificada como "Alta" o "Muy Alta" por turistas. |
| **3. Users**<br>*(Usuarios / Personas)* | • **Administrador / Operador B2B:** Configura rutas, checkpoints y monitorea la expedición en el dashboard.<br>• **Guía de Campo:** Recibe alertas en tiempo real y ejecuta acciones correctivas en el terreno.<br>• **Turista B2C:** Porta el wearable y consulta la información técnica de la ruta offline. |
| **4. User Outcomes & Benefits**<br>*(Resultados del Usuario)* | • **Agencias:** Control centralizado y reducción drástica de la incertidumbre operativa.<br>• **Guías:** Identificación rápida de turistas con descompensación física para priorizar asistencia.<br>• **Turistas:** Mayor tranquilidad en tramos aislados y autonomía de navegación offline. |
| **5. Solutions**<br>*(Soluciones propuestas)* | • Motor de sincronización asincrónica por checkpoints Bluetooth.<br>• Algoritmo de detección temprana de anomalías en signos vitales y retrasos.<br>• Dashboard web centralizado de operaciones e incidentes.<br>• Módulo de curaduría de notas técnicas de ruta (offline).<br>• Módulo de gestión de suscripciones SaaS integrado con MercadoPago. |
| **6. Hypotheses**<br>*(Hipótesis)* | • **H1 (Sync):** Creemos que con la sincronización por checkpoints Bluetooth lograremos registrar el 95% de pasadas en zonas sin señal.<br>• **H2 (Alertas):** Creemos que con el algoritmo por umbrales médicos reduriremos en 40% el tiempo de detección de anomalías.<br>• **H3 (Dashboard):** Creemos que con el dashboard centralizado reduriremos en 40% el tiempo de atención de reportes e incidencias.<br>• **H4 (Notas):** Creemos que con las notas de ruta offline alcanzaremos un 85% de percepción de seguridad alta en turistas.<br>• **H5 (MercadoPago):** Creemos que con el módulo de suscripciones integrado a MercadoPago convertiremos al 25% de agencias piloto a pago anual. |
| **7. What's the most important thing we need to learn first?**<br>*(Riesgos / Aprendizaje prioritario)* | • ¿La frecuencia de sincronización por ráfagas Bluetooth en checkpoints es suficiente para detectar una anomalía a tiempo?<br>• ¿Las reglas de alerta generan falsas alarmas que saturen la atención del guía durante la caminata? |
| **8. What's the least amount of work we can do to learn the next most important thing?**<br>*(Experimentos / MVP)* | • **Simulación de capa IoT y API RESTful:** Enviar eventos simulados a la API para medir la latencia y confiabilidad del motor de reglas sin requerir hardware físico.<br>• **Pruebas de usabilidad con prototipo en Figma:** Validar la comprensión del Dashboard con administradores de agencias MYPE en sesiones de 5 minutos. |

![Lean UX Canvas — VitalTrek](./assets/images/chapter-1/lean-ux-canvas.png)
*Figura 1.2.2.4. Representación visual del Lean UX Canvas para el ecosistema VitalTrek.*

# 1.3 Segmentos Objetivo

A partir del análisis del dominio del problema, la falta de sistemas de alertas tempranas basados en monitoreo periódico para turismo de aventura en zonas remotas del Perú, se han identificado dos segmentos objetivo claramente diferenciados a los que VitalTrek dirige su propuesta de valor. El primero corresponde a las agencias y operadores turísticos de aventura que requieren herramientas de gestión, supervisión y trazabilidad operativa de sus tours; el segundo corresponde a los turistas de aventura nacionales y extranjeros que demandan experiencias seguras, guiadas y enriquecidas en entornos naturales del país. A continuación se describen ambos segmentos junto con sus características demográficas y la información estadística que sustenta su relevancia.

*Segmento 1: Agencias y Operadores de Turismo de Aventura*

**Descripción**

Empresas formalmente constituidas, registradas en el Directorio Nacional de Prestadores de Servicios Turísticos del MINCETUR, dedicadas a la organización y operación de tours de aventura: trekking, montañismo, canotaje, ciclismo de montaña, escalada y actividades de ecoturismo. Su operación se concentra principalmente en regiones con alto potencial de turismo de aventura como Cusco, Áncash, Arequipa, Puno, Madre de Dios y San Martín, donde la conectividad celular es intermitente o inexistente. Estas agencias enfrentan limitaciones operativas para supervisar el estado y la ubicación de sus grupos durante los recorridos, así como para responder de forma oportuna ante anomalías o emergencias.

**Características demográficas y de negocio**

- Tipo de empresa: Micro y pequeñas empresas (MYPEs) en su mayoría, con entre 5 y 50 colaboradores entre guías, choferes y personal administrativo.
- Ubicación geográfica: Cusco, Áncash (Huaraz), Arequipa, Puno, Madre de Dios, Lima y San Martín.
- Antigüedad operativa: Mayoritariamente con más de 3 años en el mercado y registradas en DIRCETUR/GERCETUR.
- Capacidad operativa: Atienden grupos de entre 4 y 20 turistas por tour, con frecuencia diaria o semanal según temporada.
- Perfil tecnológico: Adopción digital baja a media, con uso predominante de WhatsApp y radios para comunicación, y escaso uso de plataformas integradas de gestión.

**Información estadística de sustento**

- Solo en Cusco, la Asociación de Agencias de Turismo del Cusco (AATC) representa a más de 190 agencias activas dedicadas a turismo de aventura, místico, ecológico y tradicional, lo que evidencia la concentración del mercado objetivo en regiones específicas.
- Según MINCETUR, en el 2025 se registraron 14.1 millones de visitas a sitios turísticos del país, un crecimiento del 33.2% frente al 2024, con una recuperación del 95.4% respecto al nivel prepandemia, lo que se traduce en una mayor demanda de servicios para los operadores.
- El 83% de los operadores turísticos del segmento aventura reportó incremento de ingresos en 2025, y un 46% indicó que estos crecieron por encima del 26% según el estudio anual de la Adventure Travel Trade Association (ATTA), lo que demuestra capacidad de inversión en herramientas tecnológicas.
- El sector turismo aportó aproximadamente el 2.9% del PBI nacional en 2025, según estimaciones del MINCETUR a partir de las Cuentas Satélite del Turismo, consolidando a las agencias como un mercado de alto valor económico.

*Segmento 2: Turistas de Aventura*

**Descripción**

Personas que viajan al Perú, ya sea desde el extranjero o desde otras regiones del país, motivadas por experiencias de naturaleza, deporte y exploración en entornos remotos. Buscan vivir recorridos como el Camino Inca, Salkantay, Choquequirao, Huayhuash, Colca o la Amazonía, contratando agencias formales que les brinden seguridad, organización y guías especializados. Demandan herramientas digitales que les permitan navegar offline, registrar su experiencia y acceder a información contextual del recorrido sin depender de conectividad continua.

**Características demográficas**

- Edad: El 49% de los viajeros de aventura a nivel mundial se ubica entre los 41 y 60 años; en Sudamérica esta franja sube al 54%, mientras que un 26% tiene menos de 40 años.
- Género: Predominio femenino, con 53% de mujeres frente a 46% de hombres realizando viajes de aventura, según ATTA 2024.
- Composición del grupo de viaje: El 36% viaja en pareja, 24% en grupo y 21% en familia. En Sudamérica, la familia (26%) supera a los grupos como segunda modalidad más popular.
- Procedencia: Mayoritariamente turistas extranjeros provenientes de Sudamérica (51.7%), Norteamérica (23.8%) y Europa (16.8%), complementados por turistas nacionales que viajan dentro del territorio peruano.
- Nivel socioeconómico: Medio-alto y alto, con capacidad de pagar paquetes turísticos completos y seguros de viaje con cobertura para deportes de riesgo.

**Información estadística de sustento**

- En el 2025, el Perú recibió 3.2 millones de turistas internacionales, un crecimiento del 29% frente al 2024, con proyecciones de alcanzar las cifras prepandemia de 4.4 millones en los próximos años.
- Se estima que el país alcanzará 43.5 millones de viajes por turismo interno al cierre de 2025, un 16.9% más que en 2024, ampliando significativamente la base potencial de turistas nacionales que demandan experiencias de aventura.
- El segmento global de turismo de aventura registró un crecimiento del 65% en número de viajeros atendidos respecto al 2019, y un 54% adicional respecto al 2022, consolidándose como uno de los nichos de mayor expansión a nivel mundial.
- El 51.5% de las visitas registradas en sitios turísticos peruanos en 2025 corresponde a turistas internacionales y el 48.5% a nacionales, lo que confirma que la propuesta de VitalTrek debe atender a ambos perfiles bajo experiencias multilingües y adaptadas culturalmente.
- Regiones clave para el turismo de aventura como Cusco e Ica ya están a solo 2.6% y 3.6% de alcanzar sus cifras prepandemia, evidenciando la consolidación de los destinos donde opera el segmento.
