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

---

>todas estas practicas deben evaluarse y aplicarse de forma continua durante todo el ciclo de vida de las aplicaciones y la Infraestructura basadas en AWS.

## Planificacion

>no solo es el primier paso de la arquitectura, es un paso fundamental. garantiza que cuente con todos los aspectos cruciales.

1. Comience con los requisitos empresariales
2. implemente un diseño9 a prueba de fallas
3. implemente la seguridad en todos los niveles
4. automatice cuando sea posible
5. utilice servicios administrados
6. Supervise y realice mediciones
7. mantengase al dia. 

## Recursos de planificacion

determine los requisistos formulando las preguntas correctas a fin de ayudar a perfeccionar el alcance y la precision de su arquitectura.

[Ir al Centro de Arquitecturas](https://aws.amazon.com/es/architecture/how-to-build-this/?tma.sort-by=item.additionalFields.airDate&tma.sort-order=desc&awsf.categories=*all)

## Requisitos funcionales frente a no funcionales

>El objetivo fianl de un proyecto es entregar un producto de alta calidad tal y como lo solicito el cliente.

### Funcionales 

**Requisitos Funcionales**: Definen lo que un producto o sistema debe hacer y cuales son sus caracteristicas y funciones.

    * los **requisitos funcionales** son la principale forma en que un cliente expresa susrequisitos al equipo del proyecto.
    * los **requisitos funcionales** ayudan a que el equipo del proyecto avance en la direccion correcta.

|  concepto     |         Funcionales |
| ------------- | ------------------------------ |
|  Objetivo      | Describen lo que hace el producto |
| Resultado Final | Definen las caracteristicas del producto |
| Enfoque       | Se enfocan en los requisitos delusuario |
| documentacion | Capturados en el caso de uso |
| Esencialidad | Obligatorios |
| tipo de origen | Definidos por el usuario |
| pruebas |     Pruebas de componentes, Api e interfaz del usuario |

### No Funcionales

**Requisitos no funcionales**: describen las propiedades generales de un sistema.

Por lo general, un clinete tiene necesidades y **deseos**:
    - Despues de analizar la estimacion de costos, es posible que solicite reducir el alcances(normalmente, eliminar algunos de los requisitos no funcionales reduce el alcance). 
        - muchos **requisitos no funcionales** pueden aumentar rapidamente el costo.
        - la **insuficiencia de requisitos no funcionales** puede causar una mala experiencia del usuario.

|   concepto        |       No funcionales
| ----------------------- | -------------------------------------|
| objetivo  | describe como funciona el producto |
| Resultado final | definen las propiedades del producto |
| enfoque | se enfocan en las expectativas del usuario |
| documentacion | capturado como atributo de calidad |
| esencialidad | no son obligatorios, pero son deseables | 
| tipo de origen | definidos por un desarrollador o un experto en tecnologia |
| pruebas | pruebas de rendimiento, usabilidad y seguridad | 

---

>carla tecnica "Marco del buen arquitecto: proceso o checklist ?"

duracion 5min y 17 sec. 

# Infraestructura global de AWS 
    los centros de datos y la conectividad de redes. sigue siendo la base de todas las apliaciones en la nube. en AWS, esta infraestructura fisica constitue la infreastrutura global de AWS en forma de regiones y zonas de disponibilidad.

## centro de datos de AWS 

en 2006, aws fue pionero de la computacion en la nube. AWS innova continuamente el diseño y los sistemas de centros de datos para protegerlos de riesgos ocasionados por el hombre o naturales. como resultados las organizaciones con mayor regulacion del mundo confian en AWS todos los dias

## zonas de disponbilidad

una zona de disponibilidad consta de uno o mas centros de datos discretos, cda uno con capacidad redundante, redes y conectividad en una region de AWS. las varias areas aisladas dentro  de una ubicacion geografica particular. cuando lanza una instanci, puede seleccionar una zona de disponibilida o dejar que AWS elija una por ustd. 
las AZ funcionan en caso de producirse un erro en un centro de datos, puede diseñar su aplicacion para que de forma automatica se lanace otra en otra AZ.

## regiones 
Cada region de AWS consta de varias AZ ailadas y separadas fisicamente, gracias a esto se logra mayor tolerancia a errores. y estabilidad posible. en su cuenta, usted determina que regiones necesita. puede ejecutar aplicaciones y caras de trabajo de una region a fin de reducir la latencia par alos usuarios finales. Tambien puede hacer esto mientras evita los gastos iniciales, los compromisos a largo plaazo, los desafios de escalado asociados con el mantenimiento y la operacion de una infraestructura global. 

## Zonas Locales de AWS 

las zonas locales pueden utilizarse para las aplicaciones muy demandantes que requieren una latencia en milisegundos de un solo digito. para los usuarios finales. creacion de contenido multimedia y de entretenimiento, los juegos multijugador en tiempo real, el alojamiento y entrenamiento de machinelearning

## Ubicaciones perifericas 

una ubicacion periferica es el punto mas cercano a un solicitante de un servicio de AWS. Dichas ubicaciones estan situadas en las grandes ciudades del mundo. Reciben solicitudes y almacenan en cache copias de su contenido para agilizar la entrega 

### selecion de region 

Son independientes entre sí: sin el consentimiento y la autorización explícitos del cliente, los datos no se replican de una región a otra. Cuando decida en qué región de AWS alojará sus aplicaciones y cargas de trabajo, tenga en cuenta cuatro aspectos principales: la gobernanza, la latencia, la disponibilidad del servicio y el costo.

### diferencias reales de AWS Local Zones y Edge Locations

| AWS Local Zones | Edge Lotations |
|  ------------------------ | ------------------------------- |
| * baja latencia   |   * Caching of data  |
| * procesamiento de informacion local | * entrega de contenido rapidisima | 
| * Experiencia consistente de AWS | * Mejor experiencia de usuario | 


# Seguridad y modelo de responsabilidad compartida de AWS 

## Responsabilidad de AWS

AWS es responsable de la seguridad de la nube. Esto significa que AWS protege y asegura la infraestructura que ejecuta los servicios ofrecidos en la nube de AWS. AWS es responsable de lo siguiente:

Proteger y asegurar las regiones, las zonas de disponibilidad y los centros de datos de AWS, hasta la seguridad física de los edificios.

Administrar los componentes de hardware, software y redes que ejecutan los servicios de AWS, como los servidores físicos, los sistemas operativos de host, las capas de virtualización y los componentes de redes de AWS.

El nivel de responsabilidad de AWS depende del servicio. AWS clasifica los servicios en dos categorías, cuya información se detalla en la siguiente tabla, junto con la responsabilidad de AWS.

## Responsabilidad del cliente 

Los clientes son responsables de la seguridad en la nube. Cuando utiliza cualquier servicio de AWS, el cliente es responsable de configurar correctamente el servicio y sus aplicaciones, y garantizar que sus datos estén seguros.

El nivel de responsabilidad de los clientes depende del servicio de AWS. Algunos servicios requieren que el cliente realice todas las tareas de configuración y administración de seguridad necesarias. Otros servicios más abstractos requieren que los clientes solo administren los datos y controlen el acceso a sus recursos. Cuando se utilizan las dos categorías de servicios de AWS, los clientes pueden determinar su nivel de responsabilidad para cada servicio de AWS que utilicen.

# Aspectos basicos de las redes

## direcciones IP (addressing)

en aws se utilizan la notacion CIDR o enrutamiento entre dominios sin clases. siempre que se vea una direccion seguido de un slash '/'. 
entre mayor sea el numer , mas pequeña es la red, a menor numero mayor numeros de hosts disponbibles hay para utilizar en las subredes, de manera que tu tengas una red /16, sera una red que tendra 172.31.2.15/16 
el 2.15 sera el area designada para los hosts. tendras 2 octetos para los hosts. 

en la VPS puedes utilizar la direccion 0.0.0.0/0 que representa todo el rango de direcciones ip disponibles, para uso interno. 

* una direcion IP identifica la ubicacion de un recurso dentro de la red, en resumen esta dividida en 2 partes, la parte de la red y la parte del host, 

### direccion IPv4
la direccion IPv4 salio en los años 80s y utiliza direcciones de 32 bits, se agrupan en octetos.
se anotan en direccion numerica decimal. pueden crear mas de 4300 millones de direcciones, es decir se deben volver a usar y se deben enmascarar.

### direccion IPv6

en el 98 se desarrollo las IPv6 Para remplazar a las IPV4, Utiliza direcciones de **128** bits, las direcciones se dividen en 8 grupos de cuatro digitos, hexadecimales para un total de 128 bits, los grupos se escriben con el signo de los dos puntos por separado.
 
    50b2:6400:0000:0000:0000:6c3a:b17d:0:10a9

las direcciones IPv6 admiten la configuracion automatica.

cuando creas tu red en **AWS** con componentes de la VPC, especificas los bloques de CIDR y subredes. debes asignar la cantidad suficiente de direcciones IP para adminitir los recuruso de la red. puede contener hasta 5 bloques CIDR y los intervalos de direcciones no dse pueden superponer.

>debemos dar un estudio mas profundo acerca de la notacion CIDR y la practica de como dividir nuestra VPC en *n* cantidad de subredes, no olvidemos que muchos de los recursos deben estar organizados en subredes. 
>> recordar que la red mas pequeña es la de /28 con 16 direcciones IP y la mayor disponible es la de /16 que contiene un max de 65 536. 

En resumen, la red se puede identificar usando de 16 a 28 bits en la dirección IPv4 de 32 bits. Por otro lado, los recursos en la subred se pueden identificar con 4 a 16 bits en la dirección IPv4 de 32 bits.

> puedes utilizar esta herramienta online para practicar y visualizar la notacion CIDR, calcular subredes y entender mejor la distribucion de direcciones IP en tu VPC.

[calculadora de CIDR](https://cidr.xyz/)

## Amazon VPC 

es el entorno de la red en la nube, con **VPC**, puede iniciar recursos de AWS en una red virtual que usted defina. las VPC se implementan en una de las regiones de AWS. y pueden alojar recursos de cualquier zona de disponbilidad dentro de esa region. 

### Subred

es un rango de direciones IP dentro de la VPC. existen subredes publicas y privadas, que es lo que convierte una subred privada a una publica ????
la respuesta es una ruta hacia el exterior. 
como logramos esto?. mediante 2 cosas, la creacion de un Internet Gateway, despues crear la ruta dentro de la route table de casa subred.

hay que considerar que aunque tengamos una subredpublica no garantiza la comunicacion entre instanciaas a internet, porque aun debemos configurar el firewall del grupo de seguridad en las EC2. 

puntos fuertes a considerar:
* una subred no puede ser mas grande que la VPC que la contiene. 
* existen subredes publicas y privadas.
* por defecto toda subred contiene una tabla de enrutamiento.
* la mejor practicas de segurida es nunca exponer nuestros recursos criticos en las subredes publicas, sino crear una ruta desde la privada, que los lleve hasta la internetgateway.

### componentes de la VPC

#### subredes publicas

Una subred pública está asociada a una tabla de enrutamiento que tiene una ruta a una puerta de enlace de internet. Le permite comunicarse con recursos dentro de la subred desde la Internet pública mediante la asignación de direcciones IP públicas. La configuración de la subred pública actúa como una puerta bidireccional: permite que el tráfico fluya en ambas direcciones, ya sea solicitado o no.

Las subredes públicas utilizan lo siguiente:

Las puertas de enlace de internet permiten la comunicación entre los recursos de la VPC e internet.
Las tablas de enrutamiento son un conjunto de reglas que la VPC usa para enrutar el tráfico de red. En una subred pública, incluye una ruta a la puerta de enlace de internet.
Las direcciones IP públicas son accesibles desde internet. 
Las direcciones IP privadas solo son accesibles en la red.

#### puerta de enlace de internet 

Una puerta de enlace de internet es un componente de la VPC de alta disponibilidad, redundante y que se escala de forma horizontal que permite la comunicación entre las instancias en la VPC e internet. Por lo tanto, no representa riesgos de disponibilidad ni limitaciones de ancho de banda en su tráfico de red. Una puerta de enlace de internet admite el tráfico IPv4 e IPv6.

Una puerta de enlace de internet tiene dos propósitos: 

2. Proporciona un objetivo en su tabla de enrutamiento para el tráfico enrutable de internet.

2. Protege las direcciones IP en su red mediante la traducción de direcciones de red (NAT).

Una puerta de enlace de internet realiza la traducción de direcciones de red (NAT) asignando las direcciones IP públicas y privadas. En este ejemplo, la puerta de enlace de internet traduce la dirección IP fuente de una solicitud desde una dirección IP privada utilizada en la red (172.31.2.15) a una dirección IP pública (54.56.9.10). El destinatario dirige su respuesta a la dirección IP pública. La puerta de enlace de internet recibe la respuesta y traduce la dirección IP pública para la dirección IP privada con la que coincide. La VPC enruta la respuesta para el solicitante.

#### Tablas de enrutamiento

Una tabla de enrutamiento contiene una serie de reglas (rutas) que se utilizan para determinar hacia dónde se dirige el tráfico de red. Cuando crea una VPC, esta tiene automáticamente una tabla de enrutamiento principal. Inicialmente, la tabla de enrutamiento principal (y todas las de una VPC) contiene una única ruta: una ruta local con la que se puede establecer la comunicación de todos los recursos dentro de la VPC. No se puede modificar la ruta local en una tabla de enrutamiento. Cuando quiere iniciar una instancia en la VPC, la ruta local automáticamente cubre esa instancia. Se pueden crear tablas de enrutamiento personalizadas adicionales para su VPC.

#### subredes privadas

Las subredes privadas permiten el acceso indirecto a Internet. El tráfico se queda dentro de su red privada. Una dirección de IP privada asignada a una instancia de EC2 no cambiará a menos que se asigne manualmente una nueva dirección IP en la interfaz de red de la instancia de EC2. 

Aunque puede poner las instancias de nivel web en una subred pública, le recomendamos que las ponga dentro de subredes privadas detrás de un equilibrador de carga ubicado en una subred pública. Más adelante en este curso abordaremos Elastic Load Balancing (ELB).

#### VPC predeterminada

Todas las cuentas de AWS traen una VPC predeterminada y está configurada para que la pueda utilizar de inmediato. No necesita crear y configurar su propia VPC. Este es el gráfico de una VPC predeterminada. El bloque de CIDR para la VPC predeterminada siempre es una máscara de subred /16. En este ejemplo, el bloque de CIDR de 172.31.0.0/16 implica que esta VPC puede proporcionar hasta 65 536 direcciones IP. Incluye solo una subred pública en cada zona de disponibilidad en la región. Estas subredes utilizan una máscara de subred de /20 y proporcionan 4096 direcciones por subred. También incluye una puerta de enlace de internet. La VPC utiliza una tabla de enrutamiento principal para conectar las subredes a la puerta de enlace de internet.

Las varias capas independientes de seguridad son un factor disuasivo que disminuye el impulso y la efectividad de un ataque. Este enfoque requiere que el atacante atraviese varias capas de defensa especializada. El esfuerzo que requiere montar el ataque lo vuelve difícil y costoso. 

### Lista de control de accesos o ACL para los amigos.

los ACL son una medida opcional para tus VPC que actua como un *Firewall* de acceso, con el objetivo de filtrar y controlar el trafico, por defecto, tu VPC predeterminada y las que crees, contienen una ALC por defecto, ademas que son **sin estado**

**Sin Estado*** quiere decir que no recuerdan y si necesitan tener reglas de entrada y de salida. (stateless)

#### Trafico IPv4 entrante y saliente

- Una ACL de la red contiene una lista de reglas numeradas. las evaluamos en orden, comenzando por la regla con el numero mas bajo, para determinar si se permite la entrada o salida de trafico a cualquier subred asociada con la ACL de la red
- Las VPC incluyen automaticamente una ACL de red predeterminada y modificable. por defecto, todo el trafico IPv4 esta permitido, tanto entrante como saliente. puede crear una ACL de la red personalizada y asociarla a una subred. De forma predeterminada las ACL de la red personalizadas deniegan todo el trafico entrante y saliente hasta que se agreguen las reglas.
- cada ACL de la red incluye una regla cuyo numero de regla es un asterisco. esta regla garantiza que si un paquete no coincide con ninguna de las demas reglas enumeradas, se denegara. esto no se puede modificar ni eliminar. 

#### Reglas de ACL de la red

Cada ACL de la red incluye una regla cuyo numero de regla es un asterisco. esta regla garantiza que si un paquete no coincide con ninguna de las demas reglas numeradas, se denegara. esto no se puede modificar ni eliminar. entre los componente de una ACL de la red podemos encontrar: 

- numero de la regla: las reglas se evaluan comnezando por la regla con el numero mas bajo. no bien una regla coincide con el trafico, se aplica sin importar que haya otras reglas con numero mas altos que la contradigan.
- tipo: el tipo de trafico, por ejemplo, Secure Shell o SSH. tambien puede especificar todo el trafico o un intervalo personalizado.
- protocolo: puede especificar cualquier protocolo que tenga un numero de protocolo estandar.
- intervalo de puertos: el puerto de escucha o intervalo de puertos para el trafico. por ejemplo el trafico del puerto 80 para HTTP. 
- Fuente: solo las reglas entrantes, la fuente del trafico(intervalo de CIDR).
- Destino: solo para reglas salientes, el destino para el trafico(intervalo de CIDR).

las ACL de la red no tiene estados, lo que significa que las respuestas para el trafico entrante permitido estan sujetas a las reglas para el trafico saliente, y viceversa.

### Grupos de seguridad.

los grupos de seguridad funcionan como un firewall virtual de la instancia para controlar el trafico entrante y saliente. los grupos de seguridad actuan en el nivel de la interfaz de red, no en el nivel de la subred, y solo admiten reglas de permiso. 

- permite el trafico en funcion de un protocolo IP, un puerto o una direccion IP, y utiliza reglas con estado, el trafico se restingre con direccion IP , puerto, ip origin o destino y bloque CIDR

#### grupos de seguridad predeterminados y nuevos

de forma predeterminada, los SG security groups. se incluye una regla de salida que permite que todo el trafico salga, es posible quitar esa regla y agregar reglas de salida que permitan unicamente cierta parte especifica del trafico saliente. si su grupo de segurida no tiene reglas de salida, no se permite el trafico saliente que se origina desde su instancia.

#### reglas personalizadas de los grupos de seguridad

Con las reglas de las grupos de seguridad. puede filtrar trafico en funcion de los protocolos y numeros de puertos, los grupos de seguridad son con estado. si envian una solicitud desde su instancia, se permite que el trafico de respuesta para esa solicitud fluya sin importar las reglas de entrada del grupo de seguridad.

#### encadenamiento de grupos de seguridad

- una cadena de grupos de seguridad. establece de forma escalonada el flujo de acceso a los recursos. determinando una serie de reglas, que permiten un trafico de un nivel superior hasta un nivel inferior. los grupos de seguridad funcionan como firewalls para evitar que una filtracion de segurdiad en un nivel proporcione automaticamente acceso a toda la subred de tos los recusos al cliente comprometido.
 
 ### Comparacion entre grupos de seguridad y ACL de la red

 un grupo de seguridad actua como firewalls para las instancias de EC2 asociadas, ya que controla el trafico entrante y saliente en el nivel de la instancia. 

 Las ACL de la red actuan como un firewall para subredes asociadas y controla el traico entrante y saliente e el nivel de la subred. una ACL de la red deniega la comunicacion de forma predeterminada. el orden de las reglas de la ACL de la red es importante. 

| Grupos de seguridad | ACL de la red | 
|--------------------------- | ----------------------- |
| los grupos de seguridad actuan como firewall de la instancia ec2 asociadas y esta asociadas con la interfaz de red elastica implementada por el hipervisor | las ACL de red actuan como firewall para las subredes asociadas | 
| controlan el trafico entrante y saliente al nivel de la instancia | controlan el trafico entrante y saliente al nivel de la subred |
| Solo admite reglas de permiso | admite las reglas de permiso y denegacion | 
| es un firewall con estado | es un firewall sin estado |
| se debe asignar manualmente a las instancias | se aplica automaticamente cuando las instancias se agregan a la subred |

#### Caso de uso de una ACL de la red 

la ACL de la red controla el acceso a las instancias en una subred y actua como capa de defensa de respaldo, las reglas de ACL de la red se aplica na todas las instancias en la subred.

# Computacion como servicio

existen 3 tipos de opciones a nivel fundamental: maquinas virtuales VM, servicios de contenedores y computacion sin servidor. 

## eleccion de la configuracion de computacion adecuada.
 
 al diseñar tu arquitectura en AWS, necesitara computacion para ejecutar sus servidores en la nube. AWS ofrece varias opciones de computacion. en primer lugar, debe saber que servicio de computacion usar para cada caso de uso. 

 > un hipervisor  es un software o firmware que permite compartir recursos de hardware fisico en una o mas maquinas virutales, el hipervisor aprovisiona los recursos para crear y ejecutar las maquinas virtuales. 

 el EC2 es un servicio que proporciona la capacidad de computacion segura y redimensionable en la nube. puede aprovisionar servidores virtuales denomianadas instancias.

### daremos un repaso rapido por EC2

es com un servidor en las instalaciones tradicional, pero esta disponible en la nube. puede admitir cargas de trabajo coom alojamiento web, aplicaciones, bases de datos, servicios de autenticacion y ccualquier otra cosa que un servidor pueda admitir. 

#### consideraciones sobre el lanzamiento de las instancias de EC2

1. *Nombre y etiquetas*: se recomienda agregar metadatos a los recursos en forma de etiquetas, en tipo clave valor para filtrar y agrupas cada uno de nuestros recursos o preyectos. con ellas ademas podemos administrar el control de acceso a los recursos, realizar seguimiento de los costos y ayudar a automatizar tareas y mantener todo organizado. 
2. *Aplicacion e imagen de SO*: que aplicacion o sistema operativo ejecutara esta instancia? 
3. *tipo y tamaño de la instancia*: que requisitos tecnicos debe cumplir? 
4. *par de claves*: como se conectara a la instancia con otros componentes de la aplicaion y como se autenticara el acceso?.
5. *Redes y seguridad*: que nube privada virtual (vpc), subred y grupos de seguridad utilizara?.
6. *Configuracion del almacenamiento.* : que tipo de almacenamiento de bloques es mejor para su caso de uso??
7. *ubicacion y tenencia*: Donde debe ejecutar sus intancias de EC2? 
8. *Scripts y metadatos* : que puede hacer para automatizar su lanzamiento? 

### AMI 

una ami podemos decir que proporciona la informacion necesaria para lanzar una instancia, un Servidor virtual en la nube. cuando necesitas varias instancias con la misma configuracion.puede lanzarlas desde la misma AMI. Cuando necesite instancias con distintas configuraciones. puede usar distintas Ami para lanzarlas. 

**Que incluye**

- una plantilla para el volumen raiz de la instancia, por ejemplo un sistema operativo, aplicaciones y un servidor de aplicaciones. 
- permisos de lanzamiento que controlan que cuentas de aws pueden utilizar la AMI para lanzar instancias.
- asignacion de dispositivos de bloques que especifican los volumenes que deben adjutnarse a la instancia cuando se lanza.

#### en donde se obtiene una AMI

1. utilizar las AMI prediseñadas de AWS
2. Buscar en el Marketplaces miles de soluciones 
3. cree tus propias AMI manualmente o utilice el generador de AMI para EC2

#### explicacion de los nombres de tipos de instancias.

sabemos que existen cientos de tipos de instancias a elejir, asi que es mejor clasificarlas de acuerdo a su uso. AWS trabaja con una nomenclatura. aprender a diferencias entre los tipos de isntancia es crucial para nuestro proyecto, pues uno de los pilares es la eficiencia en el rendimiento. 

    c6g.xlarge

*c* - la familia de instancia: la primera letra es la familia. entonces la familia c, esta optimizada para computacion, existen de uso general, instancias expandibles e intancias de uso intensivo y para memoria, etc.
*6* - la generacion: el numero indica la generacion, que aumenta con el paso del teimpo pues AWS actualiza su hardware en sus centros de datos.
*g* - a veces hay una o mas letras despues de lageneracion, representan propiedades adicionales. por ejemplo la *g* represnta *graviton2*, un procesador de ARM desarrollado por AWS. 
*xlarge* - la ultima parte representa el tamaño de la instancia. Esto incluye la CPU, la memoria, el almacenamiento y el rendimiento de la red. 

* recuerda estudiar las familias de instancias de EC2

1. De uso general
2. optimizada para computacion
3. optimizadas para memoria
4. Computo acelerado
5. Optimizadas para el almacenamiento
6. Optimizadas para la computacion de alto rendimiento HPC

## AWS computer Optimizer 

utilizar **Machine Learning** para analizar la configuracion actual de sus recursos y sus datos de uso de CloudWatch. Recibira recomendaciones de computacion segun su configuracion y uso.

las recomendaciones se pueden integrar en diferentes servicios. por ejemplo, se pueden exportar a S3 donde se intengran al explorador de costso de AWS y System Manager.

## Pär de claves

