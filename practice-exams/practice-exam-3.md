# 📝 Examen de Práctica 3 - AWS Cloud Practitioner

> **Simulación de examen final con casos límite desafiantes y escenarios del mundo real**

## 📋 Instrucciones del Examen

- **Límite de Tiempo**: 90 minutos (recomendado)
- **Preguntas**: 65 de opción múltiple y respuesta múltiple
- **Puntuación para Aprobar**: 70% (46 de 65 preguntas)
- **Distribución por Dominio**: Refleja las ponderaciones del examen real
- **Formato**: Elige la MEJOR respuesta para cada pregunta
- **Dificultad**: Nivel avanzado con escenarios complicados

### 📊 Distribución de Preguntas por Dominio
- **Dominio 1 (Conceptos de la Nube)**: 16 preguntas (24%)
- **Dominio 2 (Seguridad y Cumplimiento)**: 20 preguntas (30%)
- **Dominio 3 (Tecnología y Servicios)**: 22 preguntas (34%)
- **Dominio 4 (Facturación y Soporte)**: 7 preguntas (12%)

---

## 🌩️ Dominio 1: Conceptos de la Nube (Preguntas 1-16)

### Pregunta 1
**Una institución financiera está evaluando la adopción de la nube pero tiene preocupaciones sobre la soberanía de datos y el cumplimiento regulatorio. Necesitan asegurar que sus datos nunca salgan de las fronteras de su país. ¿Qué solución de AWS aborda esta preocupación mientras aún proporciona beneficios de la nube?**

- A) Usar la infraestructura global de AWS con cifrado de datos
- B) Desplegar aplicaciones solo en Regiones de AWS dentro de su país
- C) Usar AWS Edge Locations para todo el almacenamiento de datos
- D) Implementar recuperación ante desastres multi-región

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Desplegar aplicaciones solo en Regiones de AWS dentro de su país asegura la soberanía de datos. AWS garantiza que los datos almacenados en una Región permanecen dentro de los límites geográficos de esa Región a menos que sean movidos explícitamente por el cliente.
</details>

### Pregunta 2
**Una empresa está comparando la economía de la nube con su infraestructura local actual. Sus servidores locales están actualmente utilizados al 15% en promedio, con picos que alcanzan el 40% durante períodos comerciales específicos. ¿Cómo aborda la computación en la nube esta ineficiencia?**

- A) La computación en la nube garantiza 100% de utilización del servidor
- B) Los recursos de la nube pueden dimensionarse para la demanda real y escalarse automáticamente
- C) La computación en la nube requiere operación 24/7 como los sistemas locales
- D) Los recursos de la nube no pueden redimensionarse una vez desplegados

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: La computación en la nube te permite dimensionar recursos para la demanda real y escalar automáticamente, eliminando la necesidad de aprovisionar para la capacidad pico que permanece inactiva la mayor parte del tiempo. Esto aborda directamente la ineficiencia de utilización del 15%.
</details>

### Pregunta 3
**Una empresa de videojuegos necesita desplegar servidores globalmente para proporcionar experiencias multijugador de baja latencia. Estiman que necesitan infraestructura en 8 regiones geográficas diferentes. ¿Cuál es la ventaja principal de usar AWS para este requisito comparado con construir su propia infraestructura global?**

- A) AWS siempre es más barato que la infraestructura autoconstruida
- B) AWS elimina la necesidad de optimización de red
- C) AWS proporciona presencia global inmediata sin inversión inicial masiva
- D) AWS garantiza latencia cero entre todas las regiones

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: La infraestructura global de AWS permite el despliegue inmediato a través de múltiples regiones sin el gasto de capital masivo y el tiempo requerido para construir tus propios centros de datos globales.
</details>

### Pregunta 4
**La aplicación de una startup experimenta un aumento de tráfico de 1000x durante la noche debido a la atención viral en redes sociales. Su infraestructura local no puede manejar esta carga. ¿Cómo sería diferente este escenario si estuvieran usando computación en la nube?**

- A) La aplicación aún fallaría debido al pico repentino
- B) Los recursos de la nube podrían escalar automáticamente para manejar el aumento de demanda
- C) Necesitarían agregar servidores manualmente lo que toma semanas
- D) La computación en la nube no puede manejar picos repentinos de tráfico

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: La elasticidad de la computación en la nube permite el escalado automático para manejar picos repentinos de demanda. Características como Auto Scaling pueden aumentar la capacidad en minutos en lugar de las semanas requeridas para infraestructura física.
</details>

### Pregunta 5
**¿Qué escenario demuestra mejor la ventaja "Dejar de gastar dinero ejecutando y manteniendo centros de datos" de la computación en la nube?**

- A) Una empresa reduce sus costos de licencias de software en un 50%
- B) Una empresa elimina los costos de instalaciones de centros de datos, facturas de energía y personal de mantenimiento de hardware
- C) Una empresa mejora el rendimiento de su aplicación en un 200%
- D) Una empresa aumenta el tamaño de su equipo de desarrollo

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Esta ventaja se refiere específicamente a eliminar la sobrecarga operacional de los centros de datos físicos: costos de instalaciones, energía, refrigeración, mantenimiento de hardware y personal asociado.
</details>

### Pregunta 6
**Una organización de investigación procesa grandes conjuntos de datos que requieren recursos de computación especializados durante 2 horas cada mes. El resto del tiempo, los recursos de computación permanecen inactivos. ¿Qué característica de la nube aborda mejor este caso de uso?**

- A) Acceso amplio a la red
- B) Agrupación de recursos
- C) Autoservicio bajo demanda
- D) Servicio medido

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: El autoservicio bajo demanda permite a la organización aprovisionar recursos solo cuando los necesita (durante esas 2 horas) y liberarlos cuando termine, evitando costos por recursos inactivos.
</details>

### Pregunta 7
**Una empresa está decidiendo entre Plataforma como Servicio (PaaS) e Infraestructura como Servicio (IaaS) para su aplicación web. Quieren enfocarse en el desarrollo de aplicaciones y no preocuparse por las actualizaciones del sistema operativo. ¿Qué modelo deberían elegir?**

- A) IaaS porque es más barato
- B) PaaS porque el proveedor de la nube gestiona el sistema operativo
- C) IaaS porque proporciona más control
- D) Ninguno, deberían usar SaaS

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: PaaS abstrae la gestión del sistema operativo, permitiendo a los desarrolladores enfocarse en el código de la aplicación mientras el proveedor de la nube maneja las actualizaciones del SO, parches y gestión de infraestructura.
</details>

### Pregunta 8
**Una plataforma de e-learning sirve a estudiantes globalmente con contenido de video. Los estudiantes en Asia reportan tiempos de carga lentos para videos alojados en centros de datos de EE.UU. ¿Qué componente de infraestructura de AWS abordaría mejor este problema?**

- A) Zonas de Disponibilidad adicionales en EE.UU.
- B) Servidores más potentes en el centro de datos existente de EE.UU.
- C) Entrega de contenido a través de ubicaciones edge de CloudFront cerca de estudiantes asiáticos
- D) Migrar toda la infraestructura a Asia

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Las ubicaciones edge de CloudFront almacenan en caché el contenido más cerca de los usuarios finales globalmente, reduciendo significativamente la latencia para estudiantes en Asia sin requerir migración de infraestructura.
</details>

### Pregunta 9
**Una empresa quiere entender la diferencia entre escalado horizontal y vertical para su nivel de base de datos. Su base de datos está actualmente limitada por CPU durante las horas pico. ¿Qué enfoque de escalado sería más apropiado para este escenario específico?**

- A) Escalado horizontal agregando más servidores de base de datos
- B) Escalado vertical actualizando a un servidor más potente
- C) Ambos enfoques son igualmente efectivos
- D) Ningún enfoque ayudaría con las limitaciones de CPU

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Para una base de datos limitada por CPU, el escalado vertical (actualizar a hardware más potente con mejor CPU) es a menudo más apropiado que el escalado horizontal, que funciona mejor para aplicaciones distribuidas.
</details>

### Pregunta 10
**¿Cuál de los siguientes escenarios demuestra el principio de computación en la nube de "servicio medido" o "pago por uso"?**

- A) Una empresa paga una tarifa mensual fija independientemente del uso
- B) Una empresa paga solo por el espacio de almacenamiento y tiempo de cómputo que realmente consume
- C) Una empresa debe comprometerse a un contrato anual mínimo
- D) Una empresa paga basándose en el número de empleados

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Servicio medido significa que pagas solo por lo que realmente consumes (almacenamiento, tiempo de cómputo, transferencia de datos, etc.), no tarifas fijas o compromisos mínimos.
</details>

### Pregunta 11
**Un consultor de recuperación ante desastres está explicando los beneficios de las múltiples Zonas de Disponibilidad de AWS dentro de una Región. ¿Cuál es el beneficio empresarial principal de esta arquitectura?**

- A) Reduce costos compartiendo recursos
- B) Proporciona tolerancia a fallos - si una AZ falla, las aplicaciones pueden continuar ejecutándose en otra AZ
- C) Mejora el rendimiento distribuyendo la carga
- D) Simplifica la gestión centralizando recursos

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Múltiples AZs proporcionan tolerancia a fallos y alta disponibilidad. Si una AZ experimenta una interrupción, las aplicaciones pueden continuar ejecutándose en otras AZs dentro de la misma Región, asegurando la continuidad del negocio.
</details>

### Pregunta 12
**Una empresa manufacturera está evaluando el despliegue de nube híbrida. Quieren mantener sus procesos de manufactura sensibles en las instalaciones pero usar servicios de nube para aplicaciones orientadas al cliente. ¿Cuál es el beneficio principal de este enfoque?**

- A) Siempre es más barato que nube pura o instalaciones puras
- B) Les permite mantener control sobre procesos sensibles mientras aprovechan los beneficios de la nube para otras cargas de trabajo
- C) Elimina la necesidad de conectividad a internet
- D) Garantiza 100% de tiempo de actividad para todas las aplicaciones

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: La nube híbrida permite a las organizaciones mantener cargas de trabajo sensibles o reguladas en las instalaciones mientras aprovechan la escalabilidad, alcance global e innovación de la nube para otras aplicaciones.
</details>

### Pregunta 13
**¿Cuál es la diferencia clave entre las Regiones de AWS y las Zonas Locales de AWS en términos de sus casos de uso principales?**

- A) Las Regiones son para producción, las Zonas Locales son para desarrollo
- B) Las Regiones proporcionan servicios completos de AWS, las Zonas Locales acercan el cómputo a ubicaciones geográficas específicas
- C) Las Zonas Locales son más caras que las Regiones
- D) No hay diferencia en sus capacidades

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Las Regiones proporcionan la suite completa de servicios de AWS a través de múltiples AZs, mientras que las Zonas Locales acercan un subconjunto de servicios de AWS a grandes centros de población para aplicaciones de ultra-baja latencia.
</details>

### Pregunta 14
**El CTO de una empresa está tratando de entender cómo la computación en la nube cambia su enfoque de planificación de capacidad. ¿Cuál es el cambio fundamental en la planificación de capacidad al moverse a la nube?**

- A) Aún necesitas planificar para la capacidad pico por adelantado
- B) Puedes comenzar con capacidad mínima y escalar basándote en la demanda real
- C) La planificación de capacidad se vuelve más compleja en la nube
- D) La nube elimina la necesidad de cualquier planificación de capacidad

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: La computación en la nube cambia fundamentalmente la planificación de capacidad de adivinar las necesidades pico por adelantado a comenzar pequeño y escalar basándose en la demanda real medida, reduciendo riesgo y costos.
</details>

### Pregunta 15
**¿Cuál de los siguientes ilustra mejor el beneficio "Aumentar velocidad y agilidad" de la computación en la nube en un escenario empresarial real?**

- A) Una startup puede lanzar una aplicación global en múltiples países en días en lugar de meses
- B) Las aplicaciones automáticamente se ejecutan más rápido en la nube
- C) La computación en la nube proporciona poder de cómputo ilimitado
- D) Las velocidades de red siempre son más rápidas en la nube

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: A**

**Explicación**: El aumento de velocidad y agilidad se refiere a la capacidad de aprovisionar recursos rápidamente y desplegar aplicaciones globalmente, habilitando tiempo de comercialización más rápido y experimentación rápida.
</details>

### Pregunta 16
**Una agencia gubernamental está preocupada por los requisitos de residencia de datos. Necesitan asegurar que sus datos permanezcan dentro de límites geográficos específicos. ¿Cómo aborda AWS esta preocupación?**

- A) AWS automáticamente replica todos los datos globalmente para redundancia
- B) Los datos del cliente permanecen en la Región donde eligen almacenarlos a menos que lo configuren de otra manera
- C) La residencia de datos no puede controlarse en entornos de nube
- D) Solo ciertos servicios de AWS cumplen con los requisitos de residencia de datos

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS asegura que los datos del cliente permanezcan en la Región de AWS donde eligen almacenarlos y no los moverá a menos que el cliente configure explícitamente replicación entre regiones o migración.
</details>

---

## 🔒 Dominio 2: Seguridad y Cumplimiento (Preguntas 17-36)

### Pregunta 17
**Una auditoría de seguridad de una empresa reveló que varias instancias EC2 han sido lanzadas con grupos de seguridad excesivamente permisivos que permiten acceso SSH desde 0.0.0.0/0. Según el Modelo de Responsabilidad Compartida de AWS, ¿quién es responsable de arreglar este problema de seguridad?**

- A) AWS es responsable porque gestionan la infraestructura
- B) El cliente es responsable porque los grupos de seguridad son una configuración del cliente
- C) Es una responsabilidad compartida que requiere acción tanto de AWS como del cliente
- D) La responsabilidad depende del tipo de instancia

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Las configuraciones de grupos de seguridad caen bajo la responsabilidad del cliente en el Modelo de Responsabilidad Compartida. AWS proporciona el servicio de grupos de seguridad, pero los clientes son responsables de configurarlo de manera segura.
</details>

### Pregunta 18
**Una empresa de servicios financieros necesita asegurar que todas las llamadas API a su entorno AWS sean registradas para propósitos de cumplimiento. También necesitan detectar si alguien intenta eliminar estos registros. ¿Qué combinación de servicios deberían implementar?**

- A) Solo CloudWatch Logs
- B) CloudTrail para registro + alarmas CloudWatch para monitorear intentos de eliminación de registros
- C) Solo Config para monitoreo de cumplimiento
- D) Solo GuardDuty para detección de amenazas

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: CloudTrail registra todas las llamadas API para cumplimiento, y las alarmas CloudWatch pueden detectar intentos de eliminar registros CloudTrail monitoreando llamadas API específicas como DeleteTrail o StopLogging.
</details>

### Pregunta 19
**Un equipo de desarrollo está construyendo una aplicación de microservicios donde diferentes servicios necesitan acceder a diferentes recursos de AWS. ¿Cuál es la forma más segura de gestionar permisos para estos servicios ejecutándose en instancias EC2?**

- A) Usar las mismas credenciales de usuario IAM para todos los servicios
- B) Crear roles IAM individuales para cada servicio con permisos de menor privilegio
- C) Usar las credenciales de la cuenta root por simplicidad
- D) Almacenar credenciales en archivos de configuración de aplicación

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Los roles IAM individuales con permisos de menor privilegio proporcionan el enfoque más seguro, asegurando que cada servicio solo pueda acceder a los recursos que específicamente necesita sin exponer credenciales a largo plazo.
</details>

### Pregunta 20
**Una empresa quiere federar sus usuarios de Active Directory existentes a AWS para que los empleados puedan acceder a servicios de AWS usando sus credenciales corporativas. ¿Qué servicios de AWS deberían considerar? (Selecciona DOS)**

- A) AWS IAM Identity Center (anteriormente AWS SSO)
- B) AWS Directory Service
- C) AWS Cognito
- D) AWS Organizations
- E) AWS Config

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: A, B**

**Explicación**: AWS IAM Identity Center habilita SSO con credenciales corporativas, y AWS Directory Service puede integrarse con la infraestructura de Active Directory existente para habilitar federación.
</details>

### Pregunta 21
**Una empresa de comercio electrónico descubre actividad API inusual en sus registros CloudTrail - alguien está haciendo llamadas API desde un rango de direcciones IP desconocido. ¿Qué servicio de AWS podría haber detectado automáticamente esta actividad sospechosa?**

- A) AWS Config
- B) AWS CloudWatch
- C) AWS GuardDuty
- D) AWS Inspector

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: AWS GuardDuty usa aprendizaje automático para detectar comportamiento anómalo, incluyendo llamadas API desde ubicaciones o direcciones IP inusuales, y alertaría automáticamente sobre tal actividad sospechosa.
</details>

### Pregunta 22
**Una startup está construyendo una aplicación móvil que requiere autenticación de usuario y quiere permitir a los usuarios iniciar sesión con sus cuentas de Google o Facebook. ¿Qué servicio de AWS es más apropiado para este caso de uso?**

- A) AWS IAM
- B) AWS Cognito
- C) AWS Directory Service
- D) AWS IAM Identity Center

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS Cognito está diseñado para aplicaciones móviles y web y soporta federación con proveedores de identidad social como Google y Facebook para autenticación de usuarios.
</details>

### Pregunta 23
**El equipo de seguridad de una empresa quiere asegurar que los buckets S3 no puedan hacerse públicos accidentalmente. Quieren implementar un control preventivo que bloquee configuraciones de acceso público. ¿Qué deberían implementar?**

- A) Políticas de bucket S3
- B) Políticas IAM
- C) Configuraciones de Bloqueo de Acceso Público S3
- D) Registro CloudTrail

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Las configuraciones de Bloqueo de Acceso Público S3 proporcionan controles preventivos que anulan otras políticas y permisos para asegurar que los buckets no puedan configurarse para acceso público, incluso accidentalmente.
</details>

### Pregunta 24
**Una organización de salud necesita asegurar que su infraestructura AWS cumpla con los requisitos HIPAA. ¿Cuál es su responsabilidad principal respecto al cumplimiento HIPAA en AWS?**

- A) AWS automáticamente hace que todos los servicios cumplan con HIPAA
- B) La organización debe usar solo servicios elegibles para HIPAA e implementar configuraciones apropiadas
- C) El cumplimiento HIPAA no es posible en la nube
- D) Solo AWS es responsable del cumplimiento HIPAA

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Mientras AWS proporciona servicios elegibles para HIPAA y firma Acuerdos de Asociado de Negocio (BAAs), los clientes son responsables de usar estos servicios apropiadamente e implementar salvaguardas apropiadas para PHI.
</details>

### Pregunta 25
**Una empresa quiere implementar cifrado para datos almacenados en S3. Necesitan mantener control sobre las claves de cifrado y quieren usar su propia infraestructura de gestión de claves. ¿Qué opción de cifrado S3 deberían elegir?**

- A) SSE-S3 (Cifrado del Lado del Servidor con Claves Gestionadas por S3)
- B) SSE-KMS (Cifrado del Lado del Servidor con AWS KMS)
- C) SSE-C (Cifrado del Lado del Servidor con Claves Proporcionadas por el Cliente)
- D) Cifrado del lado del cliente

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: SSE-C permite a los clientes proporcionar sus propias claves de cifrado para que S3 las use para cifrado/descifrado, dándoles control completo sobre la gestión de claves mientras aún se benefician del cifrado del lado del servidor.
</details>

### Pregunta 26
**Una empresa tiene múltiples cuentas de AWS y quiere implementar políticas de seguridad centralizadas en todas las cuentas. Quieren prevenir que cualquier cuenta lance instancias en ciertas regiones. ¿Qué deberían usar?**

- A) Políticas IAM en cada cuenta
- B) AWS Organizations con Políticas de Control de Servicio (SCPs)
- C) Reglas AWS Config en cada cuenta
- D) Grupos de Seguridad en cada cuenta

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS Organizations con Políticas de Control de Servicio (SCPs) pueden hacer cumplir políticas centralizadas a través de múltiples cuentas, incluyendo restringir acciones en regiones específicas independientemente de otros permisos.
</details>

### Pregunta 27
**Una aplicación web está experimentando un ataque DDoS dirigido a la capa de aplicación con solicitudes HTTP complejas. ¿Qué servicios de AWS proporcionarían la mejor protección? (Selecciona DOS)**

- A) AWS Shield Standard
- B) AWS Shield Advanced
- C) AWS WAF
- D) Amazon GuardDuty
- E) AWS Config

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B, C**

**Explicación**: AWS Shield Advanced proporciona protección DDoS mejorada con soporte 24/7, y AWS WAF puede filtrar tráfico malicioso de capa de aplicación basado en patrones de solicitud, IPs y otros criterios.
</details>

### Pregunta 28
**Un administrador de base de datos quiere asegurar que las conexiones de base de datos estén cifradas en tránsito. Para una base de datos Amazon RDS MySQL, ¿qué deberían verificar?**

- A) La base de datos está cifrada en reposo
- B) SSL/TLS está habilitado y forzado para conexiones
- C) La base de datos está en una subred privada
- D) Las copias de seguridad de la base de datos están cifradas

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: El cifrado en tránsito para conexiones de base de datos se logra a través de SSL/TLS. RDS soporta conexiones SSL/TLS, pero debe ser forzado para asegurar que todas las conexiones estén cifradas.
</details>

### Pregunta 29
**Una empresa quiere monitorear cambios en las configuraciones de su infraestructura AWS y recibir alertas cuando los recursos estén configurados fuera de los estándares de cumplimiento. ¿Qué servicio es más apropiado?**

- A) AWS CloudTrail
- B) AWS Config
- C) AWS CloudWatch
- D) AWS Systems Manager

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS Config monitorea configuraciones de recursos, las evalúa contra configuraciones deseadas y reglas de cumplimiento, y puede disparar alertas cuando los recursos se desvían de estados conformes.
</details>

### Pregunta 30
**Una aplicación ejecutándose en EC2 necesita acceder a buckets S3. El equipo de seguridad quiere asegurar que no se almacenen credenciales a largo plazo en las instancias EC2. ¿Cuál es el enfoque más seguro?**

- A) Almacenar claves de acceso en variables de entorno
- B) Usar roles IAM adjuntos a instancias EC2
- C) Codificar credenciales en la aplicación
- D) Almacenar credenciales en un archivo de configuración

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Los roles IAM adjuntos a instancias EC2 proporcionan credenciales temporales que se rotan automáticamente, eliminando la necesidad de almacenar credenciales a largo plazo en las instancias.
</details>

### Pregunta 31
**Una empresa quiere detectar y responder a amenazas de seguridad en su entorno AWS automáticamente. Necesitan un servicio que pueda identificar instancias comprometidas y direcciones IP maliciosas. ¿Qué servicio deberían implementar?**

- A) AWS CloudTrail
- B) AWS Config
- C) AWS GuardDuty
- D) AWS Inspector

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: AWS GuardDuty es un servicio de detección de amenazas que usa aprendizaje automático para identificar actividad maliciosa, instancias comprometidas y comunicación con direcciones IP maliciosas.
</details>

### Pregunta 32
**Una institución financiera necesita asegurar que sus datos S3 estén cifrados en reposo y que mantengan control sobre las claves de cifrado. Quieren que AWS maneje el proceso de cifrado pero mantener la gestión de claves bajo su control. ¿Qué opción deberían elegir?**

- A) SSE-S3
- B) SSE-KMS con claves gestionadas por el cliente
- C) SSE-C
- D) Sin cifrado

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: SSE-KMS con claves gestionadas por el cliente permite a AWS manejar el proceso de cifrado mientras los clientes mantienen control sobre las claves de cifrado a través de AWS KMS.
</details>

### Pregunta 33
**¿Cuál es el beneficio de seguridad principal de habilitar AWS CloudTrail en todas las Regiones de AWS?**

- A) Mejora el rendimiento de la aplicación
- B) Proporciona un rastro de auditoría integral de todas las actividades API a través de todas las regiones
- C) Reduce costos consolidando registros
- D) Arregla automáticamente problemas de seguridad

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: CloudTrail habilitado en todas las regiones asegura que todas las llamadas API y actividades sean registradas independientemente de dónde ocurran, proporcionando visibilidad completa para auditoría de seguridad y cumplimiento.
</details>

### Pregunta 34
**Una empresa necesita asegurar que sus instancias EC2 cumplan con estándares de seguridad y estén libres de vulnerabilidades conocidas. ¿Qué servicio de AWS proporciona evaluaciones de seguridad automatizadas para instancias EC2?**

- A) AWS GuardDuty
- B) AWS Inspector
- C) AWS Config
- D) AWS Systems Manager

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS Inspector evalúa automáticamente instancias EC2 e imágenes de contenedor para vulnerabilidades y desviaciones de mejores prácticas de seguridad y estándares de cumplimiento.
</details>

### Pregunta 35
**Una empresa multinacional debe cumplir con GDPR para los datos de sus clientes europeos. Quieren asegurar que los datos de clientes europeos sean procesados solo en regiones de la UE. ¿Cómo deberían arquitecturar su infraestructura AWS?**

- A) Usar una sola región global para todos los datos
- B) Desplegar infraestructura separada en regiones de la UE para clientes europeos y configurar el procesamiento de datos en consecuencia
- C) Cifrar todos los datos independientemente de la ubicación
- D) Usar CloudFront para servir a todos los clientes desde regiones de la UE

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: GDPR requiere protección de datos y tiene requisitos específicos sobre ubicaciones de procesamiento de datos. Desplegar infraestructura en regiones de la UE para clientes europeos ayuda a asegurar el cumplimiento GDPR para residencia y procesamiento de datos.
</details>

### Pregunta 36
**¿Cuál es la ventaja de seguridad más significativa de usar roles IAM de AWS sobre usuarios IAM para aplicaciones?**

- A) Los roles son más baratos que los usuarios
- B) Los roles proporcionan más permisos que los usuarios
- C) Los roles usan credenciales temporales que se rotan automáticamente
- D) Los roles pueden compartirse entre múltiples aplicaciones

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Los roles IAM proporcionan credenciales temporales que se rotan automáticamente, eliminando los riesgos de seguridad asociados con claves de acceso a largo plazo y reduciendo la superficie de ataque.
</details>

---

## ⚙️ Dominio 3: Tecnología y Servicios de la Nube (Preguntas 37-58)

### Pregunta 37
**Una empresa de medios necesita procesar archivos de video subidos por usuarios. El tiempo de procesamiento varía significativamente (de 30 segundos a 2 horas) y ocurre infrecuentemente. Quieren minimizar costos mientras aseguran que el procesamiento pueda escalar para manejar múltiples subidas simultáneamente. ¿Qué opción de cómputo es más apropiada?**

- A) Instancias EC2 On-Demand ejecutándose 24/7
- B) Instancias EC2 Reservadas
- C) AWS Lambda con límites de tiempo extendidos
- D) AWS Batch con instancias Spot

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: D**

**Explicación**: AWS Batch con instancias Spot es ideal para trabajos de procesamiento por lotes de larga duración y duración variable. Puede escalar automáticamente y usar instancias Spot para ahorros significativos de costos en cargas de trabajo tolerantes a fallos.
</details>

### Pregunta 38
**Una aplicación IoT necesita almacenar millones de lecturas de sensores por día. Los datos necesitan ser consultables en tiempo real y deberían escalar automáticamente para manejar cargas variables. ¿Qué solución de base de datos es más apropiada?**

- A) Amazon RDS con réplicas de lectura
- B) Amazon DynamoDB
- C) Amazon Redshift
- D) Amazon Aurora

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: DynamoDB está diseñado para aplicaciones de alta escala con millones de solicitudes por segundo, proporciona capacidades de consulta en tiempo real, y escala automáticamente para manejar cargas variables sin intervención manual.
</details>

### Pregunta 39
**Una empresa quiere construir una API sin servidor que pueda manejar picos repentinos de tráfico sin ninguna gestión de servidor. La API necesita integrarse con múltiples servicios backend y bases de datos. ¿Qué combinación de servicios es más apropiada?**

- A) EC2 + Application Load Balancer + RDS
- B) API Gateway + Lambda + DynamoDB
- C) ECS + ALB + Aurora
- D) Elastic Beanstalk + RDS

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: API Gateway + Lambda + DynamoDB proporciona una arquitectura completamente sin servidor que escala automáticamente, no requiere gestión de servidor, y puede manejar picos repentinos de tráfico con escalado automático.
</details>

### Pregunta 40
**Una aplicación de comercio financiero requiere latencia extremadamente baja (sub-milisegundo) para operaciones de base de datos. ¿Qué opción de almacenamiento proporcionaría el mejor rendimiento?**

- A) Amazon S3
- B) Amazon EFS
- C) Amazon EBS con IOPS Aprovisionados
- D) Almacenamiento de instancia (almacenamiento SSD local)

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: D**

**Explicación**: El almacenamiento de instancia proporciona el almacenamiento de menor latencia ya que está físicamente conectado a la computadora host, ofreciendo rendimiento NVMe SSD con latencia sub-milisegundo para aplicaciones de ultra-alto rendimiento.
</details>

### Pregunta 41
**Una empresa necesita migrar 500TB de datos desde su centro de datos local a S3. Su conexión a internet tiene ancho de banda limitado y no pueden permitirse semanas de transferencia de datos afectando sus operaciones comerciales. ¿Cuál es la estrategia de migración más eficiente?**

- A) Usar AWS Direct Connect para transferencia más rápida
- B) Usar AWS DataSync sobre internet
- C) Usar dispositivos AWS Snowball Edge
- D) Usar S3 Transfer Acceleration

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Para conjuntos de datos grandes (500TB), los dispositivos AWS Snowball Edge proporcionan el método de transferencia más eficiente sin consumir ancho de banda de internet y significativamente más rápido que las transferencias basadas en red.
</details>

### Pregunta 42
**Una arquitectura de microservicios necesita entrega confiable de mensajes entre servicios, con la capacidad de manejar fallas de mensajes y reintentos. Los mensajes deberían procesarse en orden para cada cliente. ¿Qué combinación de servicios es más apropiada?**

- A) Amazon SNS para toda la mensajería
- B) Colas Amazon SQS Standard
- C) Colas Amazon SQS FIFO
- D) Amazon Kinesis Data Streams

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Las colas SQS FIFO aseguran que los mensajes se procesen en orden (importante para el ordenamiento por cliente) y proporcionan procesamiento exactamente una vez con mecanismos de reintento incorporados para entrega confiable de mensajes.
</details>

### Pregunta 43
**Una aplicación de comercio electrónico global sirve a clientes en todo el mundo y necesita proporcionar tiempos de respuesta rápidos independientemente de la ubicación del usuario. La aplicación tiene contenido dinámico que debe personalizarse para cada usuario. ¿Qué patrón de arquitectura sería más efectivo?**

- A) Despliegue de una sola región con CloudFront
- B) Despliegue multi-región con CloudFront y failover de origen
- C) Una sola región con múltiples Zonas de Disponibilidad
- D) Despliegue multi-región sin CloudFront

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: El despliegue multi-región asegura baja latencia globalmente, mientras CloudFront puede almacenar en caché contenido estático y enrutar solicitudes dinámicas a la región más cercana, con failover de origen proporcionando alta disponibilidad.
</details>

### Pregunta 44
**Un equipo de analítica de datos necesita ejecutar consultas SQL complejas en grandes conjuntos de datos (petabytes) almacenados en S3. Quieren una solución que no requiera gestionar infraestructura y pueda escalar automáticamente basándose en la complejidad de la consulta. ¿Qué servicio es más adecuado?**

- A) Amazon EMR
- B) Amazon Athena
- C) Amazon Redshift
- D) Amazon RDS

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Amazon Athena es un servicio de consulta sin servidor que te permite ejecutar consultas SQL directamente en datos almacenados en S3 sin gestionar infraestructura, y escala automáticamente basándose en la complejidad de la consulta.
</details>

### Pregunta 45
**Una empresa de juegos móviles necesita implementar tableros de clasificación en tiempo real que puedan manejar millones de jugadores concurrentes actualizando sus puntuaciones. La solución debe proporcionar clasificaciones en tiempo real y escalar automáticamente. ¿Qué combinación sería la más adecuada?**

- A) RDS con réplicas de lectura
- B) DynamoDB con DynamoDB Streams + Lambda
- C) ElastiCache con escalado manual
- D) S3 con CloudFront

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: DynamoDB puede manejar millones de actualizaciones concurrentes con escalado automático, y DynamoDB Streams con Lambda puede disparar actualizaciones de tableros de clasificación en tiempo real y cálculos de rankings.
</details>

### Pregunta 46
**Una empresa quiere implementar una estrategia de recuperación ante desastres para su aplicación crítica. Necesitan un RTO (Objetivo de Tiempo de Recuperación) de menos de 1 hora y RPO (Objetivo de Punto de Recuperación) de menos de 15 minutos. ¿Qué enfoque cumpliría estos requisitos?**

- A) Respaldo y restauración usando S3
- B) Luz piloto con failover automatizado
- C) Standby cálido en otra región
- D) Despliegue multi-sitio activo/activo

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: El standby cálido mantiene una versión reducida del entorno que puede escalarse rápidamente, cumpliendo el requisito RTO <1 hora, con replicación continua de datos cumpliendo el requisito RPO <15 minutos.
</details>

### Pregunta 47
**Una empresa necesita implementar un sistema de gestión de contenido donde los usuarios suben archivos de video grandes (hasta 100GB cada uno). El sistema debería proporcionar subidas reanudables y manejar fallas de subida elegantemente. ¿Qué característica de S3 es más apropiada?**

- A) S3 Transfer Acceleration
- B) S3 Multipart Upload
- C) S3 Cross-Region Replication
- D) S3 Intelligent Tiering

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: S3 Multipart Upload permite que archivos grandes se suban en partes, habilitando subidas reanudables y subidas paralelas para mejor rendimiento y resistencia a fallas.
</details>

### Pregunta 48
**Un equipo de aprendizaje automático necesita procesar datos de streaming en tiempo real para detectar transacciones fraudulentas. Necesitan analizar datos conforme llegan y disparar alertas inmediatas. ¿Qué combinación de servicios es más apropiada?**

- A) S3 + Lambda
- B) Kinesis Data Streams + Kinesis Analytics + Lambda
- C) SQS + EC2
- D) DynamoDB + CloudWatch

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Kinesis Data Streams ingiere datos en tiempo real, Kinesis Analytics los procesa en tiempo real usando consultas SQL, y Lambda puede disparar alertas inmediatas basadas en los resultados del análisis.
</details>

### Pregunta 49
**Una empresa quiere implementar Infraestructura como Código (IaC) para gestionar sus recursos de AWS con control de versiones y capacidades de rollback. ¿Qué servicio sería más apropiado?**

- A) AWS Systems Manager
- B) AWS CloudFormation
- C) AWS Config
- D) AWS OpsWorks

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS CloudFormation habilita Infraestructura como Código usando plantillas JSON o YAML, proporciona control de versiones a través del versionado de plantillas, y soporta capacidades de rollback para despliegues fallidos.
</details>

### Pregunta 50
**Una aplicación web experimenta patrones de tráfico predecibles con altas cargas durante horas de oficina (8 AM - 6 PM) y bajas cargas durante noches y fines de semana. ¿Qué estrategia de escalado sería más costo-efectiva?**

- A) Escalado manual basado en tiempo
- B) Auto Scaling programado con seguimiento de objetivos
- C) Solo Auto Scaling reactivo
- D) Sobre-aprovisionamiento para cargas pico

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: El Auto Scaling programado puede escalar recursos proactivamente basándose en patrones predecibles, combinado con seguimiento de objetivos para variaciones inesperadas, proporcionando el enfoque más costo-efectivo para cargas de trabajo predecibles.
</details>

### Pregunta 51
**Una empresa necesita asegurar que su aplicación web de múltiples niveles esté altamente disponible a través de múltiples Zonas de Disponibilidad. Quieren failover automático y verificación de salud. ¿Qué servicio proporciona esta capacidad?**

- A) Amazon Route 53
- B) Application Load Balancer
- C) CloudFront
- D) Auto Scaling

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Application Load Balancer distribuye automáticamente el tráfico a través de múltiples AZs, realiza verificaciones de salud, y automáticamente enruta el tráfico lejos de instancias no saludables, proporcionando alta disponibilidad.
</details>

### Pregunta 52
**Un equipo de ciencia de datos necesita analizar archivos de log almacenados en S3. El análisis es intensivo en CPU y se ejecuta por varias horas. Quieren usar un servicio gestionado que pueda aprovisionar automáticamente recursos de cómputo y manejar colas de trabajos. ¿Qué servicio es más apropiado?**

- A) AWS Lambda
- B) Amazon EMR
- C) AWS Batch
- D) Amazon ECS

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: AWS Batch está diseñado para cargas de trabajo de computación por lotes de larga duración, aprovisiona automáticamente recursos de cómputo, maneja colas de trabajos, y es ideal para tareas intensivas en CPU que se ejecutan por horas.
</details>

### Pregunta 53
**Una empresa quiere implementar una arquitectura de microservicios donde los servicios puedan descubrirse y comunicarse entre sí automáticamente. Quieren capacidades de service mesh para observabilidad y gestión de tráfico. ¿Qué combinación funcionaría mejor?**

- A) ECS + Application Load Balancer
- B) EKS + AWS App Mesh
- C) Lambda + API Gateway
- D) EC2 + Route 53

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: EKS (Kubernetes gestionado) proporciona una plataforma para microservicios, y AWS App Mesh proporciona capacidades de service mesh incluyendo descubrimiento de servicios, gestión de tráfico, y observabilidad.
</details>

### Pregunta 54
**Una empresa de servicios financieros necesita procesar datos de transacciones en tiempo real y almacenarlos en un almacén de datos para analítica. Necesitan garantías de procesamiento exactamente una vez y la capacidad de reproducir datos si es necesario. ¿Qué arquitectura es más apropiada?**

- A) Kinesis Data Streams + Kinesis Data Firehose + Redshift
- B) SQS + Lambda + DynamoDB
- C) SNS + SQS + RDS
- D) S3 + Athena + QuickSight

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: A**

**Explicación**: Kinesis Data Streams proporciona procesamiento exactamente una vez y capacidades de reproducción, Kinesis Data Firehose entrega datos de manera confiable a Redshift para analítica, cumpliendo todos los requisitos para procesamiento en tiempo real y almacenamiento.
</details>

### Pregunta 55
**Una empresa necesita monitorear el rendimiento de aplicaciones, rastrear solicitudes a través de múltiples servicios, e identificar cuellos de botella en su arquitectura distribuida. ¿Qué servicio proporciona información detallada de aplicaciones y rastreo de solicitudes?**

- A) CloudWatch Metrics
- B) CloudTrail
- C) AWS X-Ray
- D) Config

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: AWS X-Ray proporciona capacidades de rastreo distribuido, permitiéndote rastrear solicitudes a través de múltiples servicios, analizar cuellos de botella de rendimiento, y obtener información detallada sobre el comportamiento de aplicaciones.
</details>

### Pregunta 56
**Un equipo de desarrollo necesita implementar una aplicación web rápidamente sin gestionar servidores o infraestructura. Quieren escalado automático, equilibrio de carga y gestión de plataforma. ¿Qué servicio es más apropiado para despliegue rápido?**

- A) Amazon EC2
- B) AWS Elastic Beanstalk
- C) Amazon ECS
- D) AWS Lambda

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS Elastic Beanstalk es una oferta PaaS que maneja despliegue, escalado, equilibrio de carga, y gestión de plataforma automáticamente, permitiendo a los desarrolladores enfocarse en el código en lugar de la infraestructura.
</details>

### Pregunta 57
**Una empresa quiere implementar una arquitectura híbrida donde sus aplicaciones on-premises puedan acceder sin problemas a los servicios de AWS como si estuvieran en la red local. ¿Qué servicio proporciona esta capacidad?**

- A) VPN Gateway
- B) AWS Direct Connect
- C) Internet Gateway
- D) AWS Outposts

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: D**

**Explicación**: AWS Outposts trae servicios de AWS a ubicaciones on-premises, permitiendo que las aplicaciones accedan a servicios de AWS localmente con APIs y gestión consistentes, creando una experiencia verdaderamente híbrida.
</details>

### Pregunta 58
**Una empresa de streaming de medios necesita transcodificar archivos de video en múltiples formatos y resoluciones. La carga de trabajo es esporádica e intensiva en cómputo. Quieren una solución completamente gestionada que escale automáticamente. ¿Qué servicio es más adecuado?**

- A) EC2 con Auto Scaling
- B) AWS Elemental MediaConvert
- C) AWS Lambda
- D) Amazon ECS con Fargate

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS Elemental MediaConvert es un servicio de transcodificación de video completamente gestionado que escala automáticamente para manejar cargas de trabajo variables y está específicamente diseñado para flujos de trabajo de procesamiento de medios.
</details>

---

## 💰 Dominio 4: Facturación y Soporte (Preguntas 59-65)

### Pregunta 59
**Una empresa tiene una carga de trabajo mixta con algunas aplicaciones predecibles de estado estable y algunas cargas de trabajo variables y experimentales. Quieren optimizar costos mientras mantienen flexibilidad. ¿Qué estrategia de precios sería más efectiva?**

- A) Usar Instancias Reservadas para todo
- B) Usar Instancias Spot para todo
- C) Usar Instancias Reservadas para cargas de trabajo estables y On-Demand para cargas de trabajo variables
- D) Usar solo Instancias On-Demand

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Usar Instancias Reservadas para cargas de trabajo predecibles proporciona ahorros de costos (hasta 75%), mientras que las instancias On-Demand para cargas de trabajo variables proporcionan flexibilidad sin compromisos a largo plazo.
</details>

### Pregunta 60
**Una startup en crecimiento espera que su uso de AWS aumente significativamente pero no está segura de qué tipos de instancia específicos necesitará. Quieren ahorros de costos con flexibilidad para cambiar familias de instancias. ¿Qué opción proporciona el mejor equilibrio?**

- A) Instancias Reservadas Estándar
- B) Instancias Reservadas Convertibles
- C) Compute Savings Plans
- D) EC2 Instance Savings Plans

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: C**

**Explicación**: Los Compute Savings Plans proporcionan la mayor flexibilidad a través de familias de instancias, tamaños y regiones mientras aún ofrecen ahorros significativos (hasta 66%), ideal para empresas en crecimiento con necesidades cambiantes.
</details>

### Pregunta 61
**Una empresa quiere implementar seguimiento detallado de costos a través de múltiples departamentos y proyectos. Necesitan entender patrones de gasto y asignar costos con precisión. ¿Qué deberían implementar primero?**

- A) AWS Budgets
- B) Etiquetas de asignación de costos
- C) AWS Cost Explorer
- D) Recomendaciones de Instancias Reservadas

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: Las etiquetas de asignación de costos son la base para el seguimiento detallado de costos. Deben implementarse primero para habilitar la atribución precisa de costos por departamento, proyecto u otras dimensiones de negocio.
</details>

### Pregunta 62
**La factura mensual de AWS de una empresa ha aumentado repentinamente un 200% sin cambios conocidos en su infraestructura. ¿Qué servicio les ayudaría a identificar rápidamente la causa de este aumento?**

- A) AWS Trusted Advisor
- B) AWS Cost Explorer con agrupación por servicio y tiempo
- C) AWS Budgets
- D) AWS Pricing Calculator

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS Cost Explorer puede mostrar rápidamente tendencias de costos a lo largo del tiempo agrupadas por servicio, ayudando a identificar qué servicios causaron el aumento repentino y cuándo ocurrió el cambio.
</details>

### Pregunta 63
**Una empresa necesita soporte 24/7 para su aplicación de misión crítica con tiempos de respuesta garantizados de menos de 15 minutos para problemas críticos. ¿Qué plan de soporte cumple este requisito?**

- A) Basic Support
- B) Developer Support
- C) Business Support
- D) Enterprise Support

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: D**

**Explicación**: Solo Enterprise Support proporciona soporte 24/7 con tiempos de respuesta de menos de 15 minutos para casos de caída de sistemas críticos de negocio. Business Support proporciona respuesta de 1 hora para problemas críticos.
</details>

### Pregunta 64
**Una empresa quiere entender sus ahorros potenciales por usar Instancias Reservadas. Necesitan recomendaciones basadas en sus patrones de uso reales. ¿Qué herramienta proporciona este análisis?**

- A) AWS Pricing Calculator
- B) Recomendaciones de Instancias Reservadas de AWS Cost Explorer
- C) AWS Trusted Advisor
- D) AWS Budgets

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: B**

**Explicación**: AWS Cost Explorer proporciona recomendaciones de Instancias Reservadas basadas en tus patrones de uso reales, mostrando ahorros potenciales y estrategias óptimas de compra de RI.
</details>

### Pregunta 65
**Una empresa quiere hacer cumplir automáticamente límites de gasto a través de su organización para prevenir sobrecostos. Necesitan la capacidad de restringir automáticamente el lanzamiento de nuevos recursos cuando se excedan los presupuestos. ¿Qué combinación de servicios deberían usar?**

- A) AWS Budgets + AWS Organizations Service Control Policies
- B) Cost Explorer + políticas IAM
- C) Trusted Advisor + alarmas CloudWatch
- D) Alertas de facturación + intervención manual

<details>
<summary>Haz clic para revelar la respuesta</summary>

**Respuesta: A**

**Explicación**: AWS Budgets puede disparar alertas cuando se excedan los umbrales, y las Service Control Policies a través de AWS Organizations pueden restringir automáticamente el lanzamiento de recursos, proporcionando cumplimiento automatizado de control de costos.
</details>

---

## 📊 Examen de Práctica 3 - Clave de Respuestas

### Dominio 1: Conceptos de la Nube (16/16)
1. B | 2. B | 3. C | 4. B | 5. B | 6. C | 7. B | 8. C | 9. B | 10. B | 11. B | 12. B | 13. B | 14. B | 15. A | 16. B

### Dominio 2: Seguridad y Cumplimiento (20/20)
17. B | 18. B | 19. B | 20. A,B | 21. C | 22. B | 23. C | 24. B | 25. C | 26. B | 27. B,C | 28. B | 29. B | 30. B | 31. C | 32. B | 33. B | 34. B | 35. B | 36. C

### Dominio 3: Tecnología y Servicios de la Nube (22/22)
37. D | 38. B | 39. B | 40. D | 41. C | 42. C | 43. B | 44. B | 45. B | 46. C | 47. B | 48. B | 49. B | 50. B | 51. B | 52. C | 53. B | 54. A | 55. C | 56. B | 57. D | 58. B

### Dominio 4: Facturación y Soporte (7/7)
59. C | 60. C | 61. B | 62. B | 63. D | 64. B | 65. A

---

## 🎯 Evaluación Final y Verificación de Preparación

**Calcula tu puntuación:**
- Cuenta respuestas correctas: ___/65
- Porcentaje: (Respuestas correctas ÷ 65) × 100 = ___%
- **Puntuación de Aprobación**: 70% (46/65 correctas)

### 📈 Análisis Integral de Rendimiento

**95-100% (62-65 correctas)**: 🏆 **¡Listo para el Examen!** Estás completamente preparado para el examen AWS Cloud Practitioner.

**90-94% (59-61 correctas)**: 🌟 **¡Casi Perfecto!** Se recomienda revisión menor, luego programa tu examen.

**85-89% (55-58 correctas)**: ✅ **¡Muy Fuerte!** Revisa conceptos perdidos y estarás listo.

**80-84% (52-54 correctas)**: 📚 **Buena Base.** Enfócate en áreas débiles, retoma exámenes de práctica.

**70-79% (46-51 correctas)**: ⚠️ **Límite.** Se necesita revisión significativa antes del examen.

**Debajo del 70% (<46 correctas)**: 📖 **Se Requiere Más Estudio.** Regresa a materiales de estudio, construye una base más sólida.

### 🎯 Seguimiento de Rendimiento por Dominio

| Dominio | Tu Puntuación | Objetivo | Estado |
|---------|---------------|----------|--------|
| Conceptos de la Nube (16 preguntas) | ___/16 (___%) | 80%+ | ⚪ |
| Seguridad y Cumplimiento (20 preguntas) | ___/20 (___%) | 80%+ | ⚪ |
| Tecnología y Servicios (22 preguntas) | ___/22 (___%) | 80%+ | ⚪ |
| Facturación y Soporte (7 preguntas) | ___/7 (___%) | 80%+ | ⚪ |

### 🚀 Recomendaciones de Preparación Final

#### **Si obtuviste 85%+ en general:**
1. ✅ **Programa tu examen** - ¡estás listo!
2. 📖 Revisa [Guía de Referencia Rápida](../quick-reference/service-cheatsheet.md)
3. 🧠 Practica [Consejos de Examen](../quick-reference/exam-tips.md)
4. 💪 Toma el examen real con confianza

#### **Si obtuviste 70-84% en general:**
1. 📚 **Enfócate en dominios débiles** (< 75% de puntuación)
2. 🔄 **Retoma cuestionarios de capítulos específicos**
3. 📝 **Revisa preguntas perdidas minuciosamente**
4. ⏰ **Espera 3-5 días, luego retoma un examen de práctica**

#### **Si obtuviste menos del 70%:**
1. 📖 **Regresa a materiales de estudio**
2. 🎯 **Enfócate en conceptos fundamentales**
3. ⏳ **Permite 1-2 semanas de estudio adicional**
4. 🔄 **Retoma el Examen de Práctica 1 cuando estés listo**

---

## 🎓 ¡Viaje de Certificación Completado!

**¡Felicitaciones por completar los tres exámenes de práctica!** 

Ahora has experimentado:
- ✅ **195 preguntas de práctica únicas** a través de todos los dominios del examen
- ✅ **Escenarios de examen reales** y patrones de preguntas
- ✅ **Explicaciones detalladas** para cada respuesta
- ✅ **Seguimiento de rendimiento** a través de todas las áreas de conocimiento

### 🏆 Próximos Pasos hacia el Éxito en la Certificación

1. **📅 Programa Tu Examen**: Si obtienes consistentemente 80%+
2. **📚 Revisión Final**: Usa nuestros [materiales de Referencia Rápida](../quick-reference/)
3. **🧠 Preparación Mental**: Revisa [Consejos y Estrategias de Examen](../quick-reference/exam-tips.md)
4. **🎯 Toma el Examen Real**: ¡Puedes hacerlo!

### 📞 Recuerda:
- El examen real tiene el mismo formato y dificultad
- Confía en tu preparación e instintos
- Tómate tu tiempo y lee las preguntas cuidadosamente
- ¡Estás bien preparado para el éxito! 

**¡Buena suerte con tu examen AWS Certified Cloud Practitioner! 🌟**

---

*¡Tu viaje hacia el éxito en la certificación AWS está casi completo! 🚀*
