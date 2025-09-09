# 📖 Glosario AWS Cloud Practitioner

> **Definiciones completas de términos clave de AWS y computación en la nube**

## 📋 Tabla de Contenidos

- [🌩️ Fundamentos de Computación en la Nube](#️-fundamentos-de-computación-en-la-nube)
- [🏗️ Infraestructura AWS](#️-infraestructura-aws)
- [💻 Términos de Cómputo](#-términos-de-cómputo)
- [💾 Términos de Almacenamiento](#-términos-de-almacenamiento)
- [🌐 Términos de Redes](#-términos-de-redes)
- [🗄️ Términos de Base de Datos](#️-términos-de-base-de-datos)
- [🔒 Términos de Seguridad](#-términos-de-seguridad)
- [📊 Monitoreo y Gestión](#-monitoreo-y-gestión)
- [💰 Términos de Facturación y Costos](#-términos-de-facturación-y-costos)
- [🔗 Integración y Mensajería](#-integración-y-mensajería)
- [📱 Aplicaciones y Desarrollo](#-aplicaciones-y-desarrollo)

---

## 🌩️ Fundamentos de Computación en la Nube

### **Auto Scaling**
El ajuste automático de recursos de cómputo basado en la demanda. AWS Auto Scaling monitorea aplicaciones y ajusta automáticamente la capacidad para mantener un rendimiento estable y predecible al menor costo posible.

### **Acceso Amplio a la Red**
Una de las cinco características esenciales de la computación en la nube. Las capacidades de la nube están disponibles a través de la red y se acceden mediante mecanismos estándar que promueven el uso por plataformas cliente heterogéneas.

### **Gasto de Capital (CapEx)**
Dinero gastado en adquirir o mantener activos fijos, como edificios y equipos. La infraestructura de TI tradicional requiere CapEx inicial significativo para servidores, centros de datos y equipos de red.

### **Computación en la Nube**
La entrega bajo demanda de recursos de TI y aplicaciones a través de internet con precios de pago por uso. Elimina la necesidad de invertir y mantener infraestructura física.

### **Elasticidad**
La capacidad de adquirir recursos cuando los necesitas y liberar recursos cuando ya no los necesitas. En la nube, quieres hacer esto automáticamente.

### **Alta Disponibilidad**
Un enfoque de diseño de sistemas e implementación de servicios asociada que asegura un nivel preestablecido de tiempo de actividad operacional. AWS proporciona alta disponibilidad a través de múltiples centros de datos y tolerancia a fallos.

### **Nube Híbrida**
Un modelo de implementación de nube que combina infraestructura local con servicios de nube, permitiendo que datos y aplicaciones se compartan entre ellos para mayor flexibilidad y optimización.

### **Infraestructura como Servicio (IaaS)**
Un modelo de computación en la nube donde un proveedor ofrece infraestructura de computadora (servidores, almacenamiento, redes) como servicio. AWS EC2 es un ejemplo de IaaS.

### **Servicio Medido**
Los sistemas de nube controlan y optimizan automáticamente el uso de recursos aprovechando una capacidad de medición. El uso de recursos puede ser monitoreado, controlado y reportado.

### **Autoservicio Bajo Demanda**
La capacidad de los usuarios para aprovisionar capacidades de cómputo automáticamente sin requerir interacción humana con proveedores de servicios.

### **Gasto Operativo (OpEx)**
Un gasto continuo para operar un negocio. La computación en la nube típicamente convierte los costos de TI de CapEx a OpEx a través de precios de pago por uso.

### **Pago por Uso**
Un modelo de precios donde solo pagas por los recursos que realmente usas, sin costos iniciales o compromisos a largo plazo a menos que los elijas.

### **Plataforma como Servicio (PaaS)**
Un modelo de computación en la nube que proporciona una plataforma permitiendo a los clientes desarrollar, ejecutar y gestionar aplicaciones sin lidiar con la infraestructura. AWS Elastic Beanstalk es un ejemplo.

### **Nube Privada**
Infraestructura de nube operada únicamente para una sola organización, ya sea gestionada internamente o por un tercero y alojada interna o externamente.

### **Nube Pública**
Servicios de nube ofrecidos a través del internet público y disponibles para cualquiera que quiera comprarlos. AWS es un proveedor de nube pública.

### **Agrupación de Recursos**
Los recursos de cómputo del proveedor de nube se agrupan para servir a múltiples consumidores usando un modelo multi-inquilino, con recursos físicos y virtuales asignados y reasignados dinámicamente según la demanda.

### **Escalabilidad**
La capacidad de un sistema para manejar carga aumentada agregando recursos al sistema. Puede ser vertical (escalar hacia arriba) u horizontal (escalar hacia afuera).

### **Software como Servicio (SaaS)**
Un modelo de computación en la nube donde las aplicaciones son alojadas por un proveedor de servicios y puestas a disposición de los clientes a través de internet. Ejemplos incluyen Office 365 y Salesforce.

---

## 🏗️ Infraestructura AWS

### **Zona de Disponibilidad (AZ)**
Uno o más centros de datos discretos con energía, redes y conectividad redundantes en una Región de AWS. Cada AZ está aislada de fallas en otras AZs.

### **AWS Local Zones**
Un tipo de implementación de infraestructura de AWS que coloca cómputo, almacenamiento, base de datos y otros servicios selectos de AWS más cerca de grandes centros de población e industria.

### **AWS Outposts**
Un servicio completamente gestionado que extiende la infraestructura, servicios, APIs y herramientas de AWS a las instalaciones del cliente para una experiencia híbrida verdaderamente consistente.

### **Región de AWS**
Una ubicación física alrededor del mundo donde AWS agrupa centros de datos. Cada Región consiste de múltiples AZs aisladas y físicamente separadas.

### **AWS Wavelength**
Implementaciones de infraestructura que integran servicios de cómputo y almacenamiento de AWS dentro de las redes 5G de proveedores de servicios de comunicaciones (CSP).

### **Ubicación de Borde**
Centros de datos propiedad de AWS o un socio de confianza que son parte de la red de entrega de contenido (CDN) CloudFront. Usados para almacenar en caché contenido más cerca de los usuarios.

### **Infraestructura Global**
La red mundial de AWS de Regiones, Zonas de Disponibilidad y ubicaciones de borde que proporciona alta disponibilidad, tolerancia a fallos y escalabilidad.

---

## 💻 Términos de Cómputo

### **Amazon EC2 (Elastic Compute Cloud)**
Un servicio web que proporciona capacidad de cómputo segura y redimensionable en la nube. Servidores virtuales que pueden escalarse rápidamente hacia arriba o hacia abajo.

### **Amazon ECS (Elastic Container Service)**
Un servicio de orquestación de contenedores altamente escalable que soporta contenedores Docker y te permite ejecutar y escalar aplicaciones en contenedores en AWS.

### **Amazon EKS (Elastic Kubernetes Service)**
Un servicio gestionado de Kubernetes que facilita ejecutar Kubernetes en AWS sin necesidad de instalar y operar tu propio plano de control de Kubernetes.

### **Grupo de Auto Scaling**
Una colección de instancias EC2 que son tratadas como una agrupación lógica para propósitos de escalado automático y gestión.

### **AWS Batch**
Un servicio que te permite ejecutar cargas de trabajo de computación por lotes en AWS. Aprovisiona automáticamente la cantidad y tipo óptimo de recursos de cómputo.

### **AWS Elastic Beanstalk**
Un servicio para implementar y escalar aplicaciones web y servicios. Subes tu código y Elastic Beanstalk maneja la implementación.

### **AWS Fargate**
Un motor de cómputo sin servidor para contenedores que funciona con Amazon ECS y Amazon EKS. Elimina la necesidad de aprovisionar y gestionar servidores.

### **AWS Lambda**
Un servicio de cómputo sin servidor que ejecuta tu código en respuesta a eventos y gestiona automáticamente los recursos de cómputo subyacentes.

### **Host Dedicado**
Un servidor EC2 físico dedicado para tu uso. Puede ayudar a reducir costos permitiéndote usar tus licencias de software existentes vinculadas al servidor.

### **Instancia Dedicada**
Instancias EC2 que se ejecutan en una VPC en hardware dedicado a un solo cliente. Pueden compartir hardware con otras instancias de la misma cuenta de AWS.

### **Tipos de Instancia EC2**
- **Propósito General**: Cómputo, memoria y redes balanceados (t3, m5, a1)
- **Optimizado para Cómputo**: Procesadores de alto rendimiento (c5, c5n)
- **Optimizado para Memoria**: Rendimiento rápido para cargas de trabajo intensivas en memoria (r5, x1e)
- **Optimizado para Almacenamiento**: Alto acceso secuencial de lectura/escritura a grandes conjuntos de datos (i3, d2)

### **Elastic Load Balancer (ELB)**
Distribuye el tráfico de aplicaciones entrantes a través de múltiples objetivos, como instancias EC2, contenedores y direcciones IP.

### **Instancia Spot**
Instancias EC2 que usan capacidad de reserva y pueden ofrecer hasta 90% de ahorro en costos comparado con precios Bajo Demanda. Pueden ser interrumpidas por AWS con aviso de dos minutos.

---

## 💾 Términos de Almacenamiento

### **Amazon EBS (Elastic Block Store)**
Proporciona volúmenes de almacenamiento a nivel de bloque para uso con instancias EC2. Los volúmenes EBS persisten independientemente de la vida de una instancia.

### **Amazon EFS (Elastic File System)**
Un sistema de archivos NFS gestionado que puede montarse en múltiples instancias EC2 simultáneamente. Proporciona almacenamiento compartido para aplicaciones.

### **Amazon S3 (Simple Storage Service)**
Servicio de almacenamiento de objetos que ofrece escalabilidad líder en la industria, disponibilidad de datos, seguridad y rendimiento para almacenar y recuperar cualquier cantidad de datos.

### **Almacenamiento de Bloques**
Almacenamiento que divide archivos en bloques de datos de tamaño uniforme, cada uno con su propia dirección pero sin metadatos adicionales. EBS proporciona almacenamiento de bloques.

### **Durabilidad**
La probabilidad de que los datos permanezcan intactos y accesibles. Amazon S3 proporciona 99.999999999% (11 nueves) de durabilidad.

### **Almacenamiento de Archivos**
Un método de almacenar datos en una estructura jerárquica de archivos y carpetas. Amazon EFS proporciona almacenamiento de archivos.

### **Almacén de Instancia**
Proporciona almacenamiento temporal a nivel de bloque para instancias. Los datos persisten durante la vida de la instancia pero se pierden cuando la instancia se detiene o termina.

### **Política de Ciclo de Vida**
Reglas que definen acciones que S3 aplica a objetos durante su vida útil, como transicionar objetos a diferentes clases de almacenamiento o eliminarlos.

### **Almacenamiento de Objetos**
Una arquitectura de almacenamiento que gestiona datos como objetos, en oposición a sistemas de archivos o almacenamiento de bloques. Cada objeto incluye datos, metadatos y un identificador único.

### **Clases de Almacenamiento S3**
- **Standard**: Datos accedidos frecuentemente
- **Standard-IA**: Datos accedidos infrecuentemente
- **One Zone-IA**: Datos accedidos infrecuentemente en una sola AZ
- **Glacier**: Archivo a largo plazo con tiempos de recuperación de minutos a horas
- **Glacier Deep Archive**: Almacenamiento de menor costo para retención a largo plazo
- **Intelligent Tiering**: Mueve automáticamente datos al nivel más rentable

### **Versionado**
La práctica de mantener múltiples variantes de un objeto en el mismo bucket de S3. Usado para preservar, recuperar y restaurar cada versión de cada objeto.

---

## 🌐 Términos de Redes

### **Amazon CloudFront**
Un servicio de red de entrega de contenido (CDN) que entrega de forma segura datos, videos, aplicaciones y APIs a clientes globalmente con baja latencia.

### **Amazon Route 53**
Un servicio web DNS escalable que traduce nombres de dominio a direcciones IP y enruta usuarios a aplicaciones de internet.

### **Amazon VPC (Virtual Private Cloud)**
Una sección lógicamente aislada de la nube de AWS donde puedes lanzar recursos de AWS en una red virtual que defines.

### **Red de Entrega de Contenido (CDN)**
Una red de servidores distribuidos que entregan contenido web y servicios a usuarios basado en su ubicación geográfica para minimizar la latencia.

### **AWS Direct Connect**
Una conexión de red dedicada entre tus instalaciones y AWS que puede reducir costos de red y aumentar el rendimiento del ancho de banda.

### **Internet Gateway**
Un componente VPC escalado horizontalmente, redundante y altamente disponible que permite comunicación entre instancias en tu VPC e internet.

### **NAT Gateway**
Un servicio gestionado que permite a instancias en una subred privada conectarse a internet u otros servicios de AWS mientras previene que internet inicie conexiones con esas instancias.

### **Lista de Control de Acceso de Red (NACL)**
Una capa opcional de seguridad para tu VPC que actúa como un firewall para controlar tráfico entrante y saliente de una o más subredes.

### **Conexión de Peering**
Una conexión de red entre dos VPCs que te permite enrutar tráfico entre ellas usando direcciones IPv4 privadas o direcciones IPv6.

### **Subred Privada**
Una subred donde las instancias no pueden comunicarse directamente con internet. Típicamente usada para servidores backend y bases de datos.

### **Subred Pública**
Una subred donde las instancias pueden comunicarse directamente con internet a través de un internet gateway.

### **Grupo de Seguridad**
Un firewall virtual que controla tráfico entrante y saliente para instancias EC2. Actúa a nivel de instancia y es con estado.

### **Subred**
Un rango de direcciones IP en tu VPC. Puedes lanzar recursos de AWS en una subred que selecciones.

---

## 🗄️ Términos de Base de Datos

### **Amazon Aurora**
Una base de datos relacional compatible con MySQL y PostgreSQL construida para la nube que combina rendimiento y disponibilidad de bases de datos comerciales de alta gama con la rentabilidad de bases de datos de código abierto.

### **Amazon DynamoDB**
Un servicio de base de datos NoSQL completamente gestionado que proporciona rendimiento rápido y predecible con escalabilidad perfecta.

### **Amazon ElastiCache**
Un servicio web que facilita implementar, operar y escalar una caché en memoria en la nube para mejorar el rendimiento de aplicaciones.

### **Amazon RDS (Relational Database Service)**
Un servicio gestionado que facilita configurar, operar y escalar una base de datos relacional en la nube.

### **Amazon Redshift**
Un servicio de almacén de datos completamente gestionado que hace simple y rentable analizar datos usando SQL estándar y herramientas de inteligencia de negocios.

### **Servicio de Migración de Base de Datos (DMS)**
Un servicio que te ayuda a migrar bases de datos a AWS rápida y seguramente mientras mantiene la base de datos fuente completamente operacional durante la migración.

### **Implementación Multi-AZ**
Una opción de implementación para RDS que aprovisiona y mantiene automáticamente una réplica standby síncrona en una Zona de Disponibilidad diferente.

### **Base de Datos NoSQL**
Una base de datos que proporciona un mecanismo para almacenamiento y recuperación de datos modelados de maneras distintas a relaciones tabulares. DynamoDB es la oferta NoSQL de AWS.

### **Réplica de Lectura**
Una copia de solo lectura de tu base de datos que puede crearse en la misma AZ, AZ diferente, o Región diferente para mejorar el rendimiento de lectura.

### **Base de Datos Relacional**
Una base de datos que organiza datos en tablas con filas y columnas, donde se pueden establecer relaciones entre diferentes tablas. Usa SQL para consultas.

---

## 🔒 Términos de Seguridad

### **AWS Certificate Manager (ACM)**
Un servicio que te permite aprovisionar, gestionar e implementar fácilmente certificados SSL/TLS para uso con servicios de AWS y recursos conectados internos.

### **AWS CloudTrail**
Un servicio que habilita gobernanza, cumplimiento, auditoría operacional y auditoría de riesgos de tu cuenta de AWS registrando llamadas API.

### **AWS Config**
Un servicio que te permite evaluar, auditar y evaluar las configuraciones de tus recursos de AWS para análisis de cumplimiento y seguridad.

### **AWS GuardDuty**
Un servicio de detección de amenazas que usa aprendizaje automático, detección de anomalías e inteligencia de amenazas integrada para identificar amenazas.

### **AWS IAM (Identity and Access Management)**
Un servicio que te permite gestionar acceso a servicios y recursos de AWS de forma segura a través de usuarios, grupos, roles y políticas.

### **AWS Inspector**
Un servicio automatizado de evaluación de seguridad que ayuda a mejorar la seguridad y cumplimiento de aplicaciones implementadas en AWS.

### **AWS Organizations**
Un servicio que te permite gestionar y gobernar centralmente tu entorno mientras creces y escalas tus recursos de AWS.

### **AWS Shield**
Un servicio gestionado de protección DDoS que protege aplicaciones ejecutándose en AWS contra ataques DDoS de capa de red y transporte.

### **AWS WAF (Web Application Firewall)**
Un firewall de aplicaciones web que ayuda a proteger aplicaciones web de exploits web comunes que podrían afectar la disponibilidad de aplicaciones o comprometer la seguridad.

### **Acuerdo de Socio Comercial (BAA)**
Un contrato entre una entidad cubierta por HIPAA y un socio comercial que establece usos y divulgaciones permitidos de información de salud protegida.

### **Cumplimiento**
Adherencia a leyes, regulaciones, pautas y especificaciones relevantes para operaciones comerciales. AWS proporciona certificaciones y atestaciones de cumplimiento.

### **Defensa en Profundidad**
Una estrategia de seguridad que emplea múltiples capas de controles de seguridad a través de un sistema de información para reducir el riesgo.

### **Cifrado en Reposo**
El cifrado de datos cuando se almacenan en un dispositivo de almacenamiento, protegiéndolos del acceso no autorizado si el medio de almacenamiento se ve comprometido.

### **Cifrado en Tránsito**
El cifrado de datos mientras se transmiten a través de una red, protegiéndolos de la intercepción durante la transmisión.

### **Política IAM**
Un documento que define permisos y especifica qué acciones están permitidas o denegadas para recursos específicos de AWS.

### **Rol IAM**
Una identidad de AWS con políticas de permisos que determinan qué puede y no puede hacer la identidad en AWS. Los roles son asumidos por entidades confiables.

### **Menor Privilegio**
Un principio de seguridad que otorga a los usuarios los niveles mínimos de acceso necesarios para realizar sus funciones laborales.

### **Autenticación Multi-Factor (MFA)**
Una capa adicional de seguridad que requiere que los usuarios proporcionen dos o más factores de verificación para obtener acceso a un recurso.

### **Principio de Menor Privilegio**
Un concepto de seguridad donde los usuarios reciben los permisos mínimos necesarios para completar sus tareas, reduciendo los riesgos de seguridad.

### **Usuario Root**
La dirección de correo electrónico usada para crear una cuenta de AWS. Tiene acceso completo a todos los servicios y recursos de AWS en la cuenta.

### **Modelo de Responsabilidad Compartida**
El modelo de seguridad de AWS que define la división de responsabilidades de seguridad entre AWS y el cliente.

---

## 📊 Monitoreo y Gestión

### **Amazon CloudWatch**
Un servicio de monitoreo y gestión que proporciona datos e información procesable para recursos y aplicaciones de AWS.

### **AWS Systems Manager**
Una colección de capacidades que te ayuda a automatizar tareas de gestión como recopilar inventario del sistema, aplicar parches del SO, crear imágenes del sistema y configurar sistemas operativos Windows y Linux.

### **AWS Trusted Advisor**
Un recurso en línea que proporciona orientación en tiempo real para ayudarte a aprovisionar tus recursos siguiendo las mejores prácticas de AWS para optimización de costos, seguridad, tolerancia a fallos y rendimiento.

### **AWS X-Ray**
Un servicio que recopila datos sobre solicitudes que sirve tu aplicación y proporciona herramientas que puedes usar para ver, filtrar y obtener información de esos datos.

### **Alarma**
Una característica de CloudWatch que observa una sola métrica y envía notificaciones cuando la métrica supera un umbral que especificas.

### **Panel de Control**
Una página de inicio personalizable en la consola de CloudWatch que puedes usar para monitorear tus recursos en una sola vista.

### **Grupo de Registros**
Un grupo de flujos de registros que comparten la misma retención, monitoreo y configuraciones de control de acceso en CloudWatch Logs.

### **Métrica**
Un conjunto de puntos de datos ordenados por tiempo publicados en CloudWatch. Representa una variable a monitorear a lo largo del tiempo.

---

## 💰 Términos de Facturación y Costos

### **AWS Budgets**
Un servicio que te permite establecer presupuestos personalizados de costo y uso que te alertan cuando excedes o se pronostica que excederás tus umbrales.

### **Reporte de Costo y Uso de AWS (CUR)**
Un servicio que proporciona datos completos de costo y uso para servicios de AWS, habilitando análisis detallado de costos de AWS.

### **AWS Cost Explorer**
Una herramienta que te permite ver y analizar tus costos y uso a lo largo del tiempo usando gráficos y tablas interactivos.

### **Calculadora de Precios de AWS**
Una herramienta de planificación basada en web que puedes usar para crear estimaciones para tus casos de uso de AWS.

### **Facturación Consolidada**
Una característica de facturación en AWS Organizations que te permite recibir una sola factura para múltiples cuentas de AWS.

### **Etiquetas de Asignación de Costos**
Etiquetas que asignas a recursos de AWS para organizar y rastrear tus costos. Las etiquetas aparecen en reportes de costos para ayudarte a categorizar gastos.

### **Nivel Gratuito**
Un programa que ofrece uso gratuito de ciertos servicios de AWS por 12 meses desde la creación de la cuenta, además de algunos servicios que siempre son gratuitos.

### **Precios Bajo Demanda**
Un modelo de precios donde pagas por capacidad de cómputo por hora o segundo sin compromisos a largo plazo o pagos iniciales.

### **Instancia Reservada (RI)**
Un modelo de precios que proporciona descuentos significativos (hasta 75%) comparado con precios Bajo Demanda a cambio de un compromiso de 1 o 3 años.

### **Planes de Ahorro**
Un modelo de precios flexible que proporciona ahorros significativos en el uso de AWS a cambio de un compromiso a una cantidad consistente de uso por un término de 1 o 3 años.

### **Instancia Spot**
Un modelo de precios que te permite solicitar capacidad de cómputo de Amazon EC2 de reserva por hasta 90% de descuento del precio Bajo Demanda.

### **Costo Total de Propiedad (TCO)**
Una estimación financiera que te ayuda a entender tanto los costos directos como indirectos de un producto o sistema durante todo su ciclo de vida.

---

## 🔗 Integración y Mensajería

### **Amazon API Gateway**
Un servicio completamente gestionado que facilita a los desarrolladores crear, publicar, mantener, monitorear y asegurar APIs a cualquier escala.

### **Amazon Kinesis**
Una plataforma para datos de streaming en AWS, ofreciendo servicios poderosos para facilitar la carga y análisis de datos de streaming.

### **Amazon SNS (Simple Notification Service)**
Un servicio de mensajería de publicación-suscripción que te permite desacoplar microservicios, sistemas distribuidos y aplicaciones sin servidor.

### **Amazon SQS (Simple Queue Service)**
Un servicio de cola de mensajes completamente gestionado que te permite desacoplar y escalar microservicios, sistemas distribuidos y aplicaciones sin servidor.

### **AWS Step Functions**
Un servicio de flujo de trabajo sin servidor que te permite coordinar múltiples servicios de AWS en flujos de trabajo sin servidor usando flujos de trabajo visuales.

### **Cola de Mensajes No Entregados**
Una cola a la que otras colas pueden dirigir mensajes que no pueden procesarse exitosamente, ayudando con el manejo de errores y depuración.

### **Arquitectura Dirigida por Eventos**
Un patrón de arquitectura donde los componentes se comunican a través de eventos, habilitando acoplamiento flexible y escalabilidad.

### **Cola FIFO**
Colas Primero en Entrar, Primero en Salir que preservan el orden exacto en el que los mensajes son enviados y recibidos, y aseguran procesamiento exactamente una vez.

### **Cola de Mensajes**
Un método de comunicación usado en sistemas de software para habilitar comunicación asíncrona entre diferentes componentes o servicios.

### **Publicación-Suscripción (Pub/Sub)**
Un patrón de mensajería donde los remitentes (publicadores) envían mensajes a múltiples receptores (suscriptores) sin saber quiénes son los suscriptores.

---

## 📱 Aplicaciones y Desarrollo

### **Amazon Cognito**
Un servicio que proporciona autenticación, autorización y gestión de usuarios para aplicaciones web y móviles.

### **Amazon SES (Simple Email Service)**
Un servicio rentable de envío de correos electrónicos que te permite enviar correos transaccionales, mensajes de marketing o cualquier otro tipo de contenido.

### **AWS CodeCommit**
Un servicio de control de código fuente completamente gestionado que aloja repositorios seguros basados en Git.

### **AWS CodeDeploy**
Un servicio de implementación que automatiza implementaciones de aplicaciones a instancias Amazon EC2, instancias locales o funciones Lambda sin servidor.

### **AWS CodePipeline**
Un servicio de integración continua y entrega continua para actualizaciones rápidas y confiables de aplicaciones e infraestructura.

### **Integración Continua (CI)**
Una práctica de desarrollo donde los desarrolladores integran código en un repositorio compartido frecuentemente, con cada integración verificada por construcción y pruebas automatizadas.

### **Implementación Continua (CD)**
Un enfoque de ingeniería de software donde los cambios de código se implementan automáticamente a producción después de pasar por fases de pruebas automatizadas.

### **DevOps**
Un conjunto de prácticas que combina desarrollo de software y operaciones de TI para acortar el ciclo de vida de desarrollo y proporcionar entrega continua.

### **Infraestructura como Código (IaC)**
La práctica de gestionar y aprovisionar infraestructura de cómputo a través de archivos de definición legibles por máquina, en lugar de configuración de hardware físico.

### **Microservicios**
Un enfoque arquitectónico donde las aplicaciones se construyen como una colección de servicios débilmente acoplados que pueden desarrollarse, implementarse y escalarse independientemente.

### **Sin Servidor**
Un modelo de computación en la nube donde el proveedor de nube gestiona la infraestructura, y los desarrolladores pueden enfocarse en escribir código sin gestionar servidores.

---

## 🔍 Términos Adicionales

### **Ancho de Banda**
La tasa máxima de transferencia de datos a través de una ruta dada, típicamente medida en bits por segundo (bps).

### **Caché**
Un componente de hardware o software que almacena datos temporalmente para servir solicitudes futuras más rápido.

### **Contenedor**
Un paquete ejecutable ligero, independiente que incluye todo lo necesario para ejecutar una aplicación: código, tiempo de ejecución, herramientas del sistema, bibliotecas y configuraciones.

### **Lago de Datos**
Un repositorio centralizado que te permite almacenar todos tus datos estructurados y no estructurados a cualquier escala.

### **Docker**
Una plataforma que usa contenedores para empaquetar aplicaciones y sus dependencias para implementación consistente a través de diferentes entornos.

### **Kubernetes**
Una plataforma de orquestación de contenedores de código abierto que automatiza la implementación, escalado y gestión de aplicaciones en contenedores.

### **Latencia**
El retraso de tiempo entre una solicitud y respuesta, típicamente medido en milisegundos (ms).

### **Balanceador de Carga**
Un dispositivo o servicio que distribuye tráfico de red o aplicación a través de múltiples servidores para asegurar alta disponibilidad y confiabilidad.

### **Rendimiento**
La cantidad de datos procesados o transmitidos en una cantidad dada de tiempo, típicamente medido en transacciones por segundo o solicitudes por segundo.

### **Máquina Virtual (VM)**
Una emulación basada en software de un sistema de computadora que proporciona la funcionalidad de una computadora física.

---

## 📚 Consejos de Estudio para el Glosario

### 🎯 Cómo Usar Este Glosario
1. **Revisión Regular**: Lee 10-15 términos diariamente durante tu período de estudio
2. **Aprendizaje Contextual**: No solo memorices - entiende cómo los términos se relacionan entre sí
3. **Aplicación Práctica**: Trata de usar estos términos cuando discutas conceptos de AWS
4. **Referencias Cruzadas**: Vincula términos de vuelta a los materiales de estudio principales

### 🔤 Referencia Rápida de Acrónimos
- **AWS**: Amazon Web Services
- **EC2**: Elastic Compute Cloud
- **S3**: Simple Storage Service
- **IAM**: Identity and Access Management
- **VPC**: Virtual Private Cloud
- **RDS**: Relational Database Service
- **CDN**: Content Delivery Network
- **DNS**: Domain Name System
- **API**: Application Programming Interface
- **SDK**: Software Development Kit
- **CLI**: Command Line Interface
- **SLA**: Service Level Agreement
- **SQS**: Simple Queue Service
- **SNS**: Simple Notification Service
- **EBS**: Elastic Block Store
- **EFS**: Elastic File System
- **ELB**: Elastic Load Balancer
- **ACL**: Access Control List
- **MFA**: Multi-Factor Authentication
- **DDoS**: Distributed Denial of Service
- **SSL/TLS**: Secure Sockets Layer/Transport Layer Security
- **HTTPS**: Hypertext Transfer Protocol Secure

---

> **¡Felicidades!** Has completado el Glosario AWS Cloud Practitioner. Este recurso integral te ayudará durante tu preparación para el examen y como referencia futura en tu carrera con AWS.
>
> **Próximo paso**: Revisa los [Consejos de Examen](./exam-tips.md) y practica con los [Exámenes de Práctica](../practice-exams/) para solidificar tu conocimiento.

**[⬅️ Volver a Referencia Rápida](./README.md)** | **[🏠 Inicio](../README.md)**

*Use this glossary as your quick reference guide throughout your AWS certification journey! 📖*
