# 🖥️ Servicios de Cómputo

> **"La base de la computación en la nube - donde tus aplicaciones cobran vida"**

## 🎯 Resumen del Capítulo

**Tiempo de Estudio:** ~6 horas  
**Dificultad:** Principiante a Intermedio  
**Importancia:** ⭐⭐⭐⭐⭐ (¡Base fundamental!)

Los servicios de cómputo son los **motores de la nube** - proporcionan el poder de procesamiento que ejecuta tus aplicaciones. Entender los servicios de cómputo es fundamental porque toda aplicación en la nube necesita un lugar donde ejecutarse.

---

## 📋 Tabla de Contenidos

- [🏗️ Entendiendo el Cómputo en la Nube](#️-entendiendo-el-cómputo-en-la-nube)
- [🖥️ Amazon EC2 (Elastic Compute Cloud)](#️-amazon-ec2-elastic-compute-cloud)
- [⚡ AWS Lambda (Computación Sin Servidor)](#-aws-lambda-computación-sin-servidor)
- [📦 Servicios de Contenedores](#-servicios-de-contenedores)
- [🌟 Servicios de Cómputo Especializados](#-servicios-de-cómputo-especializados)
- [🎯 Eligiendo el Servicio de Cómputo Correcto](#-eligiendo-el-servicio-de-cómputo-correcto)
- [📝 Escenarios del Mundo Real](#-escenarios-del-mundo-real)

---

## 🏗️ Entendiendo el Cómputo en la Nube

### 🤔 **¿Qué es el Cómputo en la Nube?**
El cómputo en la nube proporciona **poder de procesamiento bajo demanda** para ejecutar aplicaciones, sin necesidad de comprar, instalar o mantener servidores físicos.

### 🏠 **Analogía del Mundo Real: Opciones de Vivienda**
Piensa en los servicios de cómputo como **diferentes opciones de vivienda**:

```
🏠 EC2 = Alquilar un Apartamento
├── Obtienes todo el espacio
├── Lo amueblas y mantienes
├── Eliges el tamaño y ubicación
└── Pagas renta mensual

⚡ Lambda = Servicio a la Habitación del Hotel
├── Solo usas lo que necesitas
├── Todo está proporcionado
├── Pagas por uso
└── No se requiere mantenimiento

📦 Contenedores = Apartamento Amueblado
├── Ambiente preconfigurado
├── Portátil entre ubicaciones
├── Configuración consistente en todas partes
└── Recursos compartidos del edificio
```

### 📊 **Categorías de Servicios de Cómputo**

| **Tipo de Servicio** | **Nivel de Gestión** | **Caso de Uso** | **Facturación** |
|------------------|-------------------|--------------|-------------|
| **Máquinas Virtuales (EC2)** | Alto control | Aplicaciones generales | Por hora |
| **Sin Servidor (Lambda)** | Sin gestión de infraestructura | Funciones basadas en eventos | Por ejecución |
| **Contenedores** | Control medio | Microservicios | Por recurso usado |
| **Especializados** | Varía | Cargas de trabajo específicas | Específico del servicio |

---

## 🖥️ Amazon EC2 (Elastic Compute Cloud)

### 🤔 **¿Qué es Amazon EC2?**
Amazon EC2 proporciona **servidores virtuales redimensionables en la nube**. Piénsalo como alquilar computadoras en los centros de datos de Amazon que puedes configurar y controlar remotamente.

### 🏠 **Analogía del Mundo Real: Alquiler de Apartamento**
EC2 es como **alquilar un apartamento**:
- 🏠 **Elegir tamaño de apartamento** (tipo de instancia)
- 📍 **Seleccionar ubicación** (zona de disponibilidad)
- 🏢 **Seleccionar edificio** (familia de instancia)
- 🔑 **Obtener tus llaves** (pares de llaves)
- 🪑 **Amueblarlo tú mismo** (instalar software)
- 💰 **Pagar renta mensual** (facturación por hora)

### 🏗️ **Conceptos Centrales de EC2**

#### **Tipos de Instancia**
EC2 ofrece diferentes **"tamaños" de máquinas virtuales** optimizadas para diferentes casos de uso:

**Propósito General (T3, M5, M6i):**
- 🎯 **Equilibrado** en cómputo, memoria y redes
- 💼 **Casos de uso:** Servidores web, bases de datos pequeñas, entornos de desarrollo
- 💰 **Costo:** Moderado
- 📊 **Ejemplo:** t3.medium (2 vCPUs, 4 GB RAM)

**Optimizado para Cómputo (C5, C6i):**
- 🚀 **Procesadores de alto rendimiento**
- 💼 **Casos de uso:** Aplicaciones intensivas en CPU, servidores de juegos, computación científica
- 💰 **Costo:** Enfoque en CPU más alto
- 📊 **Ejemplo:** c5.large (2 vCPUs, 4 GB RAM, CPU optimizada)

**Optimizado para Memoria (R5, R6i, X1):**
- 🧠 **Grandes cantidades de RAM**
- 💼 **Casos de uso:** Bases de datos en memoria, analítica en tiempo real, caché
- 💰 **Costo:** Enfoque en memoria más alto
- 📊 **Ejemplo:** r5.large (2 vCPUs, 16 GB RAM)

**Optimizado para Almacenamiento (I3, D2, D3):**
- 💾 **Almacenamiento local de alta velocidad**
- 💼 **Casos de uso:** Bases de datos NoSQL, data warehousing, sistemas de archivos
- 💰 **Costo:** Enfoque en almacenamiento más alto
- 📊 **Ejemplo:** i3.large (2 vCPUs, 15.25 GB RAM, NVMe SSD)

#### **Convención de Nomenclatura de Familias de Instancia**
```
Ejemplo: m5.large
├── m = Familia de instancia (propósito general)
├── 5 = Generación (5ta generación)
└── large = Tamaño (small, medium, large, xlarge, etc.)
```

### 💰 **Modelos de Precios de EC2**

#### **Instancias Bajo Demanda**
- 💳 **Paga por hora/segundo** sin compromisos a largo plazo
- 🎯 **Mejor para:** Cargas de trabajo impredecibles, desarrollo, pruebas
- 📊 **Precios:** Costo por hora más alto
- ✅ **Pros:** Máxima flexibilidad, sin compromisos
- ❌ **Contras:** Opción más costosa

**Caso de Uso de Ejemplo:**
```
Entorno de Desarrollo:
- Los desarrolladores trabajan 8 horas/día, 5 días/semana
- Instancias ejecutándose solo cuando se necesitan
- El uso varía según las fases del proyecto
- Bajo demanda perfecto para uso flexible
```

#### **Instancias Reservadas (RIs)**
- 🏷️ **Compromiso de 1 o 3 años** para descuentos significativos
- 🎯 **Mejor para:** Cargas de trabajo estables y predecibles
- 📊 **Ahorros:** Hasta 75% comparado con bajo demanda
- ✅ **Pros:** Grandes ahorros de costo para uso consistente
- ❌ **Contras:** Compromiso requerido, menos flexibilidad

**Opciones de Pago de RI:**
- **Todo por Adelantado:** Paga todo por adelantado, máximo descuento
- **Parcial por Adelantado:** Paga algo por adelantado, pagos mensuales
- **Sin Adelanto:** Sin pago por adelantado, solo pagos mensuales

**Caso de Uso de Ejemplo:**
```
Servidor Web de Producción:
- Funciona 24/7/365
- Patrones de tráfico consistentes
- Plan de negocio de 3 años
- Instancia Reservada ahorra 60% vs bajo demanda
```

#### **Instancias Spot**
- 💰 **Pujar por capacidad no utilizada** con hasta 90% de descuento
- 🎯 **Mejor para:** Cargas de trabajo tolerantes a fallos, flexibles
- 📊 **Ahorros:** Hasta 90% comparado con bajo demanda
- ✅ **Pros:** Ahorros masivos de costo
- ❌ **Contras:** Pueden ser terminadas con aviso de 2 minutos

**Caso de Uso de Ejemplo:**
```
Trabajo de Procesamiento de Datos:
- Procesar grandes datasets durante la noche
- El trabajo puede reiniciarse si se interrumpe
- No es crítico en tiempo
- Las instancias Spot proporcionan 80% de ahorro de costos
```

#### **Hosts Dedicados**
- 🏠 **Servidor físico dedicado** a tu uso
- 🎯 **Mejor para:** Requisitos de cumplimiento, licenciamiento
- 📊 **Costo:** Opción más costosa
- ✅ **Pros:** Control total, cumplimiento, trae tus propias licencias
- ❌ **Contras:** Costo más alto, capacidad fija

### 🔄 **Auto Scaling**

#### 🤔 **¿Qué es Auto Scaling?**
Auto Scaling ajusta automáticamente **el número de instancias EC2** basado en la demanda, asegurando que tengas la capacidad correcta en el momento correcto.

#### 🎢 **Analogía del Mundo Real: Personal de Restaurante**
Auto Scaling es como **personal inteligente de restaurante**:
- 📈 **Hora pico de cena ocupada** → Llamar más meseros (escalar hacia arriba)
- 📉 **Martes lento por la tarde** → Enviar meseros a casa (escalar hacia abajo)
- 📊 **Monitorear flujo de clientes** → Ajustar niveles de personal automáticamente
- 💰 **Optimización de costos** → Pagar por personal solo cuando se necesita

#### 📊 **Ejemplo de Auto Scaling**
```
Auto Scaling de Sitio Web E-commerce:

Tráfico Normal (100 usuarios):
├── 2 instancias EC2 ejecutándose
├── Uso de CPU: 30%
└── Tiempo de respuesta: 200ms

Black Friday (10,000 usuarios):
├── Auto Scaling detecta CPU alto (80%)
├── Lanza 8 instancias adicionales
├── Tráfico distribuido entre 10 instancias
├── Uso de CPU: 35%
└── Tiempo de respuesta: 220ms

Después del Black Friday:
├── El tráfico regresa a normal
├── Auto Scaling termina instancias extra
├── De vuelta a 2 instancias
└── Costo optimizado automáticamente
```

### 🏷️ **Casos de Uso de EC2**

#### 🌐 **Hospedaje Web**
- **Escenario:** Sitio web de empresa con tráfico variable
- **Solución:** Grupo de Auto Scaling con Application Load Balancer
- **Beneficios:** Manejar picos de tráfico, optimización de costos
- **Tipo de instancia:** Propósito general (t3.medium)

#### 🎮 **Servidores de Juegos**
- **Escenario:** Juego multijugador en línea
- **Solución:** Instancias optimizadas para cómputo en múltiples regiones
- **Beneficios:** Baja latencia, alto rendimiento
- **Tipo de instancia:** Optimizado para cómputo (c5.large)

#### 📊 **Análisis de Datos**
- **Escenario:** Procesamiento de grandes datasets
- **Solución:** Instancias optimizadas para memoria con precios spot
- **Beneficios:** Alta memoria, costo-efectivo para trabajos por lotes
- **Tipo de instancia:** Optimizado para memoria (r5.xlarge)

---

## ⚡ AWS Lambda (Serverless Computing)

### 🤔 **¿Qué es AWS Lambda?**
AWS Lambda te permite **ejecutar código sin gestionar servidores**. Subes tu código, y AWS maneja todo lo demás - servidores, escalado, parches, monitoreo.

### 🏨 **Analogía del Mundo Real: Servicio a la Habitación del Hotel**
Lambda es como **servicio a la habitación del hotel**:
- 📞 **Llama cuando necesites algo** (activar función)
- 🍽️ **Servicio proporcionado instantáneamente** (código se ejecuta)
- 💰 **Paga solo por lo que ordenes** (paga por ejecución)
- 🧹 **No se requiere limpieza** (AWS maneja todo)
- ⏰ **Disponible 24/7** (siempre listo para responder)

### 🎯 **Conceptos Centrales de Lambda**

#### **Función**
- 📝 **Tu código** empaquetado con dependencias
- ⏱️ **Se ejecuta por máximo 15 minutos**
- 💾 **Asignación de memoria:** 128 MB a 10,008 MB
- 🔧 **Entornos de ejecución:** Python, Node.js, Java, C#, Go, Ruby

#### **Ejecución Basada en Eventos**
Las funciones Lambda son **activadas por eventos**:
```
Activadores Comunes:
├── 📁 Subida de archivo S3
├── 🌐 Solicitud de API Gateway
├── 📧 Notificación SNS
├── ⏰ Evento programado de CloudWatch
├── 🗄️ Cambio en tabla DynamoDB
└── 📱 Invocación de skill de Alexa
```

#### **Precios de Pago por Uso**
- 💰 **Sin servidores que pagar** cuando no está ejecutándose
- 📊 **Cobrado por solicitud** y tiempo de cómputo
- 🆓 **Nivel gratuito:** 1 millón de solicitudes/mes
- 💵 **Ejemplo de costo:** $0.20 por 1 millón de solicitudes

### 🎯 **Casos de Uso de Lambda**

#### 📸 **Procesamiento de Imágenes**
```
Escenario: App para compartir fotos

Flujo de Trabajo:
1. 📱 Usuario sube foto a S3
2. 🔔 S3 activa función Lambda
3. 🖼️ Lambda redimensiona imagen a múltiples tamaños
4. 💾 Guarda miniaturas de vuelta en S3
5. 📱 Actualiza base de datos con metadatos de imagen

Beneficios:
- Sin servidores que gestionar
- Escala automáticamente con subidas
- Paga solo cuando procesa imágenes
- Responde en tiempo real
```

#### 🔔 **Notificaciones en Tiempo Real**
```
Escenario: Procesamiento de órdenes e-commerce

Flujo de Trabajo:
1. 🛒 Cliente hace pedido en app
2. 📨 Datos de orden enviados a Lambda
3. 📧 Lambda envía email de confirmación
4. 📱 Envía notificación a app móvil
5. 📊 Actualiza dashboard de analítica

Beneficios:
- Respuesta instantánea a órdenes
- Sin infraestructura que mantener
- Escala con volumen de órdenes
- Costo-efectivo para eventos esporádicos
```

#### 🤖 **Backend de API**
```
Escenario: Backend de app móvil

Arquitectura:
API Gateway → Funciones Lambda → DynamoDB

Funciones:
├── Autenticación de usuario
├── Recuperación de datos
├── Procesamiento de lógica de negocio
└── Integraciones de terceros

Beneficios:
- Endpoints de API serverless
- Escalado automático
- Paga por llamada de API
- Enfoque en lógica de negocio
```

### ⚖️ **Comparación EC2 vs Lambda**

| **Aspecto** | **EC2** | **Lambda** |
|------------|---------|------------|
| **Gestión** | Tú gestionas servidores | AWS gestiona todo |
| **Escalado** | Manual/Auto Scaling | Automático e instantáneo |
| **Precios** | Paga por tiempo de servidor | Paga por ejecución |
| **Tiempo de ejecución** | Siempre ejecutándose | Se ejecuta solo cuando se activa |
| **Caso de uso** | Aplicaciones de larga duración | Funciones basadas en eventos |
| **Arranque en frío** | Siempre caliente | Posible retraso de arranque en frío |
| **Tiempo de ejecución** | Ilimitado | Máximo 15 minutos |

---

## 📦 Container Services

### 🤔 **¿Qué son los Contenedores?**
Los contenedores empaquetan tu **aplicación con todas sus dependencias** en una unidad portátil que se ejecuta consistentemente a través de diferentes entornos.

### 📦 **Analogía del Mundo Real: Contenedores de Envío**
Los contenedores son como **contenedores de envío estandarizados**:
- 📦 **Empaquetado estandarizado** - Mismo tamaño e interfaz en todas partes
- 🚢 **Portátil** - Se mueve de barco a camión a tren
- 🔒 **Aislado** - Los contenidos no se afectan entre sí
- 📋 **Control de inventario** - Saber exactamente qué hay adentro
- ⚡ **Carga eficiente** - Rápido de mover y desplegar

### 🐳 **Contenedor vs Máquina Virtual**

```
Máquina Virtual:
┌─────────────────────────────┐
│ Aplicación                  │
├─────────────────────────────┤
│ Sistema Operativo Invitado  │
├─────────────────────────────┤
│ Hipervisor                  │
├─────────────────────────────┤
│ Sistema Operativo Anfitrión │
├─────────────────────────────┤
│ Infraestructura Física     │
└─────────────────────────────┘

Contenedor:
┌─────────────────────────────┐
│ Aplicación                  │
├─────────────────────────────┤
│ Runtime de Contenedor       │
├─────────────────────────────┤
│ Sistema Operativo Anfitrión │
├─────────────────────────────┤
│ Infraestructura Física     │
└─────────────────────────────┘
```

### 🎯 **AWS Container Services**

#### **Amazon ECS (Elastic Container Service)**
- 🎯 **Orquestación de contenedores nativa de AWS**
- 🔧 **Completamente gestionado** por AWS
- 💰 **Sin cargos adicionales** por ECS en sí
- 🎮 **Fácil de usar** con servicios AWS

**Caso de Uso de ECS:**
```
Aplicación Web de Microservicios:
├── Contenedor frontend (app React)
├── Contenedor API (Node.js)
├── Contenedor de autenticación (Java)
└── Contenedor de base de datos (PostgreSQL)

Beneficios:
- Cada servicio escala independientemente
- Despliegue y actualizaciones fáciles
- Integrado con servicios AWS
- Operación costo-efectiva
```

#### **Amazon EKS (Elastic Kubernetes Service)**
- ☸️ **Servicio Kubernetes gestionado**
- 🌍 **Estándar de la industria** para orquestación de contenedores
- 🔧 **Plano de control gestionado por AWS**
- 🔗 **Compatible con herramientas Kubernetes existentes**

**Caso de Uso de EKS:**
```
Migración de Aplicación Empresarial:
├── Aplicaciones Kubernetes existentes
├── Requisitos de estrategia multi-nube
├── Necesidades de orquestación avanzada
└── Equipos de desarrollo grandes

Beneficios:
- Usar experiencia Kubernetes existente
- Portátil entre proveedores de nube
- Programación y redes avanzadas
- Rico ecosistema de herramientas
```

#### **AWS Fargate**
- 🚫 **Contenedores serverless** - Sin gestión de servidores
- 💰 **Paga solo por recursos usados**
- 🔄 **Funciona con ECS y EKS**
- ⚡ **Escalado instantáneo**

**Caso de Uso de Fargate:**
```
Procesamiento Basado en Eventos:
├── Contenedor activado por eventos
├── Procesa datos y termina
├── Sin servidores que gestionar
└── Paga solo durante ejecución

Beneficios:
- Sin gestión de infraestructura
- Perfecto para trabajos por lotes
- Escalado automático
- Optimización de costos
```

---

## 🌟 Servicios de Cómputo Especializados

### 🏢 **Amazon Lightsail**

#### 🤔 **¿Qué es Lightsail?**
Amazon Lightsail proporciona **servidores virtuales privados simples** con precios predecibles para aplicaciones de pequeña escala.

#### 🎯 **Analogía del Mundo Real: Apartamento Estudio**
Lightsail es como un **apartamento estudio amueblado**:
- 🏠 **Todo incluido** - Servidor, almacenamiento, redes
- 💰 **Precio mensual fijo** - Costos predecibles
- 🎯 **Configuración simple** - Sin configuración compleja
- 📊 **Perfecto para necesidades pequeñas** - Proyectos personales, pequeños negocios

#### 💼 **Casos de Uso de Lightsail**
- 🌐 **Sitios web simples** - WordPress, sitios estáticos
- 🛒 **E-commerce pequeño** - Tiendas en línea básicas
- 👨‍💻 **Entornos de desarrollo** - Pruebas y prototipado
- 📚 **Proyectos de aprendizaje** - Estudiantes y principiantes

### ⚙️ **AWS Batch**

#### 🤔 **¿Qué es AWS Batch?**
AWS Batch **gestiona cargas de trabajo de procesamiento por lotes**, aprovisionando y escalando automáticamente recursos de cómputo.

#### 🏭 **Analogía del Mundo Real: Línea de Producción de Fábrica**
Batch es como una **fábrica automatizada**:
- 📋 **Cola de trabajos** - Órdenes esperando ser procesadas
- 🏭 **Línea de producción** - Recursos de cómputo haciendo trabajo
- 🔄 **Escalado automático** - Agregar/quitar líneas de producción basado en órdenes
- 📊 **Control de calidad** - Monitorear y gestionar completación de trabajos

#### 💼 **Casos de Uso de Batch**
- 🧬 **Computación científica** - Análisis genómico, modelado climático
- 📊 **Análisis financiero** - Cálculos de riesgo, optimización de portafolio
- 🎬 **Procesamiento de medios** - Renderizado de video, análisis de imágenes
- 📈 **Procesamiento de datos** - Trabajos ETL, análisis de logs

### 🏢 **AWS Outposts**

#### 🤔 **¿Qué es AWS Outposts?**
AWS Outposts trae **servicios AWS a tu centro de datos on-premises**, proporcionando capacidades de nube híbrida.

#### 🏠 **Analogía del Mundo Real: Extensión de Oficina en Casa**
Outposts es como **extender tu oficina a tu casa**:
- 🏢 **Mismas herramientas** - Usar los mismos servicios AWS on-premises
- 🔗 **Conectado** - Integración perfecta con la nube AWS
- 🔒 **Control local** - Mantener datos sensibles on-premises
- 📊 **Experiencia consistente** - Mismas APIs y herramientas de gestión

#### 💼 **Casos de Uso de Outposts**
- 🏥 **Salud** - Mantener datos de pacientes on-premises para cumplimiento
- 🏭 **Manufactura** - Procesamiento de baja latencia para automatización de fábrica
- 🏛️ **Gobierno** - Requisitos de soberanía de datos
- 💰 **Servicios financieros** - Aplicaciones de trading de ultra-baja latencia

---

## 🎯 Eligiendo el Servicio de Cómputo Correcto

### 🤔 **Marco de Decisión**

#### **Haz Estas Preguntas:**

1. **🏗️ ¿Cuánto control necesitas?**
   - **Control total** → EC2
   - **Sin gestión de servidores** → Lambda o Fargate
   - **Configuración simple** → Lightsail

2. **⏰ ¿Por cuánto tiempo se ejecuta tu código?**
   - **Siempre ejecutándose** → EC2
   - **Tareas cortas (< 15 min)** → Lambda
   - **Trabajos por lotes** → Batch o instancias Spot

3. **📈 ¿Qué tan predecible es tu carga de trabajo?**
   - **Uso constante** → Instancias Reservadas
   - **Variable/con picos** → Auto Scaling o Lambda
   - **Impredecible/interrumpible** → Instancias Spot

4. **💰 ¿Cuál es tu prioridad de costo?**
   - **Costo más bajo** → Instancias Spot o Lambda
   - **Costo predecible** → Instancias Reservadas o Lightsail
   - **Pago por uso** → Lambda o Fargate

### 📊 **Matriz de Selección de Servicios**

| **Caso de Uso** | **Mejor Servicio** | **Por Qué** |
|--------------|------------------|---------|
| **Sitio web corporativo** | EC2 + Auto Scaling | Rendimiento consistente, optimización de costos |
| **Procesamiento de imágenes** | Lambda | Basado en eventos, pago por uso |
| **App de microservicios** | ECS/EKS + Fargate | Beneficios de contenedores, sin gestión de servidores |
| **Blog personal** | Lightsail | Simple, precios predecibles |
| **Análisis de datos** | Batch + Spot | Procesamiento por lotes costo-efectivo |
| **Servidor de juegos** | EC2 Dedicado | Rendimiento consistente, control total |

### 🏗️ **Patrones de Arquitectura**

#### **Aplicación Web Simple**
```
Internet → ALB → EC2 (Auto Scaling) → RDS
├── Application Load Balancer distribuye tráfico
├── Auto Scaling ajusta capacidad
├── Instancias EC2 ejecutan aplicación
└── RDS proporciona backend de base de datos
```

#### **API Serverless**
```
App Móvil → API Gateway → Lambda → DynamoDB
├── API Gateway maneja solicitudes HTTP
├── Funciones Lambda procesan lógica de negocio
├── DynamoDB almacena datos de aplicación
└── Paga solo por uso real
```

#### **Plataforma de Microservicios**
```
Usuarios → ALB → Servicios ECS/Fargate → Varios Backends
├── Load balancer enruta a servicios apropiados
├── Cada microservicio se ejecuta en contenedores
├── Servicios escalan independientemente
└── Fargate elimina gestión de servidores
```

---

## 📝 Escenarios del Mundo Real

### 🛒 **Escenario 1: Startup E-commerce**

**Situación:**
- Nueva tienda en línea lanzándose
- Esperando tráfico variable
- Presupuesto limitado y experiencia técnica
- Necesidad de escalar rápidamente si es exitoso

**Requisitos:**
- Manejar picos de tráfico durante ventas
- Solución costo-efectiva
- Fácil de gestionar
- Despliegue rápido

**Solución Recomendada:**
```
Arquitectura:
├── Lightsail para sitio web inicial simple
├── Migrar a EC2 + Auto Scaling cuando inicie el crecimiento
├── Lambda para funciones de procesamiento de órdenes
└── Considerar contenedores mientras la app crece en complejidad

Ruta de Migración:
Fase 1: Lightsail (simple, predecible)
Fase 2: EC2 + Auto Scaling (manejar crecimiento)
Fase 3: Microservicios en contenedores (escalar complejidad)
```

**Beneficios:**
- Empezar simple y costo-efectivo
- Escalar arquitectura con crecimiento del negocio
- Pagar por lo que realmente usas
- Enfocarse en el negocio, no en infraestructura

### 🏥 **Escenario 2: Procesamiento de Datos de Salud**

**Situación:**
- Procesar datos de imágenes médicas
- Archivos grandes, computación intensiva
- Procesamiento por lotes durante la noche
- Requisitos estrictos de cumplimiento

**Requisitos:**
- Alto poder de cómputo cuando se necesite
- Optimización de costos para cargas de trabajo por lotes
- Cumplimiento con regulaciones de salud
- Procesamiento confiable de datos críticos

**Solución Recomendada:**
```
Arquitectura:
├── S3 para almacenamiento de imágenes médicas
├── Batch para orquestar trabajos de procesamiento
├── Instancias Spot para cómputo costo-efectivo
├── Lambda para activar y monitorear
└── CloudTrail para auditoría de cumplimiento

Flujo de Trabajo:
1. Imágenes médicas subidas a S3
2. Lambda activa trabajo Batch
3. Batch aprovisiona Instancias Spot
4. Imágenes procesadas durante la noche
5. Resultados almacenados de vuelta en S3
6. Instancias terminadas automáticamente
```

**Beneficios:**
- 70% de ahorro de costos con Instancias Spot
- Escalado automático para cargas de trabajo variables
- Características de cumplimiento integradas
- Sin sobrecarga de gestión de infraestructura

### 🎮 **Escenario 3: Backend de Juegos Móviles**

**Situación:**
- Juego móvil multijugador
- Base de jugadores global
- Interacciones en tiempo real requeridas
- Actividad de jugadores impredecible

**Requisitos:**
- Baja latencia a nivel mundial
- Manejar jugadores concurrentes
- Procesamiento de datos en tiempo real
- Optimización de costos para carga variable

**Solución Recomendada:**
```
Arquitectura:
├── API Gateway para endpoints de API globales
├── Lambda para funciones de lógica de juego
├── DynamoDB para datos de jugadores (tablas globales)
├── ECS para sesiones de juego en tiempo real
└── CloudFront para entrega de contenido

Estrategia de Escalado:
- Lambda maneja autenticación/estadísticas de jugadores
- ECS gestiona sesiones de juego en tiempo real
- Auto Scaling se ajusta al conteo de jugadores
- Despliegue global para baja latencia
```

**Beneficios:**
- Serverless escala automáticamente
- Baja latencia global
- Pago por actividad de jugador
- Enfoque en desarrollo de juegos

---

## 🧠 Ayudas de Memoria

### 🎯 **Trucos de Memoria para Servicios**

#### **EC2 = Elastic Compute Cloud**
- **E**lástico = Escala hacia arriba y abajo
- **C**ómputo = Poder de procesamiento
- **C**loud = Servidores virtuales en AWS

#### **Lambda = Funciones Serverless**
- **λ (Símbolo Lambda)** = Función matemática
- **Basado en eventos** = Responde a activadores
- **Pago por ejecución** = Sin costos de inactividad

#### **Servicios de Contenedores**
- **ECS** = **E**lastic **C**ontainer **S**ervice (nativo de AWS)
- **EKS** = **E**lastic **K**ubernetes **S**ervice (estándar de la industria)
- **Fargate** = **Far**away **gate** = Sin servidores que ver

### 📊 **Árbol de Decisión**
```
¿Necesitas cómputo? Empieza aquí:
├── ¿Siempre ejecutándose? 
│   ├── Sí → EC2 (con Auto Scaling)
│   └── No → ¿Basado en eventos?
│       ├── Sí → Lambda
│       └── No → ¿Procesamiento por lotes?
│           ├── Sí → AWS Batch
│           └── No → Considerar contenedores
├── ¿Necesitas contenedores?
│   ├── Simple → ECS
│   ├── Kubernetes → EKS
│   └── Sin servidores → Fargate
└── ¿Quieres simplicidad? → Lightsail
```

---

## ✅ Lista de Verificación del Capítulo

Antes de proceder, asegúrate de poder:

- [ ] Explicar cuándo usar EC2 vs Lambda vs contenedores
- [ ] Entender modelos de precios de EC2 (Bajo Demanda, Reservadas, Spot)
- [ ] Identificar beneficios y casos de uso de Auto Scaling
- [ ] Reconocer ventajas de computación serverless
- [ ] Elegir servicios de contenedores apropiados
- [ ] Hacer coincidir servicios de cómputo con escenarios de negocio
- [ ] Entender estrategias de optimización de costos

---

## 🎯 Preguntas de Práctica

### Pregunta 1
Una empresa tiene una aplicación web que experimenta tráfico predecible durante horas de negocio pero muy poco tráfico en las noches y fines de semana. ¿Qué solución de cómputo sería más costo-efectiva?

A) Instancias Reservadas EC2
B) EC2 Bajo Demanda con Auto Scaling
C) AWS Lambda
D) Hosts Dedicados EC2

<details>
<summary>💡 Haz clic para ver la Respuesta</summary>

**Respuesta: B) EC2 Bajo Demanda con Auto Scaling**

**Explicación:** Auto Scaling con instancias Bajo Demanda permite que la aplicación escale hacia abajo durante períodos de bajo tráfico y escale hacia arriba durante horas de negocio, pagando solo por la capacidad realmente necesitada. Lambda sería mejor para cargas de trabajo impredecibles basadas en eventos, mientras que las Instancias Reservadas son mejores para uso consistente 24/7.
</details>

### Pregunta 2
Una startup necesita procesar imágenes subidas redimensionándolas y aplicando filtros. El procesamiento se activa cuando las imágenes se suben a S3. ¿Qué servicio es más adecuado para este caso de uso?

A) Amazon EC2
B) AWS Lambda
C) Amazon ECS
D) AWS Batch

<details>
<summary>💡 Haz clic para ver la Respuesta</summary>

**Respuesta: B) AWS Lambda**

**Explicación:** Lambda es perfecto para procesamiento basado en eventos activado por subidas a S3. Escala automáticamente, no requiere gestión de servidores, y pagas solo cuando las imágenes son procesadas. La tarea de procesamiento de imágenes de corta duración encaja bien dentro de los límites de tiempo de ejecución de Lambda.
</details>

### Pregunta 3
¿Qué modelo de precios de EC2 ofrece el mayor descuento pero requiere un compromiso de 1-3 años?

A) Instancias Bajo Demanda
B) Instancias Spot
C) Instancias Reservadas
D) Hosts Dedicados

<details>
<summary>💡 Haz clic para ver la Respuesta</summary>

**Respuesta: C) Instancias Reservadas**

**Explicación:** Las Instancias Reservadas ofrecen hasta 75% de ahorros comparado con precios Bajo Demanda a cambio de un compromiso de 1 o 3 años. Mientras que las Instancias Spot pueden ofrecer hasta 90% de ahorros, no requieren compromisos pero pueden ser terminadas con poco aviso.
</details>

---

## 🗺️ ¿Qué Sigue?

Ahora que entiendes cómo ejecutar aplicaciones en la nube, exploremos dónde y cómo almacenar los datos que tus aplicaciones necesitan.

**🎯 Siguiente Capítulo:** [Servicios de Almacenamiento](./storage-services.md)

¡Aprende sobre las varias opciones de almacenamiento que AWS proporciona y cuándo usar cada una!

---

**🎉 ¡Excelente base!** Ahora entiendes los servicios de cómputo que impulsan las aplicaciones en la nube. A continuación, exploraremos dónde viven todos esos datos.

---

**← [Volver a Resumen del Dominio 3](./README.md)**
