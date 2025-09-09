# 🚀 Hoja de Referencia Rápida de Servicios de AWS

> **Servicios esenciales de AWS de un vistazo para el examen Cloud Practitioner**

## 📋 Tabla de Contenidos

- [💻 Servicios de Cómputo](#-servicios-de-cómputo)
- [💾 Servicios de Almacenamiento](#-servicios-de-almacenamiento)
- [🌐 Redes y Entrega de Contenido](#-redes-y-entrega-de-contenido)
- [🗄️ Servicios de Base de Datos](#️-servicios-de-base-de-datos)
- [🔒 Servicios de Seguridad e Identidad](#-servicios-de-seguridad-e-identidad)
- [📊 Gestión y Monitoreo](#-gestión-y-monitoreo)
- [🔗 Integración y Mensajería](#-integración-y-mensajería)
- [📱 Servicios de Aplicaciones](#-servicios-de-aplicaciones)
- [💰 Facturación y Gestión de Costos](#-facturación-y-gestión-de-costos)
- [🎯 Matriz de Decisión Rápida](#-matriz-de-decisión-rápida)

---

## 💻 Servicios de Cómputo

### Amazon EC2 (Elastic Compute Cloud)
- **Qué es**: Servidores virtuales en la nube
- **Cuándo usar**: Cuando necesitas máquinas virtuales con control total
- **Características clave**: Múltiples tipos de instancia, auto escalado, varios modelos de precios
- **Precios**: On-Demand, Reservadas, Spot, Dedicadas
- **Consejo de examen**: Recuerda las diferentes familias de instancias (Propósito general, Optimizadas para cómputo, Optimizadas para memoria, Optimizadas para almacenamiento)

### AWS Lambda
- **Qué es**: Servicio de cómputo sin servidor
- **Cuándo usar**: Aplicaciones basadas en eventos, funciones de corta duración
- **Características clave**: Sin gestión de servidores, escalado automático, pago por ejecución
- **Límites**: Tiempo máximo de ejecución de 15 minutos, memoria hasta 10GB
- **Consejo de examen**: Ideal para microservicios y procesamiento de eventos

### Amazon ECS (Elastic Container Service)
- **Qué es**: Servicio de orquestación de contenedores
- **Cuándo usar**: Ejecutar contenedores Docker a escala
- **Características clave**: Se integra con servicios de AWS, soporta Fargate para contenedores sin servidor
- **Consejo de examen**: ECS con Fargate = contenedores sin servidor

### Amazon EKS (Elastic Kubernetes Service)
- **Qué es**: Servicio gestionado de Kubernetes
- **Cuándo usar**: Cuando necesitas orquestación de Kubernetes
- **Características clave**: Plano de control de Kubernetes completamente gestionado
- **Consejo de examen**: Usar cuando ya conoces Kubernetes

### AWS Batch
- **Qué es**: Servicio de cómputo por lotes
- **Cuándo usar**: Ejecutar trabajos por lotes a cualquier escala
- **Características clave**: Aprovisionamiento automático, colas de trabajos, optimización de costos
- **Consejo de examen**: Para cargas de trabajo de procesamiento por lotes de larga duración

### AWS Elastic Beanstalk
- **Qué es**: Plataforma como Servicio para aplicaciones web
- **Cuándo usar**: Despliegue rápido sin gestión de infraestructura
- **Características clave**: Soporta múltiples lenguajes de programación, escalado automático
- **Consejo de examen**: Sube código y ejecuta - AWS maneja el resto

---

## 💾 Servicios de Almacenamiento

### Amazon S3 (Simple Storage Service)
- **Qué es**: Servicio de almacenamiento de objetos
- **Cuándo usar**: Almacenar cualquier tipo de datos - sitios web, respaldos, archivos
- **Clases de almacenamiento**:
  - **Standard**: Datos accedidos frecuentemente
  - **Standard-IA**: Datos accedidos infrecuentemente
  - **One Zone-IA**: Menor costo para datos accedidos infrecuentemente
  - **Glacier**: Archivo a largo plazo
  - **Glacier Deep Archive**: Archivo de menor costo
  - **Intelligent Tiering**: Optimización automática
- **Características clave**: 99.999999999% (11 9's) durabilidad, almacenamiento ilimitado
- **Consejo de examen**: Conoce cuándo usar cada clase de almacenamiento

### Amazon EBS (Elastic Block Store)
- **Qué es**: Almacenamiento de bloques para instancias EC2
- **Cuándo usar**: Almacenamiento persistente para instancias EC2
- **Tipos de volúmenes**:
  - **gp3/gp2**: SSD de propósito general
  - **io2/io1**: SSD de IOPS aprovisionadas (alto rendimiento)
  - **st1**: HDD optimizado para rendimiento
  - **sc1**: HDD frío (menor costo)
- **Características clave**: Persistente, puede ser desconectado y reconectado
- **Consejo de examen**: EBS persiste más allá del ciclo de vida de la instancia

### Amazon EFS (Elastic File System)
- **Qué es**: Sistema de archivos NFS gestionado
- **Cuándo usar**: Almacenamiento de archivos compartido entre múltiples instancias EC2
- **Características clave**: Escala automáticamente, acceso concurrente
- **Consejo de examen**: Usar cuando múltiples instancias necesitan acceso a archivos compartidos

### AWS Storage Gateway
- **Qué es**: Servicio de almacenamiento híbrido en la nube
- **Cuándo usar**: Conectar on-premises con almacenamiento de AWS
- **Tipos**: File Gateway, Volume Gateway, Tape Gateway
- **Consejo de examen**: Puente entre almacenamiento on-premises y en la nube

---

## 🌐 Redes y Entrega de Contenido

### Amazon VPC (Virtual Private Cloud)
- **Qué es**: Red virtual aislada en AWS
- **Cuándo usar**: Crear ambientes de red aislados
- **Componentes**: Subredes, Tablas de Rutas, Internet Gateways, NAT Gateways
- **Características clave**: Control completo sobre la configuración de red
- **Consejo de examen**: Base para la mayoría de arquitecturas de AWS

### Amazon CloudFront
- **Qué es**: Red de Entrega de Contenido (CDN)
- **Cuándo usar**: Entregar contenido globalmente con baja latencia
- **Características clave**: Ubicaciones edge mundiales, almacena contenido cerca de los usuarios
- **Consejo de examen**: Reduce latencia sirviendo contenido desde ubicaciones edge

### Elastic Load Balancing (ELB)
- **Qué es**: Distribuye tráfico entrante entre múltiples objetivos
- **Tipos**:
  - **Application Load Balancer (ALB)**: Capa 7, HTTP/HTTPS
  - **Network Load Balancer (NLB)**: Capa 4, TCP/UDP
  - **Classic Load Balancer**: Legado, Capa 4 y 7
- **Consejo de examen**: ALB para aplicaciones web, NLB para alto rendimiento

### Amazon Route 53
- **Qué es**: Servicio web DNS
- **Cuándo usar**: Resolución de nombres de dominio, verificaciones de salud, enrutamiento
- **Características clave**: DNS global, verificaciones de salud, múltiples políticas de enrutamiento
- **Consejo de examen**: Más que solo DNS - incluye monitoreo de salud

### AWS Direct Connect
- **Qué es**: Conexión de red dedicada a AWS
- **Cuándo usar**: Rendimiento de red consistente, transferencias de datos grandes
- **Características clave**: Ancho de banda predecible, costos de red reducidos
- **Consejo de examen**: Alternativa a VPN para conectividad dedicada

---

## 🗄️ Servicios de Base de Datos

### Amazon RDS (Relational Database Service)
- **Qué es**: Servicio de base de datos relacional gestionado
- **Motores soportados**: MySQL, PostgreSQL, MariaDB, Oracle, SQL Server, Aurora
- **Cuándo usar**: Necesidades tradicionales de base de datos relacional
- **Características clave**: Respaldos automatizados, parches, escalado
- **Consejo de examen**: AWS gestiona la infraestructura, tú gestionas datos y consultas

### Amazon Aurora
- **Qué es**: Base de datos relacional nativa de la nube
- **Cuándo usar**: Necesidades de base de datos relacional de alto rendimiento
- **Características clave**: Compatible con MySQL/PostgreSQL, almacenamiento de auto-escalado
- **Consejo de examen**: Motor de base de datos de alto rendimiento de AWS

### Amazon DynamoDB
- **Qué es**: Servicio de base de datos NoSQL
- **Cuándo usar**: Aplicaciones de gran escala, necesita latencia de milisegundos de un dígito
- **Características clave**: Sin servidor, escalado automático, tablas globales
- **Consejo de examen**: Ideal para aplicaciones móviles, web y de juegos

### Amazon Redshift
- **Qué es**: Servicio de almacén de datos
- **Cuándo usar**: Inteligencia de negocios y análisis
- **Características clave**: Almacenamiento columnar, procesamiento paralelo, escala de petabytes
- **Consejo de examen**: Para análisis y almacenamiento de datos, no bases de datos operacionales

### Amazon ElastiCache
- **Qué es**: Servicio de caché en memoria
- **Cuándo usar**: Mejorar el rendimiento de aplicaciones con caché
- **Motores**: Redis, Memcached
- **Consejo de examen**: Usar para acelerar consultas de base de datos y rendimiento de aplicaciones

---

## 🔒 Servicios de Seguridad e Identidad

### AWS IAM (Identity and Access Management)
- **Qué es**: Servicio de autenticación y autorización
- **Componentes**: Usuarios, Grupos, Roles, Políticas
- **Principios clave**: Menor privilegio, usar roles para aplicaciones
- **Consejo de examen**: Base de la seguridad de AWS

### AWS Organizations
- **Qué es**: Servicio de gestión de cuentas
- **Cuándo usar**: Gestionar múltiples cuentas de AWS
- **Características clave**: Facturación consolidada, Políticas de Control de Servicios (SCPs)
- **Consejo de examen**: Gestión central para ambientes de múltiples cuentas

### AWS CloudTrail
- **Qué es**: Servicio de registro y auditoría de API
- **Cuándo usar**: Cumplimiento, análisis de seguridad, solución de problemas
- **Características clave**: Registra todas las llamadas API, se integra con CloudWatch
- **Consejo de examen**: Esencial para auditoría de seguridad

### AWS Config
- **Qué es**: Servicio de monitoreo de configuración y cumplimiento
- **Cuándo usar**: Rastrear configuraciones de recursos y cumplimiento
- **Características clave**: Historial de configuración, reglas de cumplimiento
- **Consejo de examen**: Monitorea "qué" cambió, CloudTrail monitorea "quién" lo cambió

### AWS GuardDuty
- **Qué es**: Servicio de detección de amenazas
- **Cuándo usar**: Detección automatizada de amenazas de seguridad
- **Características clave**: Detección de amenazas basada en aprendizaje automático
- **Consejo de examen**: Usa ML para detectar comportamiento anómalo

### AWS Inspector
- **Qué es**: Servicio de evaluación de seguridad
- **Cuándo usar**: Encontrar vulnerabilidades en instancias EC2 e imágenes de contenedores
- **Características clave**: Evaluaciones de seguridad automatizadas
- **Consejo de examen**: Se enfoca en vulnerabilidades de seguridad de aplicaciones

### AWS WAF (Web Application Firewall)
- **Qué es**: Servicio de protección de aplicaciones web
- **Cuándo usar**: Proteger aplicaciones web de exploits
- **Características clave**: Protección contra inyección SQL, protección XSS
- **Consejo de examen**: Protección de Capa 7 para aplicaciones web

### AWS Shield
- **Qué es**: Servicio de protección DDoS
- **Niveles**: Standard (gratis), Advanced (pagado)
- **Cuándo usar**: Proteger contra ataques DDoS
- **Consejo de examen**: Standard viene gratis con CloudFront y Route 53

---

## 📊 Gestión y Monitoreo

### Amazon CloudWatch
- **Qué es**: Servicio de monitoreo y registro
- **Cuándo usar**: Monitorear recursos y aplicaciones de AWS
- **Características clave**: Métricas, registros, alarmas, paneles
- **Consejo de examen**: Centro de monitoreo central para AWS

### AWS Systems Manager
- **Qué es**: Servicio de gestión operacional
- **Cuándo usar**: Gestionar instancias EC2 y servidores on-premises
- **Características clave**: Gestión de parches, gestión de configuración
- **Consejo de examen**: Gestiona infraestructura tanto en la nube como on-premises

### AWS CloudFormation
- **Qué es**: Servicio de Infraestructura como Código
- **Cuándo usar**: Desplegar infraestructura usando plantillas
- **Características clave**: Plantillas JSON/YAML, gestión de stacks
- **Consejo de examen**: Forma declarativa de aprovisionar recursos de AWS

### AWS X-Ray
- **Qué es**: Monitoreo de rendimiento de aplicaciones
- **Cuándo usar**: Rastrear solicitudes en aplicaciones distribuidas
- **Características clave**: Rastreo de solicitudes, análisis de rendimiento
- **Consejo de examen**: Ayuda a identificar cuellos de botella en microservicios

---

## 🔗 Integración y Mensajería

### Amazon SQS (Simple Queue Service)
- **Qué es**: Servicio de colas de mensajes
- **Cuándo usar**: Desacoplar componentes de aplicaciones
- **Tipos**: Standard (al menos una vez), FIFO (exactamente una vez, ordenado)
- **Consejo de examen**: Usar para comunicación asíncrona entre servicios

### Amazon SNS (Simple Notification Service)
- **Qué es**: Servicio de mensajería publicar-suscribir
- **Cuándo usar**: Enviar notificaciones a múltiples suscriptores
- **Características clave**: Múltiples métodos de entrega (email, SMS, HTTP, SQS)
- **Consejo de examen**: Patrón de mensajería fan-out

### Amazon Kinesis
- **Qué es**: Servicio de streaming de datos en tiempo real
- **Cuándo usar**: Procesar datos de streaming en tiempo real
- **Componentes**: Data Streams, Data Firehose, Analytics
- **Consejo de examen**: Para procesamiento y análisis de datos en tiempo real

### AWS Step Functions
- **Qué es**: Orquestación de flujos de trabajo sin servidor
- **Cuándo usar**: Coordinar múltiples servicios de AWS en flujos de trabajo
- **Características clave**: Flujos de trabajo visuales, manejo de errores
- **Consejo de examen**: Orquesta aplicaciones sin servidor

---

## 📱 Servicios de Aplicaciones

### Amazon API Gateway
- **Qué es**: Servicio de gestión de API
- **Cuándo usar**: Crear, desplegar y gestionar APIs
- **Características clave**: APIs REST/WebSocket, limitación de velocidad, autorización
- **Consejo de examen**: Puerta de entrada para aplicaciones sin servidor

### Amazon SES (Simple Email Service)
- **Qué es**: Servicio de envío de emails
- **Cuándo usar**: Enviar emails transaccionales o de marketing
- **Características clave**: Alta entregabilidad, costo-efectivo
- **Consejo de examen**: Para emails generados por aplicaciones

### Amazon Cognito
- **Qué es**: Servicio de autenticación y autorización de usuarios
- **Cuándo usar**: Gestión de usuarios para aplicaciones móviles y web
- **Características clave**: Grupos de usuarios, grupos de identidad, inicio de sesión social
- **Consejo de examen**: Para autenticación de aplicaciones orientadas al cliente

---

## 💰 Facturación y Gestión de Costos

### AWS Cost Explorer
- **Qué es**: Herramienta de visualización y análisis de costos
- **Cuándo usar**: Entender y analizar costos de AWS
- **Características clave**: Datos históricos, pronósticos, recomendaciones
- **Consejo de examen**: Herramienta principal para análisis de costos

### AWS Budgets
- **Qué es**: Servicio de presupuestos de costos y uso
- **Cuándo usar**: Establecer límites de gasto y alertas
- **Características clave**: Presupuestos personalizados, alertas automatizadas
- **Consejo de examen**: Gestión proactiva de costos

### AWS Cost and Usage Report (CUR)
- **Qué es**: Exportación detallada de datos de facturación
- **Cuándo usar**: Análisis detallado de costos con herramientas externas
- **Características clave**: Datos de facturación integrales, análisis personalizado
- **Consejo de examen**: Datos de facturación más detallados disponibles

### AWS Trusted Advisor
- **Qué es**: Servicio de recomendaciones de mejores prácticas
- **Categorías**: Optimización de costos, rendimiento, seguridad, tolerancia a fallos
- **Niveles**: Basic (7 verificaciones), Completo (soporte Business/Enterprise)
- **Consejo de examen**: Proporciona recomendaciones de optimización

---

## 🎯 Matriz de Decisión Rápida

### Elegir el Servicio de Cómputo Correcto
| Necesidad | Servicio | Por qué |
|------|---------|-----|
| Máquinas virtuales | EC2 | Control total sobre instancias |
| Funciones sin servidor | Lambda | Basado en eventos, sin gestión de servidores |
| Orquestación de contenedores | ECS/EKS | Gestión escalable de contenedores |
| Despliegue rápido de app web | Elastic Beanstalk | PaaS, solo sube código |
| Procesamiento por lotes | Batch | Optimizado para cargas de trabajo por lotes |

### Elegir el Servicio de Almacenamiento Correcto
| Necesidad | Servicio | Por qué |
|------|---------|-----|
| Almacenamiento de objetos | S3 | Ilimitado, altamente duradero |
| Almacenamiento de bloques para EC2 | EBS | Persistente, alto rendimiento |
| Almacenamiento de archivos compartido | EFS | Acceso multi-instancia |
| Almacenamiento de archivo | S3 Glacier | Menor costo para archivos |

### Elegir el Servicio de Base de Datos Correcto
| Necesidad | Servicio | Por qué |
|------|---------|-----|
| Base de datos relacional | RDS | Bases de datos SQL gestionadas |
| Relacional de alto rendimiento | Aurora | Nativo de la nube, auto-escalado |
| Base de datos NoSQL | DynamoDB | Sin servidor, latencia de un dígito |
| Almacén de datos | Redshift | Análisis e BI |
| Caché | ElastiCache | Rendimiento en memoria |

### Elegir el Servicio de Seguridad Correcto
| Necesidad | Servicio | Por qué |
|------|---------|-----|
| Gestión de identidad | IAM | Usuarios, roles, permisos |
| Registro de API | CloudTrail | Rastro de auditoría de llamadas API |
| Monitoreo de configuración | Config | Rastrear configuraciones de recursos |
| Detección de amenazas | GuardDuty | Monitoreo de seguridad basado en ML |
| Protección de app web | WAF | Firewall de capa de aplicación |
| Protección DDoS | Shield | Protección de capa de red/transporte |

---

## 📚 Consejos de Examen

### 🎯 Estrategia de Selección de Servicios
1. **Identifica el caso de uso** - ¿Cuál es la necesidad del negocio?
2. **Considera el nivel de gestión** - ¿Cuánta gestión quieres?
3. **Piensa en la escala** - Requisitos actuales y futuros
4. **Considera el costo** - Optimiza para el modelo de precios apropiado

### 🔑 Relaciones Clave para Recordar
- **EC2 + EBS**: Máquinas virtuales con almacenamiento persistente
- **S3 + CloudFront**: Entrega global de contenido
- **VPC + Subredes**: Aislamiento y segmentación de red
- **ALB + Auto Scaling**: Alta disponibilidad y elasticidad
- **Lambda + API Gateway**: APIs web sin servidor
- **RDS + Read Replicas**: Escalado de base de datos
- **CloudTrail + CloudWatch**: Monitoreo de seguridad
- **IAM + Organizations**: Gestión de identidad y cuentas

### ⚠️ Trampas Comunes del Examen
- No confundas **CloudWatch** (monitoreo) con **CloudTrail** (registro de API)
- Recuerda **S3** es almacenamiento de objetos, **EBS** es almacenamiento de bloques
- **Lambda** tiene límites de tiempo (15 minutos máximo)
- **DynamoDB** es NoSQL, **RDS** es SQL
- **Security Groups** son con estado, **NACLs** son sin estado

---

## 🚀 Enlaces de Referencia Rápida

- 🏠 [Guía de Estudio Principal](../README.md)
- 🌩️ [Dominio 1: Conceptos de Nube](../01-cloud-concepts/README.md)
- 🔒 [Dominio 2: Seguridad y Cumplimiento](../02-security-compliance/README.md)
- ⚙️ [Dominio 3: Tecnología y Servicios](../03-technology-services/README.md)
- 💰 [Dominio 4: Facturación y Soporte](../04-billing-support/README.md)
- 📝 [Exámenes de Práctica](../practice-exams/)
- 🎯 [Consejos de Examen](exam-tips.md)
- 📖 [Glosario](glossary.md)

---

*¡Usa esta hoja de referencia para revisión rápida antes de tu examen! 🎯*
