
# 1 Telefónica como organización del sector de las telecomunicaciones
[Telefónica](https://www.telefonica.com/es/nosotros/) es una de las principales compañias multinacionales del sector de telecomunicaciones a nivel mundial. Fundada en 1924 en España. Actualmente opera por Europa y Latinoamérica, ofreciendo servicios de comunicaciones fijas y móviles, acceso a internet de banda ancha, servicios de datos, soluciones digitales. Contaba con aproximadamente 24.000 trabajadores en Noviembre de 2025  aunque por el último ERE se ha visto reducido a 22.000 en Marzo de 2026.

En el ámbito empresarial, no solo proporciona infraestructura de telecomunicaciones, sino que también desarrolla soluciones avanzadas en áreas como la transformación digital, ciberseguridad, cloud computing y servicios de gestión de redes. Su actividad se apoya en una infraestructura tecnológica compleja y en la gestión de un elevado volumen de procesos operativos diarios.

## 1.1 Contexto organizativo del proyecto
Dentro de la estructura organizativa de Telefónica, la compañía distingue entre Planta Interna y Planta Externa.

+ **Planta Interna**: orientada principalmente a la gestión técnica y administrativa de servicios dentro de infraestructuras propias.

+ **Planta Externa**: responsable del despliegue, mantenimiento, modificación y supervisión de la red de telecomunicaciones en campo.

El Trabajo de Fin de Grado se enmarca dentro del área de Planta Externa, en específico en el departamento encargado de la gestión de variaciones de infraestructura.

Este departamento gestiona solicitudes relacionadas con modificaciones en instalaciones existentes, afectaciones sobre la red, expedientes técnicos asociados a proyectos urbanísticos, obras civiles u otras actuaciones que puedan impactar sobre la infraestructura de telecomunicaciones.

## 1.2 El buzón corporativo de variaciones
El canal de entrada de variaciones es uno de los principales buzones utlizados por telefónica que relaciona con terceros. Siendo la manera de comunicación formal entre Telefónica y: 
+ Empresas constructoras
+ Ingenierías
+ Administraciones públicas
+ Organismos oficiales
+ Particulares

El objetivo principal del buzón es la consulta del estado de actuaciones, expedientes y/o [petter](./glosario/petter.md). No obstante, en la práctica, se reciben consulta heterogéneas formado por consultas incompletas, peticiones duplicadas o pregunta por otros elementos ajenos a variaciones.

# 2. Situación actual y problemática
El elevado volumen de correos recibidos diariamente, junto con la diversidad de las consultas y la complejidad de las aplicaciones para poder responder agilmente, genera una carga significativa y un entorno de mejora mediante la automatización. 


## 2.1 Problemática identificada
Ante la entrada aproximada de 1.000 correos diarios y sumado a que todo el proceso es manual. Provoca que haya correos que no puedan ser atendidos. Sumado este constante retraso la reducción de recursos humanos ha incrementado la carga operativo, dificultando el mantenimiento a niveles óptimos.

## 2.2 Descripción del proceso actual de gestión del buzón
El proceso actual consiste en la llegada de un correo al buzón de correo del canal de entrada. Un técnico se encarga de leer el correo, analizar que se pide con el correo. Si hace referencia a un número, se tiene que meter a las aplicaciones correspondientes (Sgipe, Atlas, Petter, ...), recopilar la información y formar el correo para responder.

Si en el correo recibido no hace referencia a ningun número, en función de lo que se pida, el técnico deberá desviar hacia el sitio correcto para lo que se pida. 

## 2.3 Limitaciones del modelo actual
El modelo de solucionar este proceso tiene una serie de limitaciones estructurales:
+ Dependencia del factor humano, lo que impide la automatización parcial del proceso.
+ Escasa escalabilidad, dado que el volumen de correos puede incrementarse sin que exista una ampliación proporcional de recursos.
+ Repetitividad operativa, ya que un porcentaje significativo de las consultas se limita a la solicitud de estado de expediente.
+ Riesgo de error humano, especialmente en la transcripción o interpretación de datos
+ Incremento del tiempo medio de respuesta, derivado del volumen de entrada y de la necesidad de acceder manualmente a diferentes sistemas.

# 3. Estado del arte 
La automatización de procesos repetitivos se ha convertido en una práctica habitual para mejorar la eficiencia operativa. Las tecnologías de Robotic Process Automation (RPA) permiten replicar tareas humanas basadas en reglas, como la lectura de correos, extracción de datos o consulta de sistemas.

Plataformas como [Microsoft Power Automate](./glosario/powerAutomate.md) o UiPath permiten diseñar flujos automatizados capaces de integrarse con servicios de correo electrónico y bases de datos corporativas. Estas herramientas facilitan la creación de procesos desencadenados por eventos, como la recepción de un correo, que ejecutan acciones automáticas predefinidas.

Sin embargo, su implementación en entornos corporativos complejos requiere una adecuada integración con sistemas internos y una definición precisa de reglas de negocio.

## 3.2 Sistemas de gestión de tickets
Otra aproximación común es el uso de plataformas de gestión de incidencias o tickets donde los usuarios consultan ahí estandarizando la entrada.

En telefónica ya existen estos sistemas aunque el desarrollo de este sería costoso y tardío, dejando una situación imposible de gestionar ante el despido de empleados.

Estas plataformas suelen incluir funcionalidades básicas de respuesta automática y plantillas estandarizadas, así como capacidades de integración con sistemas empresariales.

No obstante, su adopción puede implicar costes elevados de implantación y adaptación, especialmente cuando se requiere una integración profunda con sistemas internos específicos o bases de datos propietarias.

## 3.3 Automatización basada en inteligencia artificial

En los últimos años, se ha avanzado significativamente en el uso de técnicas de procesamiento de lenguaje natural (NLP) para la clasificación automática de correos electrónicos y la detección de intención. Estos sistemas permiten identificar automáticamente el tipo de solicitud recibida y dirigirla al flujo de gestión correspondiente.

Asimismo, la incorporación de modelos de generación de texto posibilita la elaboración automática de respuestas coherentes en función de la información obtenida.

Sin embargo, la aplicación directa de soluciones basadas en inteligencia artificial en entornos corporativos con datos sensibles requiere garantizar aspectos como la seguridad, la confidencialidad y el cumplimiento normativo.

## 3.4 Limitaciones de las soluciones existentes en el contexto específico

Aunque las tecnologías descritas ofrecen soluciones consolidadas en el mercado, su aplicación directa en el contexto específico del departamento de variaciones presenta ciertas limitaciones:
+ Necesidad de integración con sistemas internos no estandarizados.
+ Restricciones de seguridad en el acceso a bases de datos corporativas.
+ Costes asociados a licencias y despliegue.
+ Requerimientos de personalización para adaptarse a procesos específicos.
+ Complejidad organizativa para implantar un sistema global en un entorno ya operativo.

En consecuencia, se plantea la conveniencia de desarrollar una solución adaptada al contexto particular del buzón de variaciones, capaz de integrarse con las herramientas existentes y automatizar aquellas tareas repetitivas susceptibles de ser sistematizadas.

## 4. Justificación de la propuesta

El análisis de la situación actual evidencia una oportunidad clara de mejora en la gestión del buzón corporativo de variaciones. El elevado volumen de correos electrónicos recibidos diariamente, unido a la naturaleza repetitiva de una parte significativa de las consultas, permite identificar tareas susceptibles de automatización sin comprometer la calidad del servicio.

Aunque existen soluciones consolidadas en el mercado orientadas a la automatización de procesos y a la gestión de incidencias, su implantación directa en el contexto específico del departamento presenta limitaciones técnicas y organizativas. Entre ellas destacan la necesidad de integración con sistemas internos, restricciones de seguridad en el acceso a bases de datos corporativas y la elevada personalización requerida para adaptarse a los procedimientos internos existentes.

En este escenario, el desarrollo de una solución específica orientada a la automatización del flujo de gestión del buzón permite:

+ Reducir la carga operativa asociada a tareas repetitivas.
+ Mejorar los tiempos de respuesta.
+ Minimizar el riesgo de error humano.
+ Optimizar el uso de los recursos disponibles.
+ Establecer una base escalable para futuras mejoras tecnológicas.

La propuesta planteada en este Trabajo de Fin de Grado consiste en el diseño e implementación de un sistema automatizado capaz de analizar el contenido de los correos electrónicos entrantes, extraer información relevante (como el número de petición o expediente), consultar automáticamente las bases de datos corporativas y generar respuestas estructuradas de forma autónoma cuando sea posible.

## 5. Hipótesis de trabajo
La hipótesis que sustenta el presente Trabajo de Fin de Grado es la siguiente:

*La implementación de un sistema automatizado de análisis y respuesta de correos electrónicos mejorará la eficiencia operativa del buzón de variaciones, reduciendo los tiempos de respuesta y la carga de trabajo manual del personal asignado, manteniendo la coherencia y fiabilidad de la información proporcionada.*

Esta hipótesis parte de la premisa de que una proporción significativa de las consultas recibidas presenta una estructura repetitiva y se basa en la solicitud de información que ya se encuentra disponible en sistemas internos, lo que hace viable su automatización mediante reglas predefinidas y consultas automatizadas a bases de datos.

# 6. Objetivos

## 6.1 Objetivo general
Diseñar e implementar un sistema automatizado capaz de gestionar parcialmente el buzón corporativo de variaciones mediante el análisis del contenido de los correos electrónicos, la consulta automatizada de bases de datos internas y la generación de respuestas estructuradas de forma autónoma.

## 6.2 Objetivos específicos
1. Analizar el proceso actual de gestión del buzón e identificar las tareas susceptibles de automatización.
2. Definir los requisitos funcionales y no funcionales del sistema propuesto.
3. Diseñar la arquitectura del sistema, contemplando la integración con el servicio de correo electrónico y las bases de datos corporativas.
4. Desarrollar un prototipo funcional (MVP) que permita automatizar las consultas relacionadas con el estado de expedientes o peticiones.
5. Validar el funcionamiento del sistema mediante pruebas con casos reales o simulados.
6. Evaluar el impacto potencial del sistema en términos de eficiencia operativa y reducción de carga manual.

# 7. Metodología

El desarrollo del presente proyecto se abordará siguiendo un enfoque iterativo e incremental, permitiendo una evolución progresiva del sistema desde un análisis inicial del problema hasta la implementación de un prototipo funcional. 

Se estructura en las siguientes fases:

1. **Análisis del problema y levantamiento de requisitos**
Estudio detallado del flujo actual de gestión del buzón, identificación de actores implicados y definición de requisitos funcionales y no funcionales.

2. **Análisis y diseño del sistema**
Definición de la arquitectura del sistema, modelado del flujo de datos, diseño de la integración con bases de datos y especificación de la lógica de negocio.

3. **Desarrollo del prototipo funcional**
Implementación del sistema automatizado, incluyendo la detección de correos entrantes, extracción de datos relevantes, consulta automatizada y generación de respuestas.
4. **Pruebas y validación**
Evaluación del funcionamiento del sistema mediante pruebas controladas, análisis de resultados y verificación del cumplimiento de los requisitos definidos.
5. **Evaluación y conclusiones**
Análisis del impacto potencial del sistema y propuesta de posibles mejoras o líneas futuras de actuación.