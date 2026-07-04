# AWS Solutions Architect - Fundamentals of Architecting on AWS (Español LATAM)

## rol del arquitecto de soluciones

es importante en el diseño e implementación de la computación en la organización

*Como puesto técnico sénior, los arquitectos son responsables de diseñar, implementar y administrar la infraestructura de computación en la nube de una organización. Los arquitectos de soluciones actúan como puente entre los requisitos empresariales complejos y las soluciones técnicas en la nube.*

## el arquitecto cuenta con responsabilidades clave: 

* Desarrollo de estrategias en la nube: 

    Crear la visión de arquitectura de la organización y el plan de desarrollo para la adopción de la nube.
* Diseño de soluciones: 

    Diseñar una infraestructura de nube escalable, rentable y segura.
* Seleccion de tecnologia: 

    Evaluar y seleccionar los proveedores y servicios de nube adecuados.
* Planificacion de la migracion: 

    Desarrollar estrategias para la transición de entornos en las instalaciones a entornos en la nube.
* Cumplimiento y Seguridad
    
    Garantizar que las implementaciones en la nube cumplan con los estándares de seguridad y los requisitos normativos.

* optimizacion de costos

    Equilibrar las necesidades de rendimiento con las restricciones presupuestarias.

* Tutoría

    Guiar a los equipos de desarrollo sobre las prácticas recomendadas de la nube.

## Debe contar con habilidades obligatorias

**el arquitecto debe contar con habilidades tecnicas y sociales, me llama mucho la atencion este ultimo pues nos declara la importancia de transmitir el conocimiento a nuestro equipo y clientes.**
1. Contar con el conocimiento tecnico suficiente en servicios y plataforma de AWS 
2. comprension de la infraestructura como codigo (IaC)
3. Experiencia en arquitectura y seguridad en redes
4. Sólidas habilidades de comunicación para conectar a los equipos comerciales y técnicos.
5. Conocimiento sobre las prácticas de DevOps y las canalizaciones de CI/CD.

> Dentro del dia a dia de un arquitecto de soluciones, no solo importa la parte tecnica, la mayoria del tiempo estaras de la mano con tus clientes y enfocaras toda tu atencion en transmitirle de forma sencilla los conocimientos tecnicos de los servicios y documentar toda los cambios hechos a las cargas de trabajos (workloads)
>> en gran medida invertiras tu tiempo en mantenerte actualizado para seguir brindando las features mas recientes y lo que mejor se adapte a nuestro cliente. 
>>> muy poco tiempo la pasaras construyendo y desplegando en AWS. necesitamos dedicarle lo suficiente a desarrollar las habilidades de comunicacion. 

## Herramientas y Tecnologias del arquitecto 
nuestro principal objetivo es de contar con lar herramientas necesarias y dominar las tecnologias actuales, que se adapten mejor a la necesidades de nuestro proyecto. estas incluyen las herramientas de tercerlos como **Terraform** y **Git**. 

### Stack de herramientas de diseño principales 
es el conjunto de herramientas que nos brinda de acceso programatico a los servicios de AWS
* consola de AWS: la interfaz basada en Web para administrar nuestros recursos.
* AWS CLI: la interfaz de linea de comandos para adm. servicios de AWS
* AWS CloudFormation: servicio de Infraestructura como Codigo (IaC) que utiliza el aprovisionamiento de recursos basado en plantillas versionables y repetibles.
* AWS CDK: CLoud Developer Kit infraestructura como codigo que utiliza lenguajes de programacion conocidos. 
* diagramas y centro de arquitecturas de AWS: arquitecturas de referencia y practicas recomendadas. 

### Planificacion y administracion de infraestructuras
dentro de la planificacion y admin. tenemos los diferentes servicios que el arquitecto debe saber manejar.
* *Well-architected Tool:* nos brinda una revision de las arquitecturas en funcion de las practicas recomendadas de AWS.
* *AWS Trusted Advisor:* un servicio que contantemente supervisa nuestros entornos. 
* *Cost Explorer:* nuestro panel personal, una herramienta de estimacion y optimizacion de costos.
* *AWS Organizations:* administracion de varias cuentas y facturacion unificada. 
* *AWS Control Tower:* configuracion y gobernanza de varias cuentas (podemos minimizar costos utilizando la economia de escalas).

### Supervision y Seguridad 
 * *CloudWatch*: servicio para monitoreo y gobernanzas de nuestros servicios desplegados
 * *CloudTrail*: Capacidades de gobernanza, cumplimiento y auditorias
 * *AWS Config*: inventario de recursos y seguimiento del historial de configuracion
 * *Security Hub* administracion de la posicion de seguridad. (Realmente no entiendo que dice)

 ### Implementacion y DevOps 
 * *AWS CodePipeline, AWS CodeDeploy y AWS CodeBuild:* integración e implementación continuas.

 * *AWS Elastic Beanstalk:* plataforma como servicio (PaaS) para la implementación de aplicaciones.

 ### Herramientas de terceros

 muy importante comprender que AWS no es un entorno cerrado y nos permite integrar servicios y aplicaciones de tercero
 * *Terraform*: plataforma de infraestructura como codigo multinube.
 * *Draw.io*: herramientas de diagramas de arquitectura
 * Repositorios de GIT: control de versiones para proyectos y plantillas. 

## Impacto empresarial
los arquitectos de soluciones al momento de trabajar, diseñar y construir la infraestructura de AWS deben conseguir un valor empresarial real a traves de impactos. el valor real surge de las ventajas competitivas, la satisfaccion de nuestro cliente y oportunidades de crecimiento empresarial. 

### Beneficios

#### Financieros 
como siempre el cochino dinero
* **optimizacion de los costos:** reduciendo por encima del 20% hasta donde llegues, en costos totales de infraestructura mediante el dimensionamiento correcto de los recursos, la implementacion del escalado automatico y el aprovechamiento de los modelos de precios de AWS, por ejemplo las instancias reservadas con picos predecibles, instancias spot de cargas de trabajo no criticas, o que pueden soportar caidas temporales.

* **Cambio de CapEX a OpEx:** donde transformamos los gastos de capital inicial, cuando cotizamos el total de la infraestructura cuando realmente en AWS podemos cambiarlo por gastos operativos predecibles gracias a los servicios de Admin y costos en AWS. 

#### Excelencia operativa

* **Escalabilidad:** las empresas pueden escalar rapidamente todos sus recursos para satisfacer la demanda sin aprovisionamiento excesivo.

* **Velocidad de comercializacion:** podemos crear y destruir nuestras nuevas arquitecturas en cuestion de horas o incluso minutos haciendo uso de las plantiallas YAML o stacks de terraform. en vez de semanas. 

* **Reduccion de la deuda tecnica:** entenamos la deuda tenica  como un proceso continuo donde debemos refactorizar o pagar ese codigo que desplegamos, utilizar esa tecnologia y el costo impolicito futuro. 

#### Agilidad Empresarial

* **Aceleracion de la innovacion:** se brinda accesso a mas de 200 servicios de AWS especializados que permiten la creacion rapida de prototipos. 
* **Continuidad de actividades:** se diseñan arquitecturas resilientes de varias AZ y varias regiones que minimizan los riesgos de tiempo de inactividad. 
* **Alacnce global:** esta es buena pues elimina los orizontes y facilita una expancio rapida en nueos mercados geograficos con una sobrecarga minima de infraestructura. 

##### Riesgos

* **seguridad mejorada:** gracias a los servicios integrales de AWS podemos dar una proteccion mas profunda.

* **Cumplimiento:** debemos cumplir con los requisitos normativos, aunar mas profundo en cada uno de las distintas normas.

* **Capacidades de recuperacion ante desastres:** se crean las estrategias necesarias, estas en el pasado eran inexistentes. gracias a la arquitectura de la nube de AWS podemos generar distintos planes y como minimizar el tiempo de inoperabilidad. 

## Arquitectura en la nube
en este capitulo apreciamos la relevancia que trae el framework del WAF. antes de la nube y ahora en la nube, las cargas de trabajo se diseñaban de maneras diferentes y siempre con pura intuicion, por lo general era demasiado costoso y solo se hacia al principio del proyecto, una vez en produccion, dificilmente se pondrian a preguntarse, que cambios, que mejoras o incluso que nuevas tecnologias podrian adoptar.
El Framework del WAF, te ayuda a entender las ventajas y desventajas de las decisiones que tomas durante la creacion de las cargas de trabajo en AWS. Tener un  sistema bien diseñado ayuda muchisimo a mejorar la probabilidad de exito empresarial.

## Marco de AWS Well-Architected

ahora vamos al ¿ por que ?
* **Crear e implentar con mayor velocidad:**
* **Disminuir o mitigar los riesgos:**
* **Tomar decisiones fundamentadas:** 
* **Aprender sobre las practicas recomendadas de AWS** 

> WAF es una herramienta de cuantificacion de los riesgos. debemos aprender, compara y mejorar siempre nuestras arquitecturas en la nube a lo largo de todo el ciclo de vida. 
>> lo que no se mide, no se mejora...

repasemos 4 conceptos muy importantes en el framework

1. Pilares
2. Principios de diseño
3. Enfoques
4. Preguntas 

### Pilares
 tenemos los 6 pilares del Marco del Buen Arquitecto
 1. Excelencia Operativa
    * la capacidad de ejecutar y supervisar los sistemas para generar valor empresarial y para mejorar de forma continua los procesos y procedimientos de respaldo.

 2. Fabilidad
    * la capacidad de que tu workload  trabaje de forma correcta y uniforme, en otras palabras que no de lata y que sea fiable
    * recuperarse de errores en la infraestructura o interrupciones del servicio. que planees los errores antes de que ocurran y te prepares.
    * adquirir de manera dinamica recursos de computo para satisfacer la demanas, me suena a el Grupo de autoScaling
    * Mitigar interrupciones, como errores de configuracion o problemas transitorios de la red.
 3. Seguridad: la capacidad de proteger la informacion, los sistemas y los activos y al mismo tiempo, ofrecer valor empresarial mediante evaluaciones de riesgos y estrategias de mitigacion.

 4. Eficiencia en el rendimiento: la capacidad de utilizar recursos de computo de manera eficaz para satisfacer los requisitos del sistema. asimismo, implica la capacidad de mantener esta eficacia a medida que cambia la demanda y evolucionan las tecnologias.
 
 5. Optimizacion de costos: esta esta facil, entre menos gastes mejor, el pilar mas deseado de las empresas. pero que siga cumpliendo con los objetivos del sistema.  
 6. sostenibilidad: recordemos que codear, maquinas virtuales de github, utilizan recursos computacionales y eso aunmenta nuestra huella de carbono. aunmentar la eficienci en los componentes de una carga de tragbajo es necesario,maximizando los beneficios de los recursos

### Principios de Diseño
Basicamento son conceptos y formas de pensar que debe considerar al momento de diseñar una carga de trabajo.
    Por ejemplo, dentro del pilar de seguridad, uno de los aspectos que debe tener en cuenta es el cifrado. ¿que es lo que hay que cifrar y cuando hay que hacerlo.

El marco proporciona preguntas que se basan en los pilares, esta basados en años de conocimientos de los puntos debiles comunes de los clientes.



### Enfoques 
    los enfoques compara constantemente sus arquitecturas con las practicas recomendadas e identificar las areas de mejora. 

### Preguntas
ya trae definidar un conjunto de preguntas basadas en los principios de diseño en seis pilares.
    las preguntas facilitan una conversacion que birnda infroamcion y podemos resolver los problemas.

Amazon hace una analogia a construir un edificio, si no contiene las bases solidas, los problemas en la estructura pueden socavar la integridad y el funcionamiento del edificio. 

    los 6 pilares del framework se basan en principios de diseño para crear un sistema que funcion de acuerdo  a las espectativas.
> una parte escencial de las preguntas es que en la herramienta del welll-architected tool, nos va guiando a lo largo de todos los pilares y son preguntas que ya vienen aprovadas y testeadas, nos ayudan a enclareser las desiciones que hay que tomar si o si al diseñar nuestro servicio y como ira actualizando.

## Herramienta de AWS Well-Architected 

las workloads siempre ofrecen un valor empresarial. se deben actualizar y marcar los hitos para ver como mejora con el timepo. una especie de versionamiento de nuestros stacks tecnologicos.

la **Herramienta de AWS Well-Architected (AWS WA) es una app web, en la consola, es de autoservicio. 

### Revision de Well-Architected

como buena constumbre siempre es recomendado evaluar nuestra workload, y ver si cumple el marco. 
puntos importantes: 

* el problema mas comun no son las malas decisiones. sino, las personas que descuidan la decision y ni siquiera hablan sobre ella.

* la mayoria de workloads tienen elementos de alto riesgo. debes abordarlos, asi puedes evitar eventos que dañen  o ralenticen su empresa.

#### Caracteristicas de la herramientas
> la herramienta como cada servicio de AWS ofrece una amplia gama de caracteristicas. que ayudan a aplicar las practicas recomendadas, de arquitectura. identificar los riesgos e implmentar mejoras en las cargas de trabajo en la nube de manera estructurada.

* **Cargar de trabajo**
    * ejemplos practicos serian: sitios web de marketing, un e-commerce, el backend de una app movil y las plataformas analiticas.
    * pueden ser simples, como una SPA, o complejas como microservicios con varios almacenes de datos y muchos componentes. 
* **HItos en ingles Milestone**
    * definimos los hitos, como hechos que marcan un cambio clave en la arquitectura a medida que evoluciona a lo largo del ciclo de vida del producto. (el diseño, pruebas, puesta en marcha y la produccion).

* **Enfoques**: 
    *  proporciona una forma de compara tu arquiteftura con las practicas recomendadas, ademas puedes personalizarlas a tu antojo, ahora si que selecciones la que mas te agrade a ti.
* **Problemas de riesgo alto**: llamemos le HRI estas operaciones pueden repercutir en las operaciones en la organizacion, los activos y las personas. 
* **Probleas de riesgo medio**: MRI son opciones arquitectonicas y operativas que AWS podrian afectar negativamente a la empresa pero mesno que las HRI.

>puedes definir la prioridad de los pilares a la hora de realizar la revision de tu workload. ademas que como ultimo paso generar un  informe, visualizar los resultados de toda la organizacion en unico panel. 
## Medicion del exito

a continuacion se listaran las diferentes metricas que utilizaremos como arquitecto de soluciones, para medir nuestro exito, mas adelante, las veremos mas a profundidad. estan por pilar

*Excelencia operativa*

    * Tiempo medio de recuperación (MTTR)
    * Tiempo medio entre errores (MTBD)
    * Frecuencia de implementación y tasas de éxito
    * Tiempo para detectar y resolver problemas
    * Tasas de éxito de la administración de cambios
    * Cobertura de automatizació
*Seguridad*

* Tasas de incidentes de seguridad
* Tiempo de aplicación de parches en los sistemas
* Resultados de la auditoría de cumplimiento
* Porcentaje de recursos que cumplen con las prácticas recomendadas de seguridad
* Cantidad de hallazgos de seguridad
* Tiempo para responder a eventos de seguridad
*Fiabilidad*

* Porcentaje de disponibilidad del sistema
* Objetivo de tiempo de recuperación (RTO)
* Objetivo de punto de recuperación (RPO)
* Tasas de error
* Cantidad de conmutaciones por error exitosas
* Cumplimiento del acuerdo de nivel de servicios (SLA)

*Eficiencia del rendimiento*

* Tasas de uso de recursos
* Tiempos de respuesta
* Métricas de latencia
* Rendimiento
* Métricas de escalabilidad del sistema
* Tasas de aciertos de caché

*Optimiazion de costos*

* Costo por unidad de trabajo
* Uso de recursos en comparación con el costo
* Identificación y reducción de residuos
* Cobertura de instancias reservadas
* Exactitud en la asignación de costos
* ROI de las inversiones en la nube

*Sostenibilidad*

* Métricas de la huella de carbono
* Eficacia de los recursos
* Administración del ciclo de vida del hardware
* Uso de energía renovable
* Reducción del impacto ambiental
* Prácticas de arquitectura sostenible

## Practicas recomendadas
 >se organizan en tornos a los 6 pilares clave del well-architected. te guian al momento de crear una infreaestructura de aplicaciones seguras y de alto rendimiento, resiliente y eficiente.

 a continuancion se listan algunas de las practicas recomendadas.
 
 ### Seguridad

 1. **Defensa en profundidad**: implementar muchos controles de seguridad en las diferentes capas.
 2. **Administracion de identitades y accesos**: utilice AWS IAM con el principio de minimo privilegio. 
 3. **proteccion de datos**: cifre los datos en reposo y en transito con KMS y CloudHSM. 
 4. **Seguridad de la red:** Implemente grupos de seguridad, ACL de la red, WAF y Shield.
 5. **cumplimiento y auditoria**: utilice AWS Config y Security Hub. 

 ### Optimizacion de costos.

 * **Dimesionamiento adecuado de los recursos:** utilice recursos dimensionados correctamente para su carga de trabajo.
 * **Instancias reservadas y Saving Plans:** comprometase a usarlos para obtener descuentos significactivos.
 * **Instancias Spot:** debemos aprovechar nuestras cargas de trabajo no criticas y utilizar estos descuentos.
 * **Supervision de costos:** Implementar el explorador de costos y presupuestos de AWS.
 * **Politicas de cliclo de vida del almacenamiento:** automatice la migracion de datos a niveles de menor costo.

### Fiabilidad

* **Aislamiento de errores:** utilice varias zonas de disponibilidad y regiones.
* **Escalado:** implemente el escalado automatico en las cargas de trabajo dinamicas.
* **Planificacion de recuperacion:** diseñar con el objetivo de una recuperacion automatica y una perdida de datos minima.
* **Prueba de los procedimientos** de recuperacion: realice pruebas de recuperacion de desastres con regularidad.
* **Acoplamiento debil:** diseñe servicios para reducir las interdependencias.

### Eficiencia del rendimiento

* **Dimensionamiento correcto de los recursos:** selecciones los tipos de instancias adecuados para su carga de trabajo.
* **Aprovechamiento de los servicios adminstrados:** utilice los servicios de AWS en lugar de administrar la infraestructura
* **Almacenamiento en cache:** implementacion de ElastiCache o CloudFront para mejorar el rendimiento.
* **Optimizacion del almacenamiento de datos:** elija el servicio de almacenamiento adecuado *S3, EBS, EFS*
* **Arquitectura sin servidor:** considere *Lambda* para las cargas de trabajo impusladas por eventos.

### Excelencia operativa
* **Infraestructura como codigo:** Considere utilizar CloudFormation para automatizar las implementaciones.
* **Supervision y observabilidad:** Implementar *CLoudWatch,  X-Ray y CloudTrail*.
* **Integracion y entrega continua:** aproveche AWS CodePïpeline, Codebuild y CodeDeploy.
* **Manuales de procedimientos y guias:** documente los procedimientos para las opreaciones rutinarias y la respuesta ante incidentes. 

### Sostenibilidad
* **Uso de los recursos:** maximice la eficiencia para minimizar el impacto del entorno.
* **Seleccion de regiones:** elija regiones con fuentes de energia mas sostenibles siempre que sea posible.
* **Servicios admnistrados:** aproveche las economias de escala de AWS para aumnetar la sostenibilidad.
* **Optimizacion de las cargas de trabajo** mejore la eficiencia del codigo para reducir las necesidades de computacion. 
