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

1. Pilare
2. Principios de diseño
3. Enfoques
4. Preguntas 


 







