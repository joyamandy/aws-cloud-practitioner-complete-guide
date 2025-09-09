# 🤝 Modelo de Responsabilidad Compartida

> **"AWS asegura la nube, tú aseguras EN la nube" - La base de toda la seguridad de AWS**

## 🎯 Resumen del Capítulo

**Tiempo de Estudio:** ~4 horas  
**Dificultad:** Principiante a Intermedio  
**Importancia:** ⭐⭐⭐⭐⭐ (¡Absolutamente crítico!)

El Modelo de Responsabilidad Compartida es el **concepto de seguridad más importante** en AWS. Es la base para todo lo que aprenderás sobre seguridad en la nube. Si no entiendes esto correctamente, podrías dejar brechas críticas de seguridad en tu infraestructura.

---

## 📋 Tabla de Contenidos

- [🏠 La Analogía de la Casa](#-la-analogía-de-la-casa)
- [📊 El Modelo Explicado](#-el-modelo-explicado)
- [⚙️ Responsabilidades Específicas por Servicio](#️-responsabilidades-específicas-por-servicio)
- [🛡️ Categorías de Controles de Seguridad](#️-categorías-de-controles-de-seguridad)
- [⚠️ Conceptos Erróneos Comunes](#️-conceptos-erróneos-comunes)
- [📝 Escenarios del Mundo Real](#-escenarios-del-mundo-real)
- [✅ Mejores Prácticas](#-mejores-prácticas)

---

## 🏠 La Analogía de la Casa

### 🏡 **Entendiendo a Través de Bienes Raíces**

Piensa en AWS como un **edificio de apartamentos de lujo** y tú eres un **inquilino**:

#### 🏢 **AWS (El Propietario del Edificio) es Responsable De:**
- 🏗️ **Estructura del edificio** - Cimientos, paredes, techo (Infraestructura física)
- ⚡ **Servicios públicos** - Electricidad, agua, calefacción (Energía, refrigeración, redes)
- 🛡️ **Seguridad del edificio** - Entrada con llave, cámaras de seguridad (Seguridad física)
- 🚪 **Áreas comunes** - Vestíbulo, ascensores, pasillos (Infraestructura compartida)
- 🔧 **Mantenimiento** - HVAC, plomería, reparaciones estructurales (Mantenimiento de hardware)
- 🏢 **Administración de la propiedad** - Operaciones y gestión del edificio

#### 🏠 **Tú (El Inquilino) eres Responsable De:**
- 🪑 **Tus muebles** - Lo que pones en tu apartamento (Tus datos y aplicaciones)
- 🔐 **Tus cerraduras** - Cambiar las cerraduras de tu apartamento (Controles de acceso y contraseñas)
- 🧹 **Limpieza** - Mantener tu espacio limpio (Gestión y organización de datos)
- 👥 **Tus invitados** - A quién dejas entrar a tu apartamento (Gestión de acceso de usuarios)
- 📱 **Tus dispositivos** - Tu TV, computadora, teléfono (Aplicaciones y sistemas operativos)
- 🚪 **Seguridad del apartamento** - Cerrar tu puerta, cerrar ventanas (Seguridad a nivel de aplicación)

#### 🤝 **Responsabilidades Compartidas:**
- 🔥 **Seguridad contra incendios** - El edificio tiene rociadores, tú necesitas detectores de humo
- 🚨 **Conciencia de seguridad** - El edificio tiene cámaras, tú necesitas estar vigilante
- 📋 **Comunicación** - El edificio publica avisos, tú necesitas leerlos

---

## 📊 El Modelo Explicado

### 🔄 **El Principio Fundamental**

```
Responsabilidad de AWS = "Seguridad DE la Nube"
↓
Infraestructura física, hardware, software que ejecuta los servicios de AWS

Responsabilidad del Cliente = "Seguridad EN la Nube"
↓
Todo lo que pones en la nube y cómo lo configuras
```

### 📈 **Desglose Visual**

```
┌─────────────────────────────────────────────────────────┐
│                RESPONSABILIDAD DEL CLIENTE              │
│                   "Seguridad EN la Nube"               │
├─────────────────────────────────────────────────────────┤
│  Datos del Cliente                                      │
│  Plataforma, Aplicaciones, Gestión de Identidad y      │
│  Acceso, Sistema Operativo, Configuración de Red y     │
│  Firewall, Cifrado de Datos del Cliente e Integridad  │
│  Cifrado del Lado del Servidor (Sistema de Archivos    │
│  y/o Datos), Protección del Tráfico de Red             │
├─────────────────────────────────────────────────────────┤
│                  RESPONSABILIDAD DE AWS                 │
│                   "Seguridad DE la Nube"               │
├─────────────────────────────────────────────────────────┤
│  Software                                               │
│  Cómputo | Almacenamiento | Base de Datos | Redes      │
│  Hardware/Infraestructura Global de AWS                │
│  Regiones | Zonas de Disponibilidad | Edge Locations   │
└─────────────────────────────────────────────────────────┘
```

### 🛡️ **AWS Asegura (Seguridad DE la Nube)**

#### 🏗️ **Infraestructura Física**
- **Centros de datos** - Seguridad física, controles de acceso, controles ambientales
- **Hardware** - Servidores, dispositivos de almacenamiento, equipo de red
- **Instalaciones** - Energía, refrigeración, supresión de incendios, monitoreo físico
- **Seguridad geográfica** - Múltiples regiones y zonas de disponibilidad

#### 💻 **Servicios Fundamentales**
- **Servicios de cómputo** - Hipervisor EC2, entorno de ejecución Lambda
- **Servicios de almacenamiento** - Infraestructura S3, sistemas backend EBS
- **Servicios de base de datos** - Infraestructura subyacente RDS, plataforma DynamoDB
- **Redes** - Infraestructura VPC, plataformas de balanceadores de carga

#### 🔧 **Operaciones de Servicios**
- **Gestión de parches** - Actualizaciones de servicios AWS y parches de seguridad
- **Gestión de configuración** - Configuraciones de seguridad por defecto
- **Sistemas de monitoreo** - Monitoreo de infraestructura y alertas
- **Respuesta a incidentes** - Gestión de incidentes de seguridad a nivel AWS

### 👤 **Cliente Asegura (Seguridad EN la Nube)**

#### 📊 **Protección de Datos**
- **Clasificación de datos** - Identificar datos sensibles
- **Cifrado de datos** - Elegir e implementar cifrado
- **Controles de acceso a datos** - Quién puede acceder a qué datos
- **Respaldo y recuperación de datos** - Asegurar disponibilidad e integridad de datos

#### 👥 **Gestión de Identidad y Acceso**
- **Gestión de usuarios** - Crear y gestionar cuentas de usuario
- **Asignación de permisos** - Otorgar niveles de acceso apropiados
- **Autenticación multifactor** - Agregar capas extra de seguridad
- **Monitoreo de acceso** - Rastrear quién accede a qué

#### ⚙️ **Seguridad de Aplicaciones y SO**
- **Sistema operativo** - Parches, endurecimiento, configuración
- **Aplicaciones** - Seguridad de código, gestión de vulnerabilidades
- **Configuración de red** - Security groups, ACLs de red
- **Reglas de firewall** - Controlar tráfico de red

#### 🔐 **Cifrado y Gestión de Claves**
- **Opciones de cifrado** - Decidir qué cifrar y cómo
- **Gestión de claves** - Crear, rotar y proteger claves de cifrado
- **Gestión de certificados** - Certificados SSL/TLS para aplicaciones
- **Gestión de credenciales** - Claves API, contraseñas, tokens de acceso

---

## ⚙️ Responsabilidades Específicas por Servicio

El modelo de responsabilidad compartida varía dependiendo del **tipo de servicio** que estés usando:

### 🖥️ **Infraestructura como Servicio (IaaS) - Ejemplo: EC2**

**AWS Gestiona:**
```
✅ Hardware físico e hipervisor
✅ Infraestructura de red
✅ Seguridad física de centros de datos
✅ Parches del sistema operativo host (nivel hipervisor)
```

**Cliente Gestiona:**
```
🔧 Sistema operativo invitado (incluyendo actualizaciones y parches)
🔧 Aplicaciones y sus configuraciones
🔧 Configuración de security groups y firewall
🔧 Gestión de identidad y acceso
🔧 Cifrado de datos y gestión de claves
🔧 Protección del tráfico de red
```

**Ejemplo Real: Servidor Web en EC2**
- **AWS maneja:** El servidor físico, hipervisor, seguridad del centro de datos
- **Tú manejas:** SO Windows/Linux, software del servidor web, certificados SSL, cuentas de usuario

### 🔗 **Plataforma como Servicio (PaaS) - Ejemplo: RDS**

**AWS Gestiona:**
```
✅ Parches del sistema operativo y motor de base de datos
✅ Instalación y configuración del software de base de datos
✅ Automatización de respaldos (cuando está habilitada)
✅ Configuración de alta disponibilidad
✅ Infraestructura física
```

**Cliente Gestiona:**
```
🔧 Cuentas de usuario de base de datos y permisos
🔧 Reglas de firewall a nivel de base de datos (security groups)
🔧 Configuraciones de cifrado de datos
🔧 Configuración de red (VPC, subredes)
🔧 Código de aplicación que se conecta a la base de datos
```

**Ejemplo Real: Base de Datos MySQL en RDS**
- **AWS maneja:** Software MySQL, parches del SO, infraestructura de respaldos
- **Tú manejas:** Usuarios de base de datos, permisos de tablas, seguridad de conexión

### 📱 **Software como Servicio (SaaS) - Ejemplo: WorkMail**

**AWS Gestiona:**
```
✅ Software de aplicación y su configuración
✅ Sistema operativo y entorno de ejecución
✅ Infraestructura física
✅ La mayoría de configuraciones de seguridad
✅ Seguridad del centro de datos
```

**Cliente Gestiona:**
```
🔧 Acceso de usuarios y gestión de identidad
🔧 Clasificación y manejo de datos
🔧 Seguridad del lado del cliente (protección de endpoints)
🔧 Monitoreo de uso y cumplimiento
```

**Ejemplo Real: Amazon WorkMail**
- **AWS maneja:** Software del servidor de correo, filtrado de spam, infraestructura
- **Tú manejas:** Cuentas de usuario, políticas de correo, seguridad de dispositivos cliente

### 📊 **Tabla de Comparación de Responsabilidades**

| **Aspecto** | **EC2 (IaaS)** | **RDS (PaaS)** | **WorkMail (SaaS)** |
|-------------|-----------------|-----------------|----------------------|
| **Infraestructura Física** | AWS | AWS | AWS |
| **Sistema Operativo** | Cliente | AWS | AWS |
| **Aplicaciones** | Cliente | AWS | AWS |
| **Datos** | Cliente | Cliente | Cliente |
| **Gestión de Acceso** | Cliente | Cliente | Cliente |
| **Controles de Red** | Cliente | Cliente | AWS |

---

## 🛡️ Categorías de Controles de Seguridad

AWS organiza los controles de seguridad en tres categorías que ayudan a aclarar el modelo de responsabilidad compartida:

### 🏢 **Controles Heredados**
**Definición:** Controles que el cliente hereda completamente de AWS.

**Ejemplos:**
- **Seguridad física** - Acceso a centros de datos, controles ambientales
- **Disposición de hardware** - Destrucción segura de dispositivos de almacenamiento
- **Energía y refrigeración** - Energía ininterrumpible, control de temperatura
- **Infraestructura de red** - Seguridad de la red troncal

**Acción del Cliente:** **Ninguna requerida** - AWS maneja completamente

### 🤝 **Controles Compartidos**
**Definición:** Controles donde tanto AWS como el cliente tienen responsabilidades.

**Ejemplos:**

#### 🔄 **Gestión de Parches**
- **Responsabilidad de AWS:** Parchear infraestructura y servicios
- **Responsabilidad del Cliente:** Parchear SO invitado y aplicaciones

#### 🎓 **Gestión de Configuración**
- **Responsabilidad de AWS:** Configurar dispositivos de infraestructura
- **Responsabilidad del Cliente:** Configurar sistemas operativos, bases de datos, aplicaciones

#### 🧠 **Conciencia y Capacitación**
- **Responsabilidad de AWS:** Capacitar empleados de AWS
- **Responsabilidad del Cliente:** Capacitar a tus empleados

### 👤 **Controles Específicos del Cliente**
**Definición:** Controles que son únicamente responsabilidad del cliente.

**Ejemplos:**
- **Seguridad de zona** - Qué zonas/regiones de AWS usar
- **Protección del tráfico de red** - Diseño de VPC, security groups
- **Seguridad del sistema operativo** - Acceso de usuarios, parches, endurecimiento
- **Cifrado del lado del servidor** - Elegir métodos de cifrado y claves
- **Cifrado de datos del lado del cliente** - Cifrar datos antes de enviar a AWS

---

## ⚠️ Conceptos Erróneos Comunes

### ❌ **"AWS Maneja Toda la Seguridad"**
**El Mito:** "Como es la nube, AWS se encarga de toda la seguridad."

**La Realidad:** AWS asegura la infraestructura, pero tú debes asegurar tus aplicaciones, datos y configuraciones.

**Impacto Real:** Las empresas han tenido violaciones de datos porque asumieron que AWS protegería bases de datos mal configuradas.

**Escenario de Ejemplo:**
```
❌ Suposición Incorrecta:
"Puse mi base de datos en AWS, así que está automáticamente segura."

✅ Entendimiento Correcto:
"AWS asegura la infraestructura de la base de datos. Yo debo:
- Configurar controles de acceso
- Configurar cifrado
- Gestionar permisos de usuario
- Monitorear logs de acceso"
```

### ❌ **"El Cliente No Tiene Responsabilidades de Seguridad en SaaS"**
**El Mito:** "Con servicios SaaS, no necesito preocuparme por la seguridad."

**La Realidad:** Incluso con SaaS, eres responsable del acceso de usuarios, clasificación de datos y cumplimiento.

**Ejemplo: Amazon WorkSpaces (Escritorio Virtual)**
- **AWS maneja:** Infraestructura de escritorio, parches, seguridad del host
- **Tú manejas:** Acceso de usuarios, datos en escritorios, seguridad de dispositivos cliente

### ❌ **"AWS Me Dirá Si Algo Es Inseguro"**
**El Mito:** "AWS monitorea mi configuración y me alerta sobre problemas de seguridad."

**La Realidad:** AWS proporciona herramientas, pero tú debes implementarlas y monitorearlas.

**Aclaración:**
- AWS proporciona herramientas de seguridad (GuardDuty, Config, etc.)
- Tú debes habilitar y configurar estas herramientas
- Tú debes responder a alertas y hallazgos

### ❌ **"La Responsabilidad Compartida Es Igual para Todos los Servicios"**
**El Mito:** "La división de responsabilidad es consistente en todos los servicios de AWS."

**La Realidad:** La responsabilidad cambia basada en el tipo de servicio (IaaS vs PaaS vs SaaS).

**Ejemplo:**
- **EC2:** Tú gestionas la seguridad del SO
- **Lambda:** AWS gestiona la seguridad del runtime
- **S3:** Responsabilidad compartida para controles de acceso

---

## 📝 Escenarios del Mundo Real

### 🏥 **Escenario 1: Proveedor de Atención Médica**

**Situación:** Hospital desplegando sistema de gestión de pacientes en AWS

**Responsabilidades de AWS:**
- 🏢 **Seguridad física** de centros de datos que almacenan datos de pacientes
- 🔧 **Parches de infraestructura** de sistemas subyacentes
- 🛡️ **Seguridad de hardware** y disposición segura
- 📋 **Certificaciones de cumplimiento** (servicios elegibles para HIPAA)

**Responsabilidades del Cliente:**
- 🔐 **Cifrado de datos** de registros de pacientes
- 👥 **Controles de acceso** para personal médico
- 📋 **Registro de auditoría** de acceso a datos
- 🎓 **Capacitación del personal** en cumplimiento HIPAA
- 🔒 **Seguridad de aplicación** del software de gestión de pacientes

**Responsabilidades Compartidas:**
- 📊 **Gestión de configuración** - AWS configura infraestructura, hospital configura aplicaciones
- 🎓 **Capacitación** - AWS capacita a su personal, hospital capacita al personal médico
- 🔄 **Gestión de parches** - AWS parchea infraestructura, hospital parchea aplicaciones

### 🏦 **Escenario 2: Empresa de Servicios Financieros**

**Situación:** Banco moviendo portal de clientes a AWS

**Requisitos Críticos de Seguridad:**
- Cumplimiento PCI DSS para procesamiento de pagos
- Protección de datos de clientes
- Detección y prevención de fraudes
- Requisitos de auditoría regulatoria

**División de Responsabilidades:**

**AWS Proporciona:**
- 🏢 **Infraestructura compatible con PCI**
- 🔒 **Seguridad física** de sistemas de procesamiento de pagos
- 📋 **Certificaciones de cumplimiento** y reportes de auditoría
- 🛡️ **Seguridad de infraestructura de red**

**El Banco Debe Implementar:**
- 🔐 **Cifrado de extremo a extremo** de datos de pago
- 👥 **Verificación de identidad del cliente**
- 📊 **Monitoreo de transacciones** y detección de fraudes
- 🔍 **Registro de acceso** y pistas de auditoría
- 🎓 **Capacitación de seguridad para empleados**

### 🛒 **Escenario 3: Startup de E-commerce**

**Situación:** Minorista en línea usando múltiples servicios de AWS

**Arquitectura:**
- EC2 para servidores web
- RDS para base de datos de clientes
- S3 para imágenes de productos
- Lambda para procesamiento de órdenes

**Responsabilidades Específicas por Servicio:**

**Servidores Web EC2:**
- **AWS:** Hipervisor, infraestructura física
- **Cliente:** Parches del SO, seguridad del servidor web, certificados SSL

**Base de Datos RDS:**
- **AWS:** Parches del motor de base de datos, infraestructura de respaldos
- **Cliente:** Usuarios de base de datos, configuraciones de cifrado, controles de acceso

**Almacenamiento de Imágenes S3:**
- **AWS:** Infraestructura de almacenamiento, durabilidad
- **Cliente:** Políticas de bucket, cifrado de objetos, controles de acceso

**Funciones Lambda:**
- **AWS:** Entorno de ejecución, escalado de infraestructura
- **Cliente:** Seguridad del código de función, permisos IAM, variables de entorno

---

## ✅ Mejores Prácticas

### 🎯 **Entendiendo Tus Responsabilidades**

#### 📋 **Crear una Matriz de Responsabilidades**
Documenta qué maneja AWS vs. qué manejas tú para cada servicio:

```
Servicio: Amazon RDS
┌────────────────────┬─────────────┬──────────────┐
│ Aspecto Seguridad  │ AWS         │ Cliente      │
├────────────────────┼─────────────┼──────────────┤
│ Seguridad física   │ ✅ Sí       │ ❌ No        │
│ Parches del SO     │ ✅ Sí       │ ❌ No        │
│ Parches de BD      │ ✅ Sí       │ ❌ No        │
│ Gestión usuarios   │ ❌ No       │ ✅ Sí        │
│ Cifrado            │ 🤝 Compartido│ 🤝 Compartido│
│ Gestión respaldos  │ 🤝 Compartido│ 🤝 Compartido│
└────────────────────┴─────────────┴──────────────┘
```

#### 🔍 **Revisiones Regulares de Responsabilidades**
- **Revisiones trimestrales** de responsabilidades de servicios
- **Actualizar documentación** al agregar nuevos servicios
- **Capacitar miembros del equipo** en sus responsabilidades específicas
- **Auditar cumplimiento** con la matriz de responsabilidades

### 🛡️ **Implementando Responsabilidades del Cliente**

#### 🔐 **Protección de Datos**
```
✅ HACER:
- Cifrar datos sensibles en reposo y en tránsito
- Clasificar datos basado en niveles de sensibilidad
- Implementar controles de acceso apropiados
- Pruebas regulares de respaldo y recuperación

❌ NO HACER:
- Asumir que AWS cifra todo por defecto
- Almacenar datos sensibles en texto plano
- Dar permisos de acceso amplios
- Omitir verificación de respaldos
```

#### 👥 **Gestión de Identidad y Acceso**
```
✅ HACER:
- Usar roles IAM en lugar de claves de acceso a largo plazo
- Implementar acceso de menor privilegio
- Habilitar MFA para todos los usuarios
- Revisiones regulares de acceso y limpieza

❌ NO HACER:
- Compartir credenciales entre usuarios
- Usar cuenta root para operaciones diarias
- Otorgar permisos amplios "para estar seguro"
- Omitir auditorías regulares de permisos
```

#### 🔧 **Gestión de Configuración**
```
✅ HACER:
- Usar infraestructura como código (CloudFormation)
- Implementar detección de deriva de configuración
- Revisiones regulares de configuración de seguridad
- Automatizar verificación de cumplimiento

❌ NO HACER:
- Hacer cambios manuales de configuración
- Omitir documentación de configuración
- Ignorar alertas de deriva de configuración
- Asumir que configuraciones por defecto son seguras
```

### 🤝 **Aprovechando Controles Compartidos**

#### 📊 **Estrategia de Gestión de Parches**
```
Parches de AWS:
- Componentes de infraestructura
- Plataformas de servicios gestionados
- Hipervisores y SO host

Parches del Cliente:
- Sistemas operativos invitados
- Aplicaciones y middleware
- Componentes de software personalizado

Coordinación:
- Monitorear anuncios de servicios AWS
- Planificar ventanas de mantenimiento juntos
- Probar parches en no-producción primero
```

#### 🎓 **Capacitación y Conciencia**
```
Capacitación de AWS:
- Capacitación de seguridad para empleados AWS
- Guía de seguridad específica por servicio
- Documentación de mejores prácticas

Capacitación del Cliente:
- Fundamentos de seguridad en la nube
- Responsabilidades específicas por servicio
- Procedimientos de respuesta a incidentes
- Requisitos de cumplimiento
```

---

## 🧠 Ayudas de Memoria

### 🎯 **Formas Fáciles de Recordar**

#### 🏠 **La Regla de la Casa**
- **AWS = Propietario** (edificio, servicios públicos, áreas comunes)
- **Tú = Inquilino** (tus cosas, tus invitados, tu limpieza)

#### 🎂 **El Pastel de Capas**
```
Tus Aplicaciones     ← Tú decoras el pastel
Tus Datos           ← Tú eliges el relleno
Plataforma AWS      ← AWS hornea el pastel
Infraestructura AWS ← AWS proporciona el horno
```

#### 🚗 **La Analogía del Alquiler de Autos**
- **Empresa de Alquiler (AWS):** Mantiene el auto, proporciona seguro, maneja recalls
- **Conductor (Tú):** Conduce seguro, cierra puertas, no deja objetos de valor visibles

### 📝 **Tarjetas de Referencia Rápida**

#### **Servicios IaaS (Como EC2)**
```
AWS: Hardware físico, hipervisor, infraestructura de red
TÚ: Sistema operativo, aplicaciones, datos, gestión de acceso
```

#### **Servicios PaaS (Como RDS)**
```
AWS: Gestión de plataforma, parches, infraestructura
TÚ: Configuración, usuarios, datos, controles de acceso
```

#### **Servicios SaaS (Como WorkMail)**
```
AWS: Aplicación, plataforma, infraestructura
TÚ: Usuarios, datos, seguridad del cliente, políticas de uso
```

---

## 🎯 Preguntas de Práctica

### Pregunta 1
Una empresa está ejecutando una aplicación web en instancias Amazon EC2. Según el modelo de responsabilidad compartida, ¿quién es responsable de parchear el sistema operativo?

A) AWS es responsable de todos los parches
B) El cliente es responsable de parchear el SO
C) AWS y el cliente comparten la responsabilidad de parchear el SO
D) La responsabilidad depende del tipo de instancia

<details>
<summary>💡 Haz clic para ver la Respuesta</summary>

**Respuesta: B) El cliente es responsable de parchear el SO**

**Explicación:** Para instancias EC2 (IaaS), AWS gestiona la infraestructura subyacente e hipervisor, pero los clientes son responsables del sistema operativo invitado, incluyendo parches, actualizaciones y configuraciones de seguridad.

**Punto Clave:** Recuerda que EC2 es Infraestructura como Servicio (IaaS), por lo que el cliente tiene más responsabilidades comparado con Plataforma como Servicio (PaaS) o Software como Servicio (SaaS).
</details>

### Pregunta 2
¿Cuál de los siguientes es un ejemplo de "control compartido" en el modelo de responsabilidad compartida de AWS?

A) Seguridad física de centros de datos
B) Gestión de parches
C) Cifrado de datos del cliente
D) Gestión de identidad y acceso

<details>
<summary>💡 Haz clic para ver la Respuesta</summary>

**Respuesta: B) Gestión de parches**

**Explicación:** La gestión de parches es un control compartido donde AWS es responsable de parchear la infraestructura y servicios gestionados, mientras que los clientes son responsables de parchear sistemas operativos invitados y aplicaciones.

**Punto Clave:** Los controles compartidos requieren que tanto AWS como el cliente implementen sus respectivas partes del control.
</details>

### Pregunta 3
Una empresa está usando Amazon RDS para su base de datos. ¿Cuál responsabilidad de seguridad pertenece al cliente?

A) Parches del motor de base de datos
B) Mantenimiento del sistema operativo
C) Gestión de cuentas de usuario de base de datos
D) Seguridad del hardware físico

<details>
<summary>💡 Haz clic para ver la Respuesta</summary>

**Respuesta: C) Gestión de cuentas de usuario de base de datos**

**Explicación:** Con Amazon RDS (un servicio gestionado), AWS maneja la infraestructura, sistema operativo y mantenimiento del motor de base de datos. Sin embargo, los clientes son responsables de gestionar usuarios de base de datos, permisos y controles de acceso.

**Punto Clave:** Incluso con servicios gestionados, los clientes retienen la responsabilidad de gestión de identidad y acceso dentro de sus aplicaciones.
</details>

---

## ✅ Lista de Verificación del Capítulo

Antes de proceder al siguiente capítulo, asegúrate de poder:

- [ ] Explicar la diferencia entre "seguridad DE la nube" y "seguridad EN la nube"
- [ ] Identificar responsabilidades de AWS vs cliente para diferentes tipos de servicio (IaaS, PaaS, SaaS)
- [ ] Reconocer controles compartidos y entender los roles de ambas partes
- [ ] Aplicar el modelo de responsabilidad compartida a escenarios del mundo real
- [ ] Evitar conceptos erróneos comunes sobre responsabilidades de seguridad en la nube

---

## 🗺️ ¿Qué Sigue?

Ahora que entiendes **quién** es responsable de **qué** en la seguridad de AWS, profundicemos en la herramienta más importante para gestionar **tus** responsabilidades de seguridad.

**🎯 Siguiente Capítulo:** [Fundamentos de IAM](./iam-fundamentals.md)

¡Aprende cómo implementar gestión adecuada de identidad y acceso - la piedra angular de las responsabilidades de seguridad del cliente!

---

**🎉 ¡Excelente base!** Ahora entiendes el marco fundamental que gobierna toda la seguridad de AWS. Este conocimiento guiará cada decisión de seguridad que tomes en la nube.

---

**← [Volver al Resumen del Dominio 2](./README.md)**
