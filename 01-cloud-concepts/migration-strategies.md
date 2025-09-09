# 🚀 Estrategias de Migración de AWS y Marco de Adopción de la Nube

> **Esencial para el Éxito del Cloud Practitioner | Tiempo de Estudio: ~2.5 horas**

¡Bienvenido a uno de los temas más prácticos e importantes para los profesionales de la nube! Las estrategias de migración y el Marco de Adopción de la Nube proporcionan el enfoque estructurado que las organizaciones necesitan para moverse exitosamente a la nube.

## 📋 Tabla de Contenidos
- [🎯 Objetivos de Aprendizaje](#-objetivos-de-aprendizaje)
- [🌍 Las 6 Rs de la Migración](#-las-6-rs-de-la-migración)
- [🏗️ Marco de Adopción de la Nube de AWS (CAF)](#️-marco-de-adopción-de-la-nube-de-aws-caf)
- [⚙️ Herramientas de Migración de AWS](#️-herramientas-de-migración-de-aws)
- [📊 Planificación de Migración](#-planificación-de-migración)
- [🎮 Escenarios del Mundo Real](#-escenarios-del-mundo-real)
- [📝 Preguntas de Práctica](#-preguntas-de-práctica)

---

## 🎯 Objetivos de Aprendizaje

Al final de este capítulo, podrás:

✅ **Entender las 6 Rs de la Migración** - Conocer cada estrategia y cuándo usarla  
✅ **Explicar el Marco de Adopción de la Nube de AWS** - Entender las seis perspectivas  
✅ **Identificar herramientas de migración de AWS** - Saber qué herramientas soportan diferentes tipos de migración  
✅ **Planificar estrategias de migración** - Seleccionar enfoques apropiados para diferentes escenarios  
✅ **Reconocer desafíos de migración** - Entender obstáculos comunes y soluciones  

---

## 🌍 Las 6 Rs de la Migración

### 🏠 **Analogía del Mundo Real: Mudarse de Casa**
Al igual que mudarse de casa, hay diferentes estrategias para mover aplicaciones a la nube:

```
Estrategias de Mudanza:
├── 📦 Llevar todo tal como está (Rehost)
├── 🔧 Arreglar algunas cosas mientras te mudas (Replatform)
├── 🏗️ Renovar completamente (Refactor)
├── 🛍️ Comprar nuevo en su lugar (Repurchase)
├── 🗑️ Tirar lo que no necesitas (Retire)
└── 🏠 Mantener algunas cosas en la casa vieja (Retain)
```

---

### 1️⃣ **Rehost (Lift and Shift)**

#### 🚚 **¿Qué es el Rehosting?**
**Mover aplicaciones a la nube con cambios mínimos o nulos** - como levantar tu aplicación y colocarla en AWS.

#### 🎯 **Características Clave:**
- **Cambios mínimos** - La aplicación funciona tal como está
- **Migración rápida** - La forma más rápida de llegar a la nube
- **Menor esfuerzo inicial** - No se necesitan modificaciones de código
- **Enfoque en infraestructura** - Pasar de físico a virtual

#### 🏆 **Beneficios:**
- ⚡ **Velocidad** - Enfoque de migración más rápido
- 💰 **Ahorros inmediatos de costos** - Reducir costos del centro de datos
- 🛡️ **Reducción de riesgo** - Cambios mínimos = menos problemas
- 📈 **Victorias rápidas** - Comenzar a beneficiarse de la nube inmediatamente

#### 📊 **Ejemplo de Rehost:**
```
Configuración Tradicional:
├── Servidores físicos ejecutando aplicación web
├── Base de datos Oracle en hardware dedicado
├── Dispositivo balanceador de carga
└── Arrays de almacenamiento de red

AWS Rehost:
├── Instancias EC2 (mismo OS, misma aplicación)
├── RDS para Oracle (base de datos gestionada)
├── Application Load Balancer
└── Almacenamiento EBS

Cambios Realizados: Mínimos - solo infraestructura
Beneficios: Economía de nube inmediata
```

#### 🎯 **Mejor Para:**
- **Aplicaciones legacy** con cronogramas ajustados
- **Pruebas de concepto** de migraciones
- **Iniciativas impulsadas por costos** de migración
- **Aplicaciones cerca del fin de vida**

---

### 2️⃣ **Replatform (Lift, Tinker, and Shift)**

#### 🔧 **¿Qué es el Replatforming?**
**Hacer algunas optimizaciones para la nube** sin cambiar la arquitectura central - como actualizar tus electrodomésticos cuando te mudas de casa.

#### 🎯 **Características Clave:**
- **Cambios moderados** - Alguna optimización para la nube
- **Servicios gestionados** - Reemplazar infraestructura con servicios de AWS
- **Mejor rendimiento** - Aprovechar características de la nube
- **Reducida sobrecarga operacional** - Menos gestión requerida

#### 🏆 **Beneficios:**
- 📈 **Rendimiento mejorado** - Optimizaciones de nube
- 💰 **Optimización de costos** - Los servicios gestionados suelen ser más baratos
- 🛡️ **Mantenimiento reducido** - AWS maneja la infraestructura
- 🚀 **Fundación para el futuro** - Establece el escenario para más modernización

#### 📊 **Ejemplo de Replatform:**
```
Antes (On-premises):
├── Servidores de aplicación (auto-gestionados)
├── Base de datos MySQL auto-gestionada
├── Almacenamiento de archivos en unidades de red
└── Configuración personalizada de balanceador de carga

Después (AWS Replatform):
├── Instancias EC2 (mismo código de aplicación)
├── Amazon RDS para MySQL (base de datos gestionada)
├── Amazon EFS para almacenamiento de archivos
└── Application Load Balancer

Cambios Realizados: 
- Base de datos → RDS Gestionado
- Almacenamiento de archivos → EFS
- Balanceador de carga → ALB
Aplicación central: Sin cambios
```

#### 🎯 **Mejor Para:**
- **Aplicaciones que pueden beneficiarse** de servicios gestionados
- **Candidatos de modernización** de base de datos
- **Aplicaciones de complejidad media**
- **Organizaciones que desean alguna optimización**

---

### 3️⃣ **Refactor (Re-architect)**

#### 🏗️ **¿Qué es el Refactoring?**
**Reimaginar cómo la aplicación está arquitecturada y desarrollada** - como rediseñar completamente tu casa para que sea más moderna y eficiente.

#### 🎯 **Características Clave:**
- **Cambios significativos** - Nuevos patrones de arquitectura
- **Diseño nativo de la nube** - Construido para la nube desde cero
- **Tecnologías modernas** - Microservicios, serverless, contenedores
- **Máximos beneficios de la nube** - Utilización completa de capacidades de la nube

#### 🏆 **Beneficios:**
- 🚀 **Máxima agilidad** - Verdaderos beneficios nativos de la nube
- 📈 **Mejor rendimiento** - Optimizado para la nube
- 💰 **Eficiencia de costos a largo plazo** - Pagar solo por lo que usas
- 🔄 **Más fácil de mantener** - Aplicaciones modernas y bien arquitecturadas

#### 📊 **Ejemplo de Refactor:**
```
Antes (Monolítico):
├── Aplicación grande única
├── Componentes fuertemente acoplados
├── Base de datos tradicional
└── Infraestructura fija

Después (Nativo de la nube):
├── Arquitectura de microservicios
│   ├── Servicio de usuario → Lambda + API Gateway
│   ├── Servicio de producto → Contenedores ECS
│   ├── Servicio de pedido → Lambda + SQS
│   └── Servicio de pago → Lambda + DynamoDB
├── Comunicación basada en eventos
├── Auto-escalado basado en demanda
└── Precios de pago por uso

Cambios Realizados: Re-arquitectura completa
Beneficios: Máximas ventajas de la nube
```

#### 🎯 **Mejor Para:**
- **Aplicaciones estratégicas** con valor a largo plazo
- **Aplicaciones de alto tráfico** que necesitan escala
- **Iniciativas enfocadas** en productividad del desarrollador
- **Proyectos greenfield** o actualizaciones importantes

---

### 4️⃣ **Repurchase (Replace)**

#### 🛒 **¿Qué es el Repurchasing?**
**Moverse a un producto diferente** - como vender tu auto viejo y comprar uno nuevo en lugar de mudarlo.

#### 🎯 **Características Clave:**
- **Nueva solución de software** - Usualmente aplicaciones SaaS
- **Reemplazar sistemas legacy** - Alternativas modernas
- **Gestionado por proveedor** - Software como Servicio
- **Conjunto de características diferentes** - Puede requerir cambios de proceso

#### 🏆 **Beneficios:**
- 🚀 **Características modernas** - Última tecnología y capacidades
- 💰 **Costos predecibles** - Precios basados en suscripción
- 🛡️ **Mantenimiento reducido** - El proveedor maneja las actualizaciones
- 📈 **Mejor experiencia de usuario** - Interfaces y flujos de trabajo modernos

#### 📊 **Ejemplos de Repurchase:**
```
Sistema Legacy → Alternativa SaaS
├── CRM personalizado → Salesforce
├── Email on-premises → Microsoft 365
├── Sistema HR legacy → Workday
├── ERP personalizado → SAP SuccessFactors
└── Servidores de archivos → Google Workspace

Beneficios:
- No hay infraestructura que gestionar
- Actualizaciones regulares de características
- Interfaces amigables para móviles
- Capacidades de integración incorporadas
```

#### 🎯 **Mejor Para:**
- **Sistemas legacy** con alternativas SaaS modernas
- **Aplicaciones no centrales** del negocio
- **Organizaciones que desean** reducir sobrecarga de TI
- **Aplicaciones de fin de vida** que necesitan reemplazo

---

### 5️⃣ **Retire**

#### 🗑️ **¿Qué es el Retirement?**
**Cerrar aplicaciones** que ya no son necesarias - como tirar elementos que no necesitas cuando te mudas.

#### 🎯 **Características Clave:**
- **Eliminación de aplicación** - Cierre completo
- **No se necesita migración** - Simplemente apagar
- **Ahorros de costos** - Eliminar licencias y mantenimiento
- **Reducción de riesgo** - Remover vulnerabilidades de seguridad

#### 🏆 **Beneficios:**
- 💰 **Ahorros inmediatos de costos** - No más costos de licencias o hosting
- 🛡️ **Riesgo de seguridad reducido** - Menos sistemas que asegurar
- 🎯 **Portafolio simplificado** - Enfocarse en aplicaciones valiosas
- 📊 **Mejor asignación de recursos** - Enfocar esfuerzos en sistemas importantes
- ⚡ **Migración general más rápida** - Menos aplicaciones que mover

#### 📊 **Candidatos para Retirement:**
```
Aplicaciones a Considerar para Retirar:
├── Funcionalidad duplicada
│   ├── Múltiples herramientas de reportes
│   ├── Sistemas de respaldo redundantes
│   └── Herramientas de monitoreo superpuestas
├── Aplicaciones de bajo uso
│   ├── <5% adopción de usuarios
│   ├── Reportes raramente accedidos
│   └── Herramientas estacionales (usadas una vez/año)
├── Sistemas de fin de vida
│   ├── Sin soporte del proveedor
│   ├── Vulnerabilidades de seguridad
│   └── Problemas de cumplimiento
└── Funcionalidad reemplazada
    ├── Características movidas a otros sistemas
    ├── Cambios en procesos de negocio
    └── Reestructuración organizacional
```

#### 🎯 **Mejor Para:**
- **Aplicaciones no utilizadas o subutilizadas**
- **Funcionalidad duplicada** entre sistemas
- **Aplicaciones de fin de vida** sin soporte
- **Aplicaciones con vulnerabilidades** de seguridad
- **Aplicaciones Shadow IT**

---

### 6️⃣ **Retain (Revisit)**

#### 🏠 **¿Qué es la Retención?**
**Mantener aplicaciones on-premises** por ahora - como mantener algunas pertenencias en tu casa vieja porque no estás listo para moverlas aún.

#### 🎯 **Características Clave:**
- **Permanecer on-premises** - Sin migración inmediata
- **Decisión temporal** - Revisar más tarde
- **Razones válidas de negocio** - Cumplimiento, latencia, etc.
- **Migración futura planificada** - Parte de estrategia a largo plazo

#### 🏆 **Beneficios:**
- ⏰ **Sin decisiones apresuradas** - Tomar tiempo para planificar apropiadamente
- 🛡️ **Mantener cumplimiento** - Mantener datos sensibles on-premises
- 💰 **Evitar costos de migración** - Para aplicaciones que funcionan bien
- 🎯 **Enfocar recursos** - Priorizar otras migraciones

#### 📊 **Ejemplos de Retención:**
```
Escenarios Comunes de Retención:
├── Regulatorio/Cumplimiento
│   ├── Sistemas de trading financiero
│   ├── Sistemas clasificados del gobierno
│   ├── Sistemas PHI de salud
│   └── Requisitos específicos de la industria
├── Restricciones Técnicas
│   ├── Aplicaciones mainframe
│   ├── Dependencias de hardware legacy
│   ├── Integraciones de hardware personalizadas
│   └── Sistemas críticos de rendimiento
├── Restricciones de Negocio
│   ├── Misión crítica sin ventana de inactividad
│   ├── Integraciones complejas con sistemas legacy
│   ├── Inversiones importantes recientes
│   └── Proyectos importantes en curso
└── Consideraciones de Tiempo
    ├── Próximos reemplazos de aplicaciones
    ├── Actualizaciones de tecnología planificadas
    ├── Restricciones de presupuesto
    └── Disponibilidad de recursos
```

#### 🎯 **Mejor Para:**
- **Aplicaciones mainframe** que requieren experiencia especializada
- **Sistemas de misión crítica** durante períodos críticos de negocio
- **Hardware/software con inversión reciente**
- **Sistemas legacy complejos** que requieren planificación extensa

---

## 🏗️ Marco de Adopción de la Nube de AWS (CAF)

### 🎯 **¿Qué es AWS CAF?**
El **Marco de Adopción de la Nube de AWS** proporciona orientación para ayudar a las organizaciones a diseñar y recorrer un camino acelerado hacia la adopción exitosa de la nube.

### 🏠 **Analogía del Mundo Real: Construir una Casa**
CAF es como tener **seis expertos diferentes** ayudándote a construir la casa de tus sueños:

```
Equipo de Construcción de Casa:
├── 👔 Experto en Negocios (Perspectiva de Negocio)
├── 👥 Coordinador de Familia (Perspectiva de Personas)  
├── 🎯 Gerente de Proyecto (Perspectiva de Gobernanza)
├── 🏗️ Ingeniero de Plataforma (Perspectiva de Plataforma)
├── 🔒 Experto en Seguridad (Perspectiva de Seguridad)
└── 🔧 Gerente de Operaciones (Perspectiva de Operaciones)
```

---

### 📊 **Las Seis Perspectivas de CAF**

#### 1️⃣ **Perspectiva de Negocio**
**Asegura que las inversiones en la nube aceleren los resultados del negocio**

**Partes Interesadas Clave:**
- Gerentes de negocio
- Gerentes de finanzas
- Propietarios de presupuesto
- Partes interesadas de estrategia

**Áreas de Enfoque:**
- 💰 **Desarrollo de caso de negocio** - Justificación de ROI
- 📈 **Realización de beneficios** - Midiendo el valor de la nube
- 🎯 **Alineación estratégica** - La nube apoya los objetivos del negocio
- 📊 **Gestión financiera** - Economía de la nube

**Actividades de Ejemplo:**
```
Entregables de Perspectiva de Negocio:
├── Caso de negocio de nube con proyecciones de ROI
├── Métricas de éxito y KPIs
├── Matriz de prioridad de migración
├── Análisis de costo-beneficio
└── Evaluación de riesgo y planes de mitigación
```

---

#### 2️⃣ **Perspectiva de Personas**
**Apoya el desarrollo de estrategia de gestión de cambio a nivel organizacional**

**Partes Interesadas Clave:**
- Gerentes de RRHH
- Gerentes de capacitación
- Gerentes de personas
- Desarrollo organizacional

**Áreas de Enfoque:**
- 🎓 **Evaluación de habilidades** - Capacidades actuales vs necesarias
- 📚 **Programas de capacitación** - Desarrollando habilidades de nube
- 🔄 **Gestión de cambio** - Transformación cultural
- 👥 **Organización de equipos** - Nuevos roles y responsabilidades

**Actividades de Ejemplo:**
```
Entregables de Perspectiva de Personas:
├── Análisis de brecha de habilidades
├── Hoja de ruta de capacitación y certificación
├── Plan de gestión de cambio
├── Nueva estructura organizacional
└── Actualizaciones de gestión de rendimiento
```

---

#### 3️⃣ **Perspectiva de Gobernanza**
**Asegura la gobernanza del negocio en la nube**

**Partes Interesadas Clave:**
- CIO
- Gerentes de programa
- Arquitectos empresariales
- Analistas de negocio

**Áreas de Enfoque:**
- 📋 **Gestión de portafolio** - Priorizando iniciativas de nube
- 🎯 **Gestión de programa** - Coordinando proyectos de nube
- 📊 **Medición de rendimiento** - Seguimiento del progreso
- 🔄 **Optimización de procesos** - Mejorando operaciones de nube

**Actividades de Ejemplo:**
```
Entregables de Perspectiva de Gobernanza:
├── Marco de gobernanza de nube
├── Procesos de gestión de portafolio
├── Sistema de medición de rendimiento
├── Estándares de gestión de proyectos
└── Procedimientos de monitoreo de cumplimiento
```

---

#### 4️⃣ **Perspectiva de Plataforma**
**Principios para diseñar, implementar y optimizar la arquitectura de AWS**

**Partes Interesadas Clave:**
- Arquitectos de soluciones
- Ingenieros de software
- Arquitectos de nube
- Ingenieros de plataforma

**Áreas de Enfoque:**
- 🏗️ **Diseño de arquitectura** - Sistemas escalables y resilientes
- 🔧 **Implementación de plataforma** - Selección de servicios de AWS
- 📈 **Planificación de escalabilidad** - Acomodación del crecimiento
- 🛡️ **Recuperación ante desastres** - Continuidad del negocio

**Actividades de Ejemplo:**
```
Entregables de Perspectiva de Plataforma:
├── Diseños de arquitectura de referencia
├── Guías de selección de servicios de AWS
├── Plantillas de Infraestructura como Código
├── Procedimientos de recuperación ante desastres
└── Guías de optimización de rendimiento
```

---

#### 5️⃣ **Perspectiva de Seguridad**
**Asegura que la organización cumpla los objetivos de seguridad**

**Partes Interesadas Clave:**
- CISO
- Arquitectos de seguridad
- Oficiales de cumplimiento
- Gerentes de riesgo

**Áreas de Enfoque:**
- 🔒 **Gestión de identidad y acceso** - Quién puede acceder a qué
- 🛡️ **Protección de datos** - Cifrado y privacidad
- 🔍 **Detección de amenazas** - Monitoreo y respuesta
- 📋 **Gestión de cumplimiento** - Cumplir requisitos regulatorios
- 🛡️ **Gestión de riesgo** - Evaluación de amenazas
- 🔍 **Respuesta ante incidentes** - Monitoreo de seguridad

**Actividades de Ejemplo:**
```
Entregables de Perspectiva de Seguridad:
├── Arquitectura de seguridad de referencia
├── Evaluación de cumplimiento y mapeo
├── Diseño de gestión de identidad y acceso
├── Estrategia de protección de datos
└── Procedimientos de respuesta ante incidentes
```

---

#### 6️⃣ **Perspectiva de Operaciones**
**Define el modelo operativo para la adopción de la nube**

**Partes Interesadas Clave:**
- Gerentes de operaciones de TI
- Ingenieros de operaciones de nube
- Ingenieros de confiabilidad del sitio
- Gerentes de servicio

**Áreas de Enfoque:**
- 📊 **Monitoreo y alertas** - Observabilidad del sistema
- 🔄 **Automatización** - Eficiencia operacional
- 🎯 **Gestión de servicios** - Entrega de servicios de TI
- 📈 **Optimización de rendimiento** - Mejora continua

**Actividades de Ejemplo:**
```
Entregables de Perspectiva de Operaciones:
├── Diseño de modelo operativo de nube
├── Estrategia de monitoreo y alertas
├── Marco de automatización
├── Acuerdos de nivel de servicio
└── Procedimientos operacionales y runbooks
```

---

## ⚙️ Herramientas de Migración de AWS

### 🛠️ **Descubrimiento y Evaluación**

#### **AWS Application Discovery Service**
**Descubre aplicaciones on-premises y dependencias**

**Lo que hace:**
- 📊 **Descubrimiento basado en agente** - Información detallada del servidor
- 🔍 **Descubrimiento sin agente** - Descubrimiento basado en red
- 📈 **Mapeo de dependencias** - Relaciones de aplicaciones
- 📋 **Planificación de migración** - Reportes de evaluación

#### **AWS Migration Hub**
**Ubicación central para rastrear el progreso de migración**

**Características:**
- 🎯 **Panel único** - Todas las migraciones en un lugar
- 📊 **Seguimiento de progreso** - Estado de migración en tiempo real
- 🔗 **Integración de herramientas** - Funciona con múltiples herramientas de migración
- 📋 **Reportes** - Análisis e insights de migración

---

### 🚚 **Migración de Servidores**

#### **AWS Application Migration Service (MGN)**
**Migración lift-and-shift para servidores físicos, virtuales y de nube**

**Características Clave:**
- 🔄 **Replicación continua** - Tiempo de inactividad mínimo
- 🛡️ **Replicación a nivel de bloque** - Copias exactas del servidor
- 🎯 **Conversión automatizada** - Convertir a instancias de AWS
- 📊 **Capacidades de prueba** - Validar antes del cambio

#### **AWS Server Migration Service (SMS)**
**Migración automatizada de servidores on-premises** (Siendo reemplazado por MGN)

**Casos de Uso:**
- 📦 **Cargas de trabajo basadas en VM** - VMware, Hyper-V
- 🔄 **Replicación incremental** - Impacto mínimo en la red
- 🎯 **Creación automatizada de AMI** - Instancias listas para ejecutar

---

### 🗄️ **Migración de Base de Datos**

#### **AWS Database Migration Service (DMS)**
**Migrar bases de datos con tiempo de inactividad mínimo**

**Tipos de Migración:**
- 🔄 **Homogénea** - Mismo motor de base de datos
- 🔀 **Heterogénea** - Diferentes motores de base de datos
- 📊 **Replicación continua** - Sincronización de datos en curso

#### **AWS Schema Conversion Tool (SCT)**
**Convertir esquemas de base de datos entre motores**

**Capacidades:**
- 🔧 **Conversión de esquema** - Conversión de tabla, vista, procedimiento
- 📊 **Reportes de evaluación** - Análisis de complejidad de migración
- 💡 **Recomendaciones** - Mejores prácticas para plataforma objetivo

---

### 📁 **Transferencia de Datos**

#### **AWS DataSync**
**Transferir datos entre on-premises y AWS**

**Características:**
- 🚀 **Transferencia rápida** - Hasta 10x más rápido que herramientas tradicionales
- 🔒 **Transferencia segura** - Cifrado en tránsito
- 📊 **Verificación** - Verificación de integridad de datos
- ⏰ **Programación** - Transferencia automatizada de datos

#### **AWS Snow Family**
**Dispositivos físicos de transferencia de datos**

**Opciones:**
- ❄️ **Snowcone** - 8TB, computación en el borde
- 📦 **Snowball** - 50-80TB, migración de datos
- 🚛 **Snowmobile** - 100PB, conjuntos de datos masivos

---

## 📊 Planificación de Migración

### 📝 **Proceso de Evaluación de Migración**

#### **Fase 1: Descubrimiento**
```
Actividades de Descubrimiento:
├── Inventario de aplicaciones
│   ├── Catalogar todas las aplicaciones
│   ├── Documentar dependencias
│   ├── Evaluar complejidad técnica
│   └── Identificar criticidad del negocio
├── Evaluación de infraestructura
│   ├── Especificaciones del servidor
│   ├── Requisitos de red
│   ├── Necesidades de almacenamiento
│   └── Líneas base de rendimiento
├── Mapeo de dependencias
│   ├── Relaciones de aplicaciones
│   ├── Flujos de datos
│   ├── Puntos de integración
│   └── Dependencias de terceros
└── Entrevistas con partes interesadas
    ├── Requisitos del negocio
    ├── Restricciones técnicas
    ├── Necesidades de cumplimiento
    └── Expectativas de cronograma
```

#### **Fase 2: Planificación**
```
Entregables de Planificación:
├── Estrategia de migración por aplicación
│   ├── Asignación de 6 Rs
│   ├── Enfoque técnico
│   ├── Evaluación de riesgo
│   └── Estimación de cronograma
├── Hoja de ruta de migración
│   ├── Planificación de oleadas
│   ├── Secuenciación de dependencias
│   ├── Asignación de recursos
│   └── Definición de hitos
├── Arquitectura objetivo
│   ├── Selección de servicios de AWS
│   ├── Diseño de seguridad
│   ├── Arquitectura de red
│   └── Estrategia de monitoreo
└── Criterios de éxito
    ├── Métricas de rendimiento
    ├── Objetivos de costo
    ├── Metas de cronograma
    └── Mitigación de riesgo
```

---

### 🎯 **Estrategia de Oleadas de Migración**

#### **Enfoque Basado en Oleadas**
**Agrupar aplicaciones en lotes lógicos de migración**

```
Oleadas de Migración:
├── Oleada 1: Bajo Riesgo, Alto Aprendizaje
│   ├── Entornos de desarrollo/prueba
│   ├── Aplicaciones no críticas
│   ├── Arquitecturas simples
│   └── Dependencias limitadas
├── Oleada 2: Complejidad Media
│   ├── Apps importantes pero no críticas
│   ├── Dependencias moderadas
│   ├── Arquitecturas estándar
│   └── Alguna personalización necesaria
├── Oleada 3: Críticas del Negocio
│   ├── Aplicaciones de misión crítica
│   ├── Arquitecturas complejas
│   ├── Dependencias extensas
│   └── Requisitos de alta disponibilidad
└── Oleada 4: Más Complejas
    ├── Sistemas mainframe legacy
    ├── Aplicaciones altamente integradas
    ├── Dependencias de hardware personalizado
    └── Restricciones regulatorias
```

#### **Beneficios del Enfoque de Oleadas:**
- 📚 **Progresión de aprendizaje** - Construir experiencia a lo largo del tiempo
- 🛡️ **Mitigación de riesgo** - Limitar exposición por oleada
- 📈 **Construcción de impulso** - Victorias tempranas impulsan adopción
- 🔄 **Refinamiento de procesos** - Mejorar con cada oleada

---

## 🎮 Escenarios del Mundo Real

### 🏦 **Escenario 1: Migración de Empresa Minorista**

**Perfil de la Empresa:**
- **Cadena minorista grande** con 500 tiendas
- **Sistemas legacy** ejecutándose on-premises
- **Patrones de tráfico estacional**
- **Requisitos de cumplimiento** para procesamiento de pagos

**Estado Actual:**
```
Infraestructura On-Premises:
├── Plataforma de e-commerce (stack LAMP)
├── Sistema de gestión de inventario (Oracle)
├── Sistemas de punto de venta (Windows Server)
├── Base de datos de clientes (SQL Server)
└── Sistemas de reportes (Oracle Business Intelligence)
```

**Estrategia de Migración por Aplicación:**

#### **Plataforma de E-commerce: Replatform**
```
Enfoque de Migración:
├── Servidores web → EC2 con Auto Scaling
├── Base de datos → RDS para MySQL
├── Almacenamiento de archivos → S3 + CloudFront CDN
└── Balanceador de carga → Application Load Balancer

Beneficios:
- Manejar picos de tráfico estacional
- Rendimiento global mejorado
- Sobrecarga operacional reducida
- Optimización de costos a través de auto-escalado
```

#### **Sistema de Inventario: Rehost**
```
Enfoque de Migración:
├── Base de datos Oracle → RDS para Oracle
├── Servidores de aplicación → Instancias EC2
├── Mismo código de aplicación
└── Cambios mínimos de configuración

Beneficios:
- Migración rápida con bajo riesgo
- Ahorros inmediatos de costos de infraestructura
- Fundación para optimización futura
- Mantiene integraciones existentes
```

#### **Sistemas de Reportes: Repurchase**
```
Enfoque de Migración:
├── Oracle BI → Amazon QuickSight
├── Data warehouse → Amazon Redshift
├── Procesos ETL → AWS Glue
└── Nuevos dashboards y análisis

Beneficios:
- Capacidades de análisis modernas
- Inteligencia de negocio de autoservicio
- Costos de licencias reducidos
- Mejor acceso móvil
```

**Resultados:**
- **40% reducción de costos** en el primer año
- **99.99% disponibilidad** durante temporada alta
- **3x más rápida** generación de reportes
- **6 meses** cronograma total de migración

---

### 🏥 **Escenario 2: Organización de Salud**

**Perfil de la Empresa:**
- **Sistema hospitalario regional** con 5 ubicaciones
- **Requisitos de cumplimiento HIPAA**
- **Sistemas clínicos legacy**
- **Operaciones 24/7** con cero tolerancia al tiempo de inactividad

**Estrategia de Migración:**

#### **Sistema de Registros de Pacientes: Retain**
```
Razón para Retención:
├── Sistema basado en mainframe
├── Integraciones complejas con dispositivos médicos
├── Personalización extensa durante 20 años
├── Aprobación regulatoria requerida para cambios
└── Certificación de cumplimiento reciente

Cronograma: Revisar en 2 años después de planificación de modernización
```

#### **Email y Colaboración: Repurchase**
```
Enfoque de Migración:
├── Exchange Server → Microsoft 365
├── Servidores de archivos → SharePoint Online
├── Videoconferencias → Microsoft Teams
└── Gestión de dispositivos móviles → Intune

Beneficios:
- Herramientas de colaboración modernas
- Características de cumplimiento incorporadas
- Mantenimiento de TI reducido
- Mejor soporte móvil para doctores
```

#### **Portal Web: Refactor**
```
Enfoque de Migración:
├── Aplicación monolítica → Microservicios
├── Portal de pacientes → Serverless (Lambda + API Gateway)
├── Sistema de citas → Contenedores ECS
└── Base de datos → Aurora con cifrado

Beneficios:
- Mejor experiencia del paciente
- Escalabilidad mejorada
- Características de seguridad mejoradas
- Desarrollo de características más rápido
```

**Consideraciones de Cumplimiento:**
- **Cifrado de extremo a extremo** para toda la PHI
- **Aislamiento VPC** para sistemas clínicos
- **Registro CloudTrail** para requisitos de auditoría
- **Acuerdos BAA** con AWS para cumplimiento HIPAA

---

### 🏗️ **Escenario 3: Empresa Manufacturera**

**Perfil de la Empresa:**
- **Manufactura global** con plantas en 12 países
- **Datos de IoT y sensores** de líneas de producción
- **Requisitos de integración** del sistema ERP
- **Iniciativas de mantenimiento predictivo**

**Estrategia de Migración:**

#### **Sistema ERP: Replatform**
```
Enfoque de Migración:
├── Servidores SAP → Hosts dedicados EC2
├── Base de datos SAP → RDS para SQL Server
├── Almacenamiento de archivos → EFS para datos compartidos
└── Respaldo → S3 con políticas de ciclo de vida

Beneficios:
- Recuperación ante desastres mejorada
- Mejor rendimiento global
- Mantenimiento de hardware reducido
- Almacenamiento optimizado en costos
```

#### **Plataforma de Datos IoT: Refactor**
```
Nueva Arquitectura Nativa de la Nube:
├── Sensores IoT → AWS IoT Core
├── Ingestión de datos → Kinesis Data Streams
├── Procesamiento en tiempo real → Funciones Lambda
├── Almacenamiento de datos → DynamoDB + S3 Data Lake
├── Análisis → Amazon EMR + QuickSight
└── Aprendizaje automático → SageMaker

Beneficios:
- Insights en tiempo real de datos de producción
- Capacidades de mantenimiento predictivo
- Procesamiento de datos escalable
- Análisis avanzado y ML
```

#### **Reportes Legacy: Retire**
```
Aplicaciones Retiradas:
├── Múltiples herramientas de reportes redundantes
├── Sistemas de hojas de cálculo Shadow IT
├── Aplicaciones de dashboard obsoletas
└── Sistemas de monitoreo no utilizados

Beneficios:
- Complejidad reducida
- Costos de licencias menores
- Arquitectura de datos simplificada
- Enfoque en análisis estratégico
```

**Resultados:**
- **15% reducción** en tiempo de inactividad del equipo
- **25% ahorros de costos** en infraestructura de TI
- **Visibilidad en tiempo real** en todas las plantas
- **Toma de decisiones mejorada** con mejor análisis

---

## 📝 Preguntas de Práctica

### Pregunta 1
Una empresa quiere mover su aplicación web existente a AWS rápidamente con cambios mínimos. Necesitan reducir costos del centro de datos pero no tienen tiempo para modificaciones de aplicación. ¿Qué estrategia de migración es más apropiada?

**A)** Refactor  
**B)** Rehost  
**C)** Repurchase  
**D)** Retire  

<details>
<summary>🔍 Clic para Respuesta</summary>

**Respuesta: B) Rehost**

**Explicación:** Rehost (lift and shift) es la estrategia de migración más rápida con cambios mínimos. Permite a la empresa moverse rápidamente a AWS y comenzar a obtener beneficios de costos sin gastar tiempo en modificaciones de aplicación.

</details>

---

### Pregunta 2
Una empresa de servicios financieros está evaluando sus aplicaciones mainframe legacy. Las aplicaciones manejan transacciones bancarias centrales y están sujetas a requisitos regulatorios estrictos. ¿Qué estrategia de migración deberían considerar primero?

**A)** Rehost a EC2 inmediatamente  
**B)** Refactor a microservicios  
**C)** Retain para evaluación adicional  
**D)** Repurchase con soluciones SaaS  

<details>
<summary>🔍 Clic para Respuesta</summary>

**Respuesta: C) Retain para evaluación adicional**

**Explicación:** Las aplicaciones mainframe legacy con requisitos regulatorios estrictos y criticidad central del negocio deben típicamente ser retenidas inicialmente mientras se conduce planificación y evaluación apropiada para futuras estrategias de migración.

</details>

---

### Pregunta 3
¿Qué perspectiva del Marco de Adopción de la Nube de AWS se enfoca en desarrollar estrategias de gestión de cambio organizacional para la adopción de la nube?

**A)** Perspectiva de Negocio  
**B)** Perspectiva de Personas  
**C)** Perspectiva de Gobernanza  
**D)** Perspectiva de Operaciones  

<details>
<summary>🔍 Clic para Respuesta</summary>

**Respuesta: B) Perspectiva de Personas**

**Explicación:** La Perspectiva de Personas de AWS CAF se enfoca en desarrollar estrategias de gestión de cambio a nivel organizacional, incluyendo evaluación de habilidades, programas de capacitación y transformación cultural necesaria para la adopción exitosa de la nube.

</details>

---

### Pregunta 4
Una empresa ha identificado que su sistema actual de gestión de relaciones con clientes (CRM) está desactualizado y es difícil de mantener. Las alternativas SaaS modernas como Salesforce proporcionarían mejor funcionalidad. ¿Qué estrategia de migración es más apropiada?

**A)** Rehost  
**B)** Replatform  
**C)** Refactor  
**D)** Repurchase  

<details>
<summary>🔍 Clic para Respuesta</summary>

**Respuesta: D) Repurchase**

**Explicación:** Repurchase es la estrategia apropiada cuando se mueve a un producto diferente, típicamente una solución SaaS como Salesforce que proporciona mejor funcionalidad que mantener sistemas personalizados legacy.

</details>

---

### Pregunta 5
¿Qué servicio de AWS proporciona una ubicación central para rastrear el progreso de múltiples proyectos de migración?

**A)** AWS Application Discovery Service  
**B)** AWS Migration Hub  
**C)** AWS Database Migration Service  
**D)** AWS Server Migration Service  

<details>
<summary>🔍 Clic para Respuesta</summary>

**Respuesta: B) AWS Migration Hub**

**Explicación:** AWS Migration Hub proporciona una ubicación central para rastrear el progreso de migración a través de múltiples herramientas de migración de AWS y socios, dando una vista única de migraciones a través del portafolio.

</details>

---

## 🎯 Conclusiones Clave

### 🌟 **El Panorama General**
- **La migración es un viaje** - Diferentes estrategias para diferentes aplicaciones
- **La evaluación es crítica** - Entender el estado actual impulsa la selección de estrategia
- **No hay una solución única** - Cada aplicación necesita evaluación individual
- **El cambio cultural importa** - Las personas y procesos son tan importantes como la tecnología

### 💡 **Para el Examen**
- **Conocer las 6 Rs** - Rehost, Replatform, Refactor, Repurchase, Retire, Retain
- **Entender perspectivas CAF** - Negocio, Personas, Gobernanza, Plataforma, Seguridad, Operaciones
- **Reconocer herramientas de migración** - DMS para bases de datos, MGN para servidores, Migration Hub para seguimiento
- **Emparejar estrategias con escenarios** - Victorias rápidas vs optimización a largo plazo

### 🚀 **Para Aplicación del Mundo Real**
- **Comenzar con descubrimiento** - No puedes migrar lo que no entiendes
- **Planificar en oleadas** - Construir experiencia y reducir riesgo
- **Enfocarse en victorias rápidas** - Éxitos tempranos construyen impulso
- **Pensar más allá de la tecnología** - Abordar personas, procesos y gobernanza

### 🏆 **Factores de Éxito**
- **Patrocinio ejecutivo** - El compromiso del liderazgo es esencial
- **Desarrollo de habilidades** - Invertir en capacitación y certificación
- **Gestión de cambio** - Abordar la transformación cultural
- **Enfoque iterativo** - Aprender y mejorar con cada oleada

---

## 🧠 Ayudas de Memoria

### 🎯 **Marco de las 6 Rs: "Realmente Robusto Replatforming Requiere Retirar Redundancia"**
- **R**ehost - Lift and shift (más rápido)
- **R**eplatform - Lift, tinker, and shift (optimizado)
- **R**efactor - Re-arquitecturar (modernizado)
- **R**epurchase - Reemplazar con SaaS
- **R**etire - Eliminar innecesario
- **R**etain - Mantener por ahora

### 🏗️ **Perspectivas CAF: "Negocio Personas Gobiernan Plataforma Seguridad Operaciones"**
- **N**egocio - ROI y alineación de estrategia
- **P**ersonas - Habilidades y gestión de cambio
- **G**obernanza - Gestión de portafolio y programa
- **P**lataforma - Arquitectura e implementación
- **S**eguridad - Riesgo y cumplimiento
- **O**peraciones - Entrega de servicios y monitoreo

---

*¡Ahora tienes una comprensión integral de las estrategias de migración de AWS y el Marco de Adopción de la Nube! Estos conceptos son esenciales para planificar y ejecutar migraciones exitosas a la nube en el mundo real. 🚀*
