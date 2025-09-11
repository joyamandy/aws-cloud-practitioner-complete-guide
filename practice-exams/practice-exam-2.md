# 📝 Examen de Práctica 2 - AWS Cloud Practitioner

> **Examen de práctica avanzado con preguntas basadas en escenarios y casos límite**

## 📋 Instrucciones del Examen

- **Límite de Tiempo**: 90 minutos (recomendado)
- **Preguntas**: 65 de opción múltiple y respuesta múltiple
- **Puntuación para Aprobar**: 70% (46 de 65 preguntas)
- **Distribución por Dominio**: Refleja las ponderaciones del examen real
- **Formato**: Elige la MEJOR respuesta para cada pregunta
- **Dificultad**: Preguntas de nivel intermedio a avanzado

### 📊 Distribución de Preguntas por Dominio
- **Dominio 1 (Conceptos de la Nube)**: 16 preguntas (24%)
- **Dominio 2 (Seguridad y Cumplimiento)**: 20 preguntas (30%)
- **Dominio 3 (Tecnología y Servicios)**: 22 preguntas (34%)
- **Dominio 4 (Facturación y Soporte)**: 7 preguntas (12%)

---

## 🌩️ Dominio 1: Conceptos de la Nube (Preguntas 1-16)

### Pregunta 1
**Una empresa se está mudando de su centro de datos local a AWS. Quieren asegurar que sus aplicaciones puedan manejar automáticamente cargas variables sin intervención manual. ¿Qué característica de la computación en la nube describe mejor esta capacidad?**

- A) Autoservicio bajo demanda
- B) Acceso amplio a la red
- C) Elasticidad rápida
- D) Agrupación de recursos

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: La elasticidad rápida permite que los recursos escalen automáticamente basándose en la demanda sin intervención manual. Esto permite que las aplicaciones manejen cargas variables sin problemas.
</details>

### Pregunta 2
**Una empresa startup necesita implementar una aplicación web rápidamente pero tiene capital limitado para inversiones iniciales en infraestructura. ¿Qué ventaja de la computación en la nube es más relevante para su situación?**

- A) Mayor velocidad y agilidad
- B) Dejar de gastar dinero ejecutando y manteniendo centros de datos
- C) Intercambiar gastos de capital por gastos operativos
- D) Volverse global en minutos

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Para una startup con capital limitado, la capacidad de intercambiar gastos de capital (CAPEX) por gastos operativos (OPEX) es la ventaja más relevante, ya que elimina la necesidad de grandes inversiones iniciales en infraestructura.
</details>

### Pregunta 3
**Una organización de salud necesita mantener los datos de pacientes en sus instalaciones debido a requisitos regulatorios, pero quiere usar servicios en la nube para análisis de datos. ¿Qué modelo de implementación deberían considerar?**

- A) Nube pública
- B) Nube privada
- C) Nube híbrida
- D) Nube comunitaria

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Una implementación de nube híbrida permite a la organización mantener datos sensibles de pacientes en sus instalaciones mientras aprovecha los servicios en la nube para análisis, combinando requisitos de cumplimiento con beneficios de la nube.
</details>

### Pregunta 4
**¿Cuál escenario ilustra mejor la ventaja de "Dejar de adivinar la capacidad" de la computación en la nube?**

- A) Una empresa aprovisiona exactamente la cantidad correcta de recursos basándose en patrones de uso reales
- B) Una empresa compra servidores que pueden manejar la carga pico, resultando en 70% de capacidad inactiva la mayor parte del tiempo
- C) Una empresa agrega servidores manualmente cuando el tráfico aumenta
- D) Una empresa usa la misma cantidad de recursos independientemente de la demanda

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: A**

**Explicación**: La computación en la nube elimina la necesidad de adivinar los requisitos de capacidad. En lugar de sobre-aprovisionar (opción B), puedes aprovisionar basándote en el uso real y escalar automáticamente.
</details>

### Pregunta 5
**Una aplicación requiere la menor latencia posible para usuarios en múltiples continentes. ¿Qué componente de infraestructura de AWS sería más efectivo?**

- A) Múltiples Regiones de AWS
- B) Múltiples Zonas de Disponibilidad
- C) Edge Locations
- D) Local Zones

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Las Edge Locations están más cerca de los usuarios finales y proporcionan la menor latencia para entrega de contenido a través de servicios como CloudFront. Están específicamente diseñadas para minimizar la latencia globalmente.
</details>

### Pregunta 6
**Una empresa quiere usar servicios en la nube pero mantener control completo sobre la infraestructura subyacente, incluyendo el hipervisor. ¿Qué modelo de servicio deberían elegir?**

- A) Software como Servicio (SaaS)
- B) Plataforma como Servicio (PaaS)
- C) Infraestructura como Servicio (IaaS)
- D) Función como Servicio (FaaS)

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: IaaS proporciona el mayor control sobre la infraestructura, incluyendo sistemas operativos y middleware. Sin embargo, nota que incluso en IaaS, los clientes no controlan el hipervisor - AWS gestiona esa capa.
</details>

### Pregunta 7
**¿Cuál de las siguientes opciones demuestra mejor la ventaja de "Economías de escala" de AWS?**

- A) AWS transfiere ahorros de compras por volumen a los clientes a través de precios más bajos
- B) AWS permite desplegar globalmente
- C) AWS proporciona escalado automático
- D) AWS elimina costos iniciales

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: A**

**Explicación**: Las economías de escala significan que AWS puede lograr costos más bajos debido a su poder de compra masivo y eficiencia operacional, y transfieren estos ahorros a los clientes a través de precios más bajos.
</details>

### Pregunta 8
**Una empresa está evaluando diferentes enfoques para recuperación ante desastres. Quieren entender cómo el diseño de infraestructura de AWS soporta alta disponibilidad. ¿Cuál es el beneficio principal de las Zonas de Disponibilidad de AWS?**

- A) Proporcionan diferentes modelos de precios
- B) Están aisladas de fallas en otras Zonas de Disponibilidad
- C) Ofrecen diferentes servicios
- D) Proporcionan conexiones de internet más rápidas

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Las Zonas de Disponibilidad están diseñadas para estar aisladas de fallas en otras AZ dentro de la misma Región, proporcionando tolerancia a fallas y alta disponibilidad para aplicaciones desplegadas en múltiples AZ.
</details>

### Pregunta 9
**¿Cuál de los siguientes escenarios se beneficiaría MÁS del escalado vertical en lugar del escalado horizontal?**

- A) Una aplicación web con picos de tráfico impredecibles
- B) Una base de datos que requiere más memoria y CPU para consultas complejas
- C) Una arquitectura de microservicios con componentes independientes
- D) Un sistema de entrega de contenido sirviendo usuarios globales

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: El escalado vertical (escalar hacia arriba) es a menudo mejor para bases de datos que necesitan recursos más potentes (CPU, memoria) para manejar consultas complejas, mientras que el escalado horizontal funciona mejor para aplicaciones distribuidas.
</details>

### Pregunta 10
**Una empresa de servicios financieros necesita asegurar que su infraestructura de AWS cumpla con requisitos regulatorios estrictos para residencia de datos. ¿Qué característica de infraestructura de AWS aborda esta preocupación?**

- A) Las Edge Locations cumplen automáticamente con todas las regulaciones
- B) Los datos en las Regiones de AWS permanecen dentro de los límites geográficos a menos que se muevan explícitamente
- C) AWS replica automáticamente datos globalmente para cumplimiento
- D) Todos los servicios de AWS son compatibles por defecto

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS asegura que los datos almacenados en una Región permanezcan dentro de los límites geográficos de esa Región a menos que el cliente configure explícitamente que se muevan, ayudando a cumplir requisitos de residencia de datos.
</details>

### Pregunta 11
**¿Cuál de las siguientes es un ejemplo de AWS proporcionando "Mayor velocidad y agilidad"?**

- A) Costos más bajos comparados con instalaciones locales
- B) La capacidad de aprovisionar recursos en minutos en lugar de semanas
- C) Actualizaciones de seguridad automáticas
- D) Presencia global

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Mayor velocidad y agilidad se refiere a la capacidad de aprovisionar y desplegar recursos rápidamente (minutos vs. semanas/meses para infraestructura tradicional), habilitando innovación más rápida y tiempo al mercado.
</details>

### Pregunta 12
**Una empresa tiene aplicaciones que necesitan comunicarse con muy baja latencia dentro de la misma área geográfica. ¿Qué componente de infraestructura de AWS es más apropiado?**

- A) Múltiples Regiones
- B) Múltiples Zonas de Disponibilidad dentro de la misma Región
- C) Edge Locations
- D) Distribución CloudFront

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Múltiples Zonas de Disponibilidad dentro de la misma Región proporcionan comunicación de baja latencia (típicamente latencia de milisegundos de un solo dígito) mientras aún proporcionan tolerancia a fallas.
</details>

### Pregunta 13
**¿Qué característica de la computación en la nube permite a los clientes acceder a servicios a través de mecanismos estándar y plataformas (teléfonos móviles, tablets, laptops)?**

- A) Agrupación de recursos
- B) Servicio medido
- C) Acceso amplio a la red
- D) Autoservicio bajo demanda

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: El acceso amplio a la red significa que los servicios están disponibles a través de la red mediante mecanismos estándar y pueden ser accedidos por varias plataformas cliente y dispositivos.
</details>

### Pregunta 14
**Una empresa quiere entender el costo total de propiedad (TCO) al migrar a AWS. ¿Qué costos típicamente se reducen al moverse de instalaciones locales a la nube? (Selecciona DOS)**

- A) Costos de licencias de software
- B) Costos de instalaciones del centro de datos
- C) Costos de capacitación del personal
- D) Costos de mantenimiento de hardware
- E) Costos de ancho de banda de red

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B, D**

**Explicación**: Moverse a la nube típicamente reduce costos de instalaciones del centro de datos (renta, energía, enfriamiento) y costos de mantenimiento de hardware (AWS gestiona la infraestructura). Las licencias de software y capacitación del personal pueden aumentar, y los costos de red varían.
</details>

### Pregunta 15
**¿Cuál es la principal diferencia entre AWS Local Zones y AWS Wavelength?**

- A) Local Zones son para aplicaciones móviles, Wavelength es para aplicaciones web
- B) Local Zones acercan servicios de AWS a los usuarios, Wavelength lleva servicios al borde de redes de telecomunicaciones
- C) Local Zones son gratuitas, Wavelength requiere pago
- D) No hay diferencia entre ellas

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Local Zones acercan servicios de AWS a usuarios finales en áreas geográficas específicas, mientras que las zonas Wavelength están ubicadas en el borde de redes 5G de proveedores de telecomunicaciones para aplicaciones de ultra-baja latencia.
</details>

### Pregunta 16
**¿Cuál de las siguientes opciones describe mejor el enfoque del modelo de computación en la nube para planificación de capacidad?**

- A) Planificar para capacidad pico y mantenerla constantemente
- B) Planificar para capacidad promedio y aceptar interrupciones ocasionales
- C) Comenzar con capacidad mínima y escalar basándose en demanda real
- D) Planificar para el doble de la capacidad pico esperada

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: La computación en la nube permite comenzar con capacidad mínima y escalar hacia arriba o abajo basándose en demanda real, eliminando la necesidad de sobre-aprovisionar o arriesgar sub-aprovisionar.
</details>

---

## 🔒 Dominio 2: Seguridad y Cumplimiento (Preguntas 17-36)

### Pregunta 17
**El equipo de seguridad de una empresa quiere asegurar que las llamadas API a servicios de AWS sean registradas y puedan ser auditadas. Los registros deben incluir quién hizo la llamada, cuándo se hizo y qué acciones se realizaron. ¿Qué servicio de AWS deberían implementar?**

- A) AWS Config
- B) AWS CloudWatch
- C) AWS CloudTrail
- D) AWS X-Ray

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: AWS CloudTrail proporciona registro detallado de llamadas API, incluyendo la identidad del llamador, el tiempo de la llamada, dirección IP de origen, parámetros de solicitud y elementos de respuesta.
</details>

### Pregunta 18
**Según el Modelo de Responsabilidad Compartida de AWS, ¿quién es responsable de parchear el sistema operativo de una instancia Amazon EC2?**

- A) AWS es siempre responsable
- B) El cliente es siempre responsable
- C) AWS para Windows, cliente para Linux
- D) Compartido entre AWS y el cliente

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Para instancias EC2, los clientes son responsables de parchear el sistema operativo invitado y cualquier aplicación ejecutándose en las instancias, independientemente del tipo de SO.
</details>

### Pregunta 19
**Un equipo de desarrollo necesita proporcionar acceso temporal a recursos de AWS para un contratista que trabajará en un proyecto por 3 meses. ¿Cuál es el enfoque MÁS seguro?**

- A) Crear un usuario IAM con credenciales permanentes y eliminarlo después de 3 meses
- B) Compartir las credenciales de la cuenta root
- C) Crear un rol IAM que pueda ser asumido con credenciales temporales
- D) Darles acceso a la cuenta de otro empleado

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Los roles IAM proporcionan credenciales temporales y son el enfoque más seguro para acceso temporal. Expiran automáticamente y pueden ser revocados fácilmente sin afectar credenciales permanentes.
</details>

### Pregunta 20
**Una empresa quiere asegurar que sus buckets S3 no sean accidentalmente hechos públicos. ¿Qué servicio de AWS puede ayudarles a monitorear continuamente y alertar sobre configuraciones de recursos?**

- A) AWS CloudTrail
- B) AWS Config
- C) AWS CloudWatch
- D) AWS Inspector

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS Config monitorea continuamente las configuraciones de recursos y puede alertar cuando los recursos se desvían de las configuraciones deseadas, como buckets S3 que se vuelven públicos.
</details>

### Pregunta 21
**Una organización tiene múltiples cuentas de AWS y quiere gestionar centralmente políticas de seguridad en todas las cuentas. ¿Qué servicio deberían usar?**

- A) AWS IAM
- B) AWS Organizations con Service Control Policies (SCPs)
- C) AWS Config
- D) AWS CloudFormation

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS Organizations con Service Control Policies (SCPs) permite gestión centralizada de permisos en múltiples cuentas de AWS, proporcionando barreras de protección para qué acciones pueden ser realizadas.
</details>

### Pregunta 22
**Una aplicación web está experimentando un ataque DDoS. ¿Qué servicios de AWS pueden ayudar a mitigar este ataque? (Selecciona DOS)**

- A) AWS WAF
- B) AWS Shield
- C) AWS CloudTrail
- D) AWS Config
- E) AWS X-Ray

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: A, B**

**Explicación**: AWS Shield proporciona protección DDoS (Standard es automático, Advanced proporciona protección mejorada), y AWS WAF puede filtrar tráfico web malicioso que podría ser parte de un ataque DDoS.
</details>

### Pregunta 23
**¿Cuál es el propósito principal de la Autenticación Multi-Factor (MFA) en AWS?**

- A) Cifrar datos en tránsito
- B) Proporcionar una capa adicional de seguridad más allá de las contraseñas
- C) Monitorear actividad del usuario
- D) Gestionar permisos de usuario

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: MFA proporciona una capa adicional de seguridad requiriendo que los usuarios proporcionen dos o más factores de verificación, haciendo mucho más difícil para usuarios no autorizados obtener acceso incluso si las contraseñas están comprometidas.
</details>

### Pregunta 24
**Una empresa necesita asegurar que su infraestructura de AWS cumpla con requisitos PCI DSS para manejar datos de tarjetas de crédito. ¿Qué deberían hacer?**

- A) AWS automáticamente hace todos los servicios compatibles con PCI DSS
- B) Usar solo servicios de AWS compatibles con PCI DSS e implementar configuraciones apropiadas
- C) El cumplimiento PCI DSS no es posible en AWS
- D) Solo usar infraestructura local para cumplimiento PCI DSS

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS ofrece servicios compatibles con PCI DSS, pero los clientes deben usar estos servicios apropiadamente e implementar configuraciones apropiadas para lograr y mantener el cumplimiento PCI DSS.
</details>

### Pregunta 25
**¿Qué servicio de AWS ayuda a detectar actividad API inusual y amenazas de seguridad potenciales usando aprendizaje automático?**

- A) AWS CloudTrail
- B) AWS Config
- C) AWS GuardDuty
- D) AWS Inspector

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: AWS GuardDuty usa aprendizaje automático e inteligencia de amenazas para detectar actividad maliciosa y comportamiento no autorizado, incluyendo patrones de actividad API inusuales.
</details>

### Pregunta 26
**Una empresa quiere implementar inicio de sesión único (SSO) para que los empleados puedan usar sus credenciales corporativas para acceder a servicios de AWS. ¿Qué servicio de AWS habilita esto?**

- A) AWS IAM
- B) AWS SSO (ahora AWS IAM Identity Center)
- C) AWS Directory Service
- D) AWS Cognito

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS SSO (ahora llamado AWS IAM Identity Center) habilita acceso de inicio de sesión único a cuentas y aplicaciones de AWS usando credenciales corporativas.
</details>

### Pregunta 27
**¿Cuál es la diferencia entre Security Groups y Network ACLs en AWS?**

- A) Security Groups son para bases de datos, Network ACLs son para servidores web
- B) Security Groups operan a nivel de instancia, Network ACLs operan a nivel de subred
- C) Security Groups son pagos, Network ACLs son gratuitos
- D) No hay diferencia

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Security Groups actúan como firewalls virtuales a nivel de instancia, mientras que Network ACLs operan a nivel de subred. Security Groups son con estado, Network ACLs son sin estado.
</details>

### Pregunta 28
**¿Cuál de las siguientes es una responsabilidad del cliente al usar Amazon RDS?**

- A) Parchear el software de base de datos
- B) Gestionar cuentas de usuario y permisos de base de datos
- C) Reemplazar hardware fallido
- D) Gestionar el sistema operativo subyacente

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Con Amazon RDS, AWS gestiona la infraestructura, SO y parcheo del software de base de datos. Los clientes son responsables de gestionar cuentas de usuario de base de datos, permisos y configuraciones a nivel de base de datos.
</details>

### Pregunta 29
**Una empresa necesita cifrar datos sensibles almacenados en Amazon S3. ¿Qué opciones de cifrado están disponibles? (Selecciona DOS)**

- A) Cifrado del lado del servidor gestionado por AWS (SSE-S3)
- B) Cifrado del lado del cliente
- C) Solo cifrado a nivel de red
- D) Cifrado de base de datos
- E) Solo cifrado a nivel de aplicación

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: A, B**

**Explicación**: S3 soporta tanto cifrado del lado del servidor (gestionado por AWS con SSE-S3, SSE-KMS, o SSE-C) como cifrado del lado del cliente donde los datos son cifrados antes de ser enviados a S3.
</details>

### Pregunta 30
**¿Cuál es el beneficio principal de usar roles IAM en lugar de usuarios IAM para aplicaciones ejecutándose en instancias EC2?**

- A) Los roles son más baratos que los usuarios
- B) Los roles proporcionan mejor rendimiento
- C) Los roles eliminan la necesidad de gestionar credenciales de largo plazo
- D) Los roles proporcionan más permisos que los usuarios

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Los roles IAM proporcionan credenciales temporales que son rotadas automáticamente, eliminando la necesidad de almacenar y gestionar claves de acceso de largo plazo en instancias EC2, lo que mejora la seguridad.
</details>

### Pregunta 31
**¿Qué servicio de AWS proporciona evaluaciones de vulnerabilidades para instancias Amazon EC2?**

- A) AWS GuardDuty
- B) AWS Inspector
- C) AWS Config
- D) AWS Systems Manager

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS Inspector es un servicio automatizado de evaluación de seguridad que ayuda a identificar vulnerabilidades y desviaciones de mejores prácticas de seguridad en instancias EC2 e imágenes de contenedor.
</details>

### Pregunta 32
**Una empresa quiere asegurar que solo direcciones IP específicas puedan acceder a su bucket S3. ¿Qué deberían configurar?**

- A) Security Groups
- B) Network ACLs
- C) Políticas de bucket
- D) Políticas de usuario IAM

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Las políticas de bucket S3 pueden incluir condiciones que restringen el acceso basado en direcciones IP de origen. Security Groups y Network ACLs no se aplican directamente a S3.
</details>

### Pregunta 33
**¿Para qué se usa principalmente AWS Key Management Service (KMS)?**

- A) Gestionar usuarios y roles IAM
- B) Crear y controlar claves de cifrado
- C) Monitorear llamadas API
- D) Configurar seguridad de red

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS KMS es un servicio gestionado para crear y controlar claves de cifrado usadas para cifrar datos a través de servicios y aplicaciones de AWS.
</details>

### Pregunta 34
**¿Qué marco de cumplimiento está específicamente diseñado para agencias gubernamentales de EE.UU. y contratistas?**

- A) HIPAA
- B) SOC 2
- C) FedRAMP
- D) PCI DSS

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: FedRAMP (Federal Risk and Authorization Management Program) está específicamente diseñado para agencias gubernamentales de EE.UU. y contratistas para asegurar que los servicios en la nube cumplan requisitos de seguridad federales.
</details>

### Pregunta 35
**Una empresa necesita monitorear y bloquear tráfico web malicioso a sus aplicaciones. ¿Qué servicio de AWS deberían usar?**

- A) AWS Shield
- B) AWS WAF
- C) AWS GuardDuty
- D) AWS Inspector

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS WAF (Web Application Firewall) protege aplicaciones web de exploits web comunes y permite crear reglas para bloquear tráfico malicioso basado en varios criterios.
</details>

### Pregunta 36
**¿Cuál es el principio de "Defensa en Profundidad" en seguridad de AWS?**

- A) Usar solo un control de seguridad fuerte
- B) Implementar múltiples capas de controles de seguridad
- C) Depender solo de características de seguridad de AWS
- D) Enfocarse solo en seguridad de red

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Defensa en Profundidad involucra implementar múltiples capas de controles de seguridad a través de tu infraestructura, para que si una capa falla, otras capas continúen proporcionando protección.
</details>

---

## ⚙️ Dominio 3: Tecnología y Servicios en la Nube (Preguntas 37-58)

### Pregunta 37
**Una empresa necesita ejecutar un trabajo de procesamiento por lotes que puede tolerar interrupciones y quiere minimizar costos. ¿Qué modelo de precios de EC2 es más apropiado?**

- A) Instancias On-Demand
- B) Instancias Reservadas
- C) Instancias Spot
- D) Hosts Dedicados

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Las Instancias Spot son ideales para trabajos de procesamiento por lotes tolerantes a fallas ya que ofrecen el menor costo (hasta 90% de ahorro) pero pueden ser interrumpidas cuando AWS necesita la capacidad.
</details>

### Pregunta 38
**Una aplicación necesita almacenar datos accedidos frecuentemente con el mayor rendimiento. ¿Qué opción de almacenamiento debería usarse?**

- A) Amazon S3 Standard
- B) Amazon EBS Provisioned IOPS SSD
- C) Amazon S3 Glacier
- D) Amazon EFS

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Amazon EBS Provisioned IOPS SSD proporciona el mayor rendimiento con entrega consistente de IOPS para datos accedidos frecuentemente que requieren baja latencia.
</details>

### Pregunta 39
**Una aplicación de microservicios necesita una forma de desacoplar componentes para que puedan escalar independientemente. ¿Qué patrón de servicio de AWS es más apropiado?**

- A) Conexiones directas a base de datos
- B) Amazon SQS para colas de mensajes
- C) Almacenamiento de archivos compartido
- D) Llamadas API sincronizadas

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Amazon SQS proporciona colas de mensajes que desacoplan componentes de aplicación, permitiéndoles escalar independientemente y comunicarse de forma asíncrona.
</details>

### Pregunta 40
**Una empresa quiere migrar su base de datos Oracle existente a AWS con cambios mínimos. ¿Qué opción es más adecuada?**

- A) Amazon DynamoDB
- B) Amazon RDS for Oracle
- C) Amazon Redshift
- D) Amazon Aurora

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Amazon RDS for Oracle permite migración con cambios mínimos ya que proporciona un entorno de base de datos Oracle gestionado compatible con aplicaciones Oracle existentes.
</details>

### Pregunta 41
**Una aplicación necesita procesar imágenes subidas por usuarios y generar miniaturas. El procesamiento ocurre de forma infrecuente e impredecible. ¿Qué servicio de cómputo es más costo-efectivo?**

- A) Instancias Amazon EC2 ejecutándose 24/7
- B) AWS Lambda
- C) Contenedores Amazon ECS
- D) AWS Batch

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS Lambda es más costo-efectivo para procesamiento infrecuente e impredecible ya que solo pagas por el tiempo de ejecución y no necesitas mantener instancias ejecutándose.
</details>

### Pregunta 42
**Una empresa quiere analizar grandes conjuntos de datos usando consultas SQL sin gestionar infraestructura. ¿Qué servicio deberían usar?**

- A) Amazon EC2 con software de base de datos
- B) Amazon RDS
- C) Amazon Athena
- D) Amazon DynamoDB

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Amazon Athena es un servicio de consultas sin servidor que permite analizar datos usando SQL sin gestionar ninguna infraestructura.
</details>

### Pregunta 43
**Una aplicación de comercio electrónico experimenta picos de tráfico durante eventos de ventas. ¿Qué característica de AWS ajusta automáticamente el número de instancias basándose en la demanda?**

- A) Elastic Load Balancing
- B) Auto Scaling
- C) Amazon CloudWatch
- D) AWS Lambda

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Auto Scaling ajusta automáticamente el número de instancias EC2 basándose en la demanda, escalando hacia arriba durante picos de tráfico y hacia abajo cuando la demanda disminuye.
</details>

### Pregunta 44
**Una aplicación global necesita servir contenido estático con baja latencia a usuarios en todo el mundo. ¿Qué combinación de servicios es más apropiada?**

- A) Amazon S3 + Amazon CloudFront
- B) Amazon EC2 + Elastic Load Balancing
- C) Amazon RDS + Amazon ElastiCache
- D) AWS Lambda + Amazon API Gateway

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: A**

**Explicación**: Amazon S3 para almacenar contenido estático combinado con CloudFront para entrega global de contenido proporciona acceso de baja latencia a usuarios en todo el mundo a través de ubicaciones edge.
</details>

### Pregunta 45
**Una empresa necesita una base de datos NoSQL que pueda escalar para manejar millones de solicitudes por segundo con latencia de milisegundos de un solo dígito. ¿Qué servicio es más adecuado?**

- A) Amazon RDS
- B) Amazon Aurora
- C) Amazon DynamoDB
- D) Amazon Redshift

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Amazon DynamoDB está diseñado para cargas de trabajo NoSQL de alta escala y puede manejar millones de solicitudes por segundo con latencia de milisegundos de un solo dígito.
</details>

### Pregunta 46
**Una aplicación necesita enviar notificaciones a dispositivos móviles cuando ocurren ciertos eventos. ¿Qué servicio de AWS es más apropiado?**

- A) Amazon SES
- B) Amazon SNS
- C) Amazon SQS
- D) Amazon Connect

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Amazon SNS (Simple Notification Service) está diseñado para enviar notificaciones a múltiples endpoints incluyendo dispositivos móviles, email, SMS y otros servicios.
</details>

### Pregunta 47
**Una empresa quiere implementar una arquitectura de lago de datos para almacenar y analizar grandes cantidades de datos estructurados y no estructurados. ¿Qué servicio de almacenamiento es más apropiado?**

- A) Amazon EBS
- B) Amazon EFS
- C) Amazon S3
- D) Amazon RDS

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Amazon S3 es ideal para lagos de datos ya que puede almacenar cantidades virtualmente ilimitadas de datos estructurados y no estructurados con varias clases de almacenamiento para diferentes patrones de acceso.
</details>

### Pregunta 48
**¿Qué servicio de AWS proporciona un entorno Kubernetes gestionado?**

- A) Amazon ECS
- B) Amazon EKS
- C) AWS Fargate
- D) AWS Batch

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Amazon EKS (Elastic Kubernetes Service) proporciona un entorno Kubernetes gestionado, manejando la gestión del plano de control de Kubernetes.
</details>

### Pregunta 49
**Una empresa necesita establecer una conexión de red dedicada entre su centro de datos local y AWS. ¿Qué servicio deberían usar?**

- A) VPN Gateway
- B) AWS Direct Connect
- C) Internet Gateway
- D) NAT Gateway

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS Direct Connect proporciona una conexión de red dedicada entre instalaciones locales y AWS, ofreciendo rendimiento de red consistente y potencialmente menores costos.
</details>

### Pregunta 50
**Una aplicación necesita cachear datos accedidos frecuentemente en memoria para mejorar el rendimiento. ¿Qué servicio es más apropiado?**

- A) Amazon S3
- B) Amazon EBS
- C) Amazon ElastiCache
- D) Amazon EFS

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Amazon ElastiCache proporciona caché en memoria usando Redis o Memcached, mejorando significativamente el rendimiento de aplicaciones para datos accedidos frecuentemente.
</details>

### Pregunta 51
**Una empresa quiere construir una aplicación web sin servidor. ¿Qué combinación de servicios sería más apropiada?**

- A) EC2 + RDS + ELB
- B) Lambda + API Gateway + DynamoDB
- C) ECS + Aurora + CloudFront
- D) Fargate + RDS + Route 53

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Lambda (cómputo sin servidor) + API Gateway (gestión de API sin servidor) + DynamoDB (base de datos sin servidor) proporciona una arquitectura completamente sin servidor.
</details>

### Pregunta 52
**¿Qué servicio usarías para orquestar múltiples servicios de AWS en un flujo de trabajo?**

- A) AWS Lambda
- B) AWS Step Functions
- C) Amazon SQS
- D) Amazon SNS

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS Step Functions es un servicio de flujo de trabajo sin servidor que permite coordinar múltiples servicios de AWS en flujos de trabajo sin servidor usando flujos de trabajo visuales.
</details>

### Pregunta 53
**Una empresa necesita migrar una gran cantidad de datos (100TB) a AWS con impacto mínimo en su ancho de banda de internet. ¿Qué servicio deberían considerar?**

- A) AWS Direct Connect
- B) AWS DataSync
- C) AWS Snowball
- D) Amazon S3 Transfer Acceleration

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: AWS Snowball está diseñado para migración de datos a gran escala (escala de petabytes) sin impactar el ancho de banda de internet, usando dispositivos físicos para transferir datos.
</details>

### Pregunta 54
**¿Qué servicio de AWS proporciona streaming de mensajes gestionado para procesamiento de datos en tiempo real?**

- A) Amazon SQS
- B) Amazon SNS
- C) Amazon Kinesis
- D) AWS Lambda

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Amazon Kinesis proporciona servicios de streaming gestionados para procesamiento de datos en tiempo real, incluyendo Kinesis Data Streams, Kinesis Data Firehose y Kinesis Analytics.
</details>

### Pregunta 55
**Una empresa necesita asegurar que sus instancias EC2 puedan comunicarse entre sí pero no con internet. ¿Qué deberían configurar?**

- A) Una subred pública con internet gateway
- B) Una subred privada sin internet gateway
- C) Un security group que bloquee todo el tráfico
- D) Una VPC con solo una zona de disponibilidad

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Las subredes privadas sin internet gateway permiten que las instancias se comuniquen entre sí dentro de la VPC pero previenen el acceso directo a internet.
</details>

### Pregunta 56
**¿Qué servicio de AWS te ayuda a descubrir y clasificar datos sensibles en buckets S3?**

- A) AWS Config
- B) Amazon Macie
- C) AWS GuardDuty
- D) AWS Inspector

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Amazon Macie usa aprendizaje automático para descubrir, clasificar y proteger datos sensibles en Amazon S3, ayudando con privacidad de datos y cumplimiento de seguridad.
</details>

### Pregunta 57
**Una empresa quiere implementar Infraestructura como Código. ¿Qué servicio de AWS deberían usar?**

- A) AWS Config
- B) AWS CloudFormation
- C) AWS Systems Manager
- D) AWS CodeDeploy

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS CloudFormation habilita Infraestructura como Código permitiendo definir recursos de AWS usando plantillas y gestionarlos como código.
</details>

### Pregunta 58
**¿Qué servicio proporciona métricas de monitoreo detalladas y logs para recursos y aplicaciones de AWS?**

- A) AWS CloudTrail
- B) AWS Config
- C) Amazon CloudWatch
- D) AWS X-Ray

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Amazon CloudWatch proporciona monitoreo, métricas, logs y alarmas para recursos y aplicaciones de AWS, ofreciendo información operacional detallada.
</details>

---

## 💰 Dominio 4: Facturación y Soporte (Preguntas 59-65)

### Pregunta 59
**Una empresa tiene cargas de trabajo impredecibles pero quiere ahorrar dinero en sus costos de EC2. Pueden comprometerse a una cantidad específica de dólares por hora. ¿Qué modelo de precios deberían elegir?**

- A) Instancias On-Demand
- B) Instancias Reservadas
- C) Instancias Spot
- D) Savings Plans

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: D**

**Explicación**: Los Savings Plans permiten comprometerse a una cantidad específica de dólares por hora por 1 o 3 años, proporcionando flexibilidad para cargas de trabajo cambiantes mientras ofrecen ahorros significativos.
</details>

### Pregunta 60
**¿Qué herramienta proporciona recomendaciones para optimización de costos basadas en tu uso real de AWS?**

- A) AWS Pricing Calculator
- B) AWS Trusted Advisor
- C) AWS Cost Explorer
- D) AWS Budgets

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS Trusted Advisor proporciona recomendaciones de optimización de costos basadas en tus patrones de uso reales, identificando oportunidades para reducir costos.
</details>

### Pregunta 61
**Una empresa quiere recibir alertas cuando su factura mensual de AWS exceda $1000. ¿Qué servicio deberían usar?**

- A) AWS Cost Explorer
- B) AWS Budgets
- C) AWS Trusted Advisor
- D) AWS Pricing Calculator

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS Budgets permite establecer presupuestos personalizados de costo y uso y recibir alertas cuando el uso real o pronosticado excede los umbrales definidos.
</details>

### Pregunta 62
**¿Qué plan de soporte proporciona acceso a la API de AWS Support para gestión programática de casos?**

- A) Basic Support
- B) Developer Support
- C) Business Support
- D) Todos los planes de soporte

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: La API de AWS Support está disponible comenzando con el plan Business Support, permitiendo acceso programático para crear y gestionar casos de soporte.
</details>

### Pregunta 63
**Una startup espera que su uso de AWS crezca significativamente durante el próximo año. Quieren precios predecibles para su infraestructura central. ¿Qué enfoque es más adecuado?**

- A) Usar solo Instancias Spot
- B) Comprar Instancias Reservadas para capacidad base y usar On-Demand para crecimiento
- C) Usar solo Instancias On-Demand
- D) Comprar Instancias Reservadas para capacidad pico proyectada

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Usar Instancias Reservadas para capacidad base proporciona ahorros de costo para uso predecible, mientras que instancias On-Demand manejan crecimiento variable, balanceando optimización de costos con flexibilidad.
</details>

### Pregunta 64
**¿Cuál de las siguientes está incluida en el Nivel Gratuito de AWS? (Selecciona DOS)**

- A) 750 horas de instancias Amazon EC2 t2.micro por mes
- B) 5 GB de almacenamiento Amazon S3 Standard
- C) Transferencia de datos ilimitada
- D) 25 GB de almacenamiento Amazon DynamoDB
- E) Acceso gratuito a todos los servicios de AWS

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: A, D**

**Explicación**: El Nivel Gratuito de AWS incluye 750 horas de instancias EC2 t2.micro y 25 GB de almacenamiento DynamoDB por mes. S3 incluye 5 GB, pero la transferencia de datos y acceso a todos los servicios no son ilimitados o gratuitos.
</details>

### Pregunta 65
**Una empresa necesita datos detallados de costo y uso para análisis en sus herramientas de inteligencia de negocios. ¿Qué servicio de AWS proporciona los datos de facturación más completos?**

- A) AWS Cost Explorer
- B) AWS Budgets
- C) AWS Cost and Usage Reports (CUR)
- D) AWS Billing Dashboard

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: AWS Cost and Usage Reports (CUR) proporcionan los datos de facturación más completos y detallados que pueden ser exportados y analizados en herramientas externas de inteligencia de negocios.
</details>

---

## 📊 Practice Exam 2 - Answer Key

### Domain 1: Cloud Concepts (16/16)
1. C | 2. C | 3. C | 4. A | 5. C | 6. C | 7. A | 8. B | 9. B | 10. B | 11. B | 12. B | 13. C | 14. B,D | 15. B | 16. C

### Domain 2: Security & Compliance (20/20)
17. C | 18. B | 19. C | 20. B | 21. B | 22. A,B | 23. B | 24. B | 25. C | 26. B | 27. B | 28. B | 29. A,B | 30. C | 31. B | 32. C | 33. B | 34. C | 35. B | 36. B

### Domain 3: Cloud Technology & Services (22/22)
37. C | 38. B | 39. B | 40. B | 41. B | 42. C | 43. B | 44. A | 45. C | 46. B | 47. C | 48. B | 49. B | 50. C | 51. B | 52. B | 53. C | 54. C | 55. B | 56. B | 57. B | 58. C

### Domain 4: Billing & Support (7/7)
59. D | 60. B | 61. B | 62. C | 63. B | 64. A,D | 65. C

---

## 🎯 Scoring Guide

**Calculate your score:**
- Count correct answers: ___/65
- Percentage: (Correct answers ÷ 65) × 100 = ___%
- **Passing Score**: 70% (46/65 correct)

### 📈 Performance Analysis

**90-100% (59-65 correct)**: Outstanding! You're ready for the exam.
**80-89% (52-58 correct)**: Very good. Review missed questions and take Practice Exam 3.
**70-79% (46-51 correct)**: Passing level. Focus study on weak areas before exam.
**Below 70% (<46 correct)**: More preparation needed. Review study materials thoroughly.

### 🔍 Domain-Specific Analysis

Track your performance by domain:
- **Domain 1 (Cloud Concepts)**: ___/16 = ___%
- **Domain 2 (Security & Compliance)**: ___/20 = ___%
- **Domain 3 (Technology & Services)**: ___/22 = ___%
- **Domain 4 (Billing & Support)**: ___/7 = ___%

Focus additional study on domains where you scored below 75%.

---

## 📚 Study Resources & Next Steps

### 🎯 If you scored 85%+:
- Take [Practice Exam 3](practice-exam-3.md) for final validation
- Review [Quick Reference Guide](../quick-reference/service-cheatsheet.md)
- Schedule your real exam!

### 🎯 If you scored 70-84%:
- Review study materials for domains where you scored poorly
- Focus on scenario-based questions
- Retake this exam in 3-5 days

### 🎯 If you scored below 70%:
- Return to the main study materials
- Focus on fundamental concepts
- Take chapter quizzes before attempting another practice exam

### 📖 Domain-Specific Study Links:
- 🌩️ [Domain 1: Cloud Concepts](../01-cloud-concepts/README.md)
- 🔒 [Domain 2: Security & Compliance](../02-security-compliance/README.md)
- ⚙️ [Domain 3: Technology & Services](../03-technology-services/README.md)
- 💰 [Domain 4: Billing & Support](../04-billing-support/README.md)

---

*Keep up the great work! Each practice exam brings you closer to certification success! 🚀*

### Pregunta 3
**Una empresa de manufactura quiere mantener sus sistemas de producción críticos en sus propias instalaciones por razones de seguridad, pero usar la nube para desarrollo y pruebas. ¿Qué modelo de implementación describe mejor esta estrategia?**

- A) Nube pública
- B) Nube privada
- C) Nube híbrida
- D) Nube comunitaria

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Una nube híbrida combina infraestructura local (para sistemas críticos) con servicios de nube pública (para desarrollo y pruebas), permitiendo a las organizaciones mantener control sobre datos sensibles mientras aprovechan los beneficios de la nube.
</details>

### Pregunta 4
**¿Cuál de las siguientes opciones describe mejor la diferencia entre escalabilidad horizontal y vertical?**

- A) Horizontal es más caro que vertical
- B) Horizontal agrega más instancias, vertical aumenta el poder de instancias existentes
- C) Vertical es solo para bases de datos, horizontal es para aplicaciones web
- D) No hay diferencia, son términos intercambiables

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: La escalabilidad horizontal (scale out) agrega más instancias para manejar la carga, mientras que la escalabilidad vertical (scale up) aumenta los recursos (CPU, memoria) de las instancias existentes.
</details>

### Pregunta 5
**Una empresa global necesita cumplir con regulaciones de residencia de datos que requieren que ciertos datos permanezcan en países específicos. ¿Qué concepto de AWS les ayuda a cumplir con este requisito?**

- A) Zonas de Disponibilidad
- B) Regiones
- C) Edge Locations
- D) Local Zones

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Las Regiones de AWS están ubicadas en diferentes países y áreas geográficas, permitiendo a las empresas elegir dónde almacenar sus datos para cumplir con requisitos de residencia de datos y regulaciones locales.
</details>

---

## 🔒 Dominio 2: Seguridad y Cumplimiento (Preguntas 6-25)

### Pregunta 6
**Según el modelo de responsabilidad compartida de AWS, ¿quién es responsable de parchear el sistema operativo invitado en una instancia EC2?**

- A) AWS es completamente responsable
- B) El cliente es completamente responsable
- C) La responsabilidad es compartida entre AWS y el cliente
- D) Depende del tipo de instancia

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: En el modelo de responsabilidad compartida, el cliente es responsable de parchear el sistema operativo invitado en instancias EC2. AWS es responsable de la infraestructura subyacente y el hipervisor.
</details>

### Pregunta 7
**Una empresa quiere asegurar que solo usuarios autenticados con MFA puedan acceder a recursos críticos de AWS. ¿Qué componente de IAM sería más apropiado para implementar esta restricción?**

- A) Usuarios de IAM
- B) Grupos de IAM
- C) Políticas de IAM con condiciones
- D) Roles de IAM

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Las políticas de IAM con condiciones pueden requerir MFA usando la condición "aws:MultiFactorAuthPresent": "true", asegurando que solo usuarios con MFA activo puedan acceder a recursos específicos.
</details>

### Pregunta 8
**¿Cuál es la mejor práctica para gestionar credenciales de acceso para una aplicación que se ejecuta en EC2 y necesita acceder a S3?**

- A) Hardcodear las claves de acceso en el código de la aplicación
- B) Almacenar las credenciales en un archivo de configuración en la instancia
- C) Usar roles de IAM asignados a la instancia EC2
- D) Crear un usuario de IAM y compartir las credenciales

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Los roles de IAM proporcionan credenciales temporales y rotativas automáticamente a las instancias EC2, eliminando la necesidad de almacenar credenciales de larga duración y mejorando la seguridad.
</details>

### Pregunta 9
**¿Qué servicio de AWS proporciona protección DDoS administrada automáticamente para todos los clientes de AWS sin costo adicional?**

- A) AWS WAF
- B) AWS Shield Standard
- C) AWS Shield Advanced
- D) AWS GuardDuty

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS Shield Standard proporciona protección DDoS automática para todos los clientes de AWS sin costo adicional, protegiendo contra los ataques DDoS más comunes.
</details>

### Pregunta 10
**Una empresa necesita cifrar datos en tránsito entre su aplicación web y los usuarios finales. ¿Cuál es la mejor práctica para lograr esto?**

- A) Usar HTTP en lugar de HTTPS
- B) Implementar certificados SSL/TLS
- C) Cifrar los datos en la base de datos
- D) Usar VPN para todos los usuarios

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Los certificados SSL/TLS habilitan HTTPS, que cifra los datos en tránsito entre la aplicación web y los usuarios finales, protegiendo la información durante la transmisión.
</details>

---

## 💻 Dominio 3: Tecnología y Servicios (Preguntas 11-32)

### Pregunta 11
**Una aplicación experimenta picos de tráfico impredecibles que duran solo unos minutos. ¿Qué servicio de AWS sería más costo-efectivo para manejar estos picos?**

- A) Instancias EC2 Reserved
- B) Instancias EC2 On-Demand con Auto Scaling
- C) AWS Lambda
- D) Instancias EC2 Spot

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: AWS Lambda es ideal para cargas de trabajo de corta duración e impredecibles porque se factura solo por el tiempo de ejecución real, sin costos cuando no está ejecutándose, y escala automáticamente.
</details>

### Pregunta 12
**Una empresa necesita almacenar archivos de respaldo que se acceden raramente pero deben estar disponibles dentro de 12 horas cuando se necesiten. ¿Qué clase de almacenamiento de S3 sería más apropiada?**

- A) S3 Standard
- B) S3 Standard-IA
- C) S3 Glacier Flexible Retrieval
- D) S3 Glacier Deep Archive

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: S3 Glacier Flexible Retrieval es ideal para datos de archivo que se acceden raramente y pueden tolerar tiempos de recuperación de minutos a horas, ofreciendo un buen equilibrio entre costo y tiempo de acceso.
</details>

### Pregunta 13
**¿Cuál es la principal diferencia entre Amazon RDS y Amazon DynamoDB?**

- A) RDS es más caro que DynamoDB
- B) RDS es para bases de datos relacionales, DynamoDB es para bases de datos NoSQL
- C) RDS solo funciona con MySQL, DynamoDB con cualquier base de datos
- D) No hay diferencia, son servicios idénticos

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Amazon RDS es un servicio de base de datos relacional administrado que soporta motores como MySQL, PostgreSQL, Oracle, etc., mientras que DynamoDB es un servicio de base de datos NoSQL completamente administrado.
</details>

### Pregunta 14
**Una empresa quiere distribuir contenido estático globalmente con baja latencia. ¿Qué servicio de AWS deberían usar?**

- A) Amazon S3
- B) Amazon CloudFront
- C) Amazon Route 53
- D) Elastic Load Balancer

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Amazon CloudFront es un servicio de red de entrega de contenido (CDN) que distribuye contenido globalmente desde ubicaciones edge, proporcionando baja latencia y alta velocidad de transferencia.
</details>

### Pregunta 15
**¿Qué servicio permite crear una red privada virtual en AWS?**

- A) Amazon Route 53
- B) Amazon VPC
- C) AWS Direct Connect
- D) Amazon CloudFront

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Amazon VPC (Virtual Private Cloud) permite crear una red privada virtual en la nube de AWS, proporcionando control completo sobre el entorno de red virtual.
</details>

---

## 💰 Dominio 4: Facturación y Soporte (Preguntas 16-22)

### Pregunta 16
**Una empresa quiere recibir alertas cuando sus costos mensuales de AWS excedan $1000. ¿Qué herramienta deberían usar?**

- A) AWS Cost Explorer
- B) AWS Budgets
- C) AWS Billing Dashboard
- D) AWS Cost and Usage Report

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS Budgets permite establecer presupuestos personalizados y recibir alertas cuando los costos o el uso exceden (o se prevé que excedan) los umbrales definidos.
</details>

### Pregunta 17
**¿Cuál de las siguientes opciones está incluida en el nivel gratuito de AWS para nuevos clientes?**

- A) 750 horas de instancias EC2 t2.micro por mes durante 12 meses
- B) Uso ilimitado de todos los servicios de AWS
- C) Soporte técnico 24/7 gratuito
- D) Instancias EC2 de cualquier tamaño gratis por 6 meses

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: A**

**Explicación**: El nivel gratuito de AWS incluye 750 horas de instancias EC2 t2.micro (o t3.micro en algunas regiones) por mes durante los primeros 12 meses para nuevos clientes de AWS.
</details>

### Pregunta 18
**Una empresa quiere analizar sus patrones de gasto de AWS de los últimos 6 meses para identificar oportunidades de ahorro. ¿Qué herramienta sería más útil?**

- A) AWS Budgets
- B) AWS Cost Explorer
- C) AWS Pricing Calculator
- D) AWS Billing Dashboard

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS Cost Explorer proporciona análisis detallado de costos y uso histórico, permitiendo identificar tendencias y oportunidades de optimización de costos a lo largo del tiempo.
</details>

### Pregunta 19
**¿Qué plan de soporte de AWS incluye acceso a AWS Trusted Advisor con todas las verificaciones?**

- A) Basic Support
- B) Developer Support
- C) Business Support
- D) Todos los planes incluyen todas las verificaciones

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: AWS Trusted Advisor con todas las verificaciones está disponible para clientes con planes Business Support y Enterprise Support. Los planes Basic y Developer tienen acceso limitado a las verificaciones.
</details>

### Pregunta 20
**¿Cuál es el beneficio principal de usar Instancias Reservadas en lugar de instancias On-Demand?**

- A) Mejor rendimiento
- B) Ahorros significativos de costos
- C) Acceso a tipos de instancia exclusivos
- D) Soporte técnico mejorado

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Las Instancias Reservadas ofrecen ahorros significativos (hasta 75%) comparado con precios On-Demand a cambio de un compromiso de 1 o 3 años, siendo el principal beneficio la reducción de costos.
</details>

---

## 📊 Evaluación y Próximos Pasos

### Cálculo de Puntuación
**Para evaluar tu rendimiento:**
1. Cuenta tus respuestas correctas
2. Divide por 20 (total de preguntas en esta muestra)
3. Multiplica por 100 para obtener el porcentaje

### Interpretación de Resultados
- **85-100%**: ¡Excelente! Estás muy bien preparado para el examen
- **75-84%**: Muy bien, revisa las áreas donde fallaste
- **65-74%**: Buen progreso, necesitas más estudio en áreas específicas
- **Menos de 65%**: Necesitas más preparación antes del examen real

### Recomendaciones por Dominio

**Si tuviste dificultades con Dominio 1 (Conceptos de la Nube):**
- Revisa los beneficios y características de la computación en la nube
- Estudia los modelos de implementación (público, privado, híbrido)
- Practica escenarios de migración y casos de uso

**Si tuviste dificultades con Dominio 2 (Seguridad):**
- Enfócate en el modelo de responsabilidad compartida
- Estudia IAM en profundidad (usuarios, grupos, roles, políticas)
- Revisa los servicios de seguridad de AWS

**Si tuviste dificultades con Dominio 3 (Tecnología):**
- Revisa los servicios principales: EC2, S3, RDS, Lambda, VPC
- Estudia cuándo usar cada servicio
- Practica arquitecturas de soluciones

**Si tuviste dificultades con Dominio 4 (Facturación):**
- Estudia las herramientas de gestión de costos
- Revisa los modelos de precios y planes de soporte
- Practica con calculadoras de precios

---

## 🎯 Preparación Continua

1. **Revisa respuestas incorrectas** - Entiende el razonamiento detrás de cada respuesta
2. **Estudia documentación oficial** - Consulta la documentación de AWS para detalles
3. **Toma más exámenes** - Practica con diferentes tipos de preguntas
4. **Únete a comunidades** - Participa en foros y grupos de estudio
5. **Programa tu examen** - Cuando consistentemente obtengas 80%+ en práctica

¡Continúa con tu excelente preparación para el AWS Cloud Practitioner! 🚀