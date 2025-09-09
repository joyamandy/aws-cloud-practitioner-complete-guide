# 💰 Modelos de Precios de AWS

> **Entendiendo Cómo Pagas por la Nube | Tiempo de Estudio: ~3 horas**

Imagina los precios de AWS como **diferentes formas de usar un gimnasio**:
- **Pase diario** (On-Demand) - Pagas cada vez que vas, más caro por visita
- **Membresía anual** (Reserved) - Pagas por adelantado por un año, mucho más barato por visita
- **Horas de menor demanda** (Spot) - Usas el gimnasio en horarios menos ocupados por grandes descuentos
- **Membresía flexible** (Savings Plans) - Te comprometes a ir regularmente, obtienes descuentos en todo

¡AWS te da la misma flexibilidad con los recursos de la nube! 🏋️‍♂️

---

## 📋 Tabla de Contenidos

- [🎯 Objetivos de Aprendizaje](#-objetivos-de-aprendizaje)
- [💡 Fundamentos de Precios de AWS](#-fundamentos-de-precios-de-aws)
- [💻 Precios On-Demand](#-precios-on-demand)
- [🏦 Instancias Reservadas](#-instancias-reservadas)
- [⚡ Instancias Spot](#-instancias-spot)
- [💰 Planes de Ahorro](#-planes-de-ahorro)
- [🆓 Nivel Gratuito de AWS](#-nivel-gratuito-de-aws)
- [📊 Precios Específicos por Servicio](#-precios-específicos-por-servicio)
- [🧮 Estimación de Costos](#-estimación-de-costos)
- [📝 Preguntas de Práctica](#-preguntas-de-práctica)

---

## 🎯 Objetivos de Aprendizaje

Al final de este capítulo, podrás:

✅ **Entender los principios de precios de AWS** y cómo difieren de la TI tradicional  
✅ **Comparar modelos de precios** y elegir el correcto para diferentes escenarios  
✅ **Calcular ahorros potenciales** con Instancias Reservadas y Planes de Ahorro  
✅ **Identificar beneficios del nivel gratuito** y limitaciones  
✅ **Estimar costos** para servicios comunes de AWS  
✅ **Reconocer oportunidades de optimización de costos** en la selección de modelos de precios  

---

## 💡 Fundamentos de Precios de AWS

### 🌟 **Principios Fundamentales de Precios**

#### **💳 Pago por Uso**
Piénsalo como **pagar por electricidad**:
- **Sin tarifas mínimas** - Paga solo por lo que usas
- **Sin costos iniciales** - Comienza a usar servicios inmediatamente
- **Sin tarifas de terminación** - Para en cualquier momento sin penalizaciones
- **Facturación granular** - Paga por hora, minuto, o incluso segundo

**Beneficios:**
- **Menores barreras de entrada** - Sin grandes inversiones iniciales
- **Flexibilidad** - Escala hacia arriba o abajo según las necesidades
- **Experimentación** - Prueba nuevos servicios sin compromisos importantes
- **Flujo de caja amigable** - Gastos operativos vs gastos de capital

#### **📈 Descuentos por Volumen**
**Mientras más uses, menos pagas por unidad:**
- **Almacenamiento S3** - Costos más bajos por GB en volúmenes altos
- **Instancias EC2** - Descuentos por volumen para grandes despliegues
- **Transferencia de datos** - Precios escalonados con volúmenes altos costando menos
- **Planes de soporte** - Precios basados en porcentaje escalan con el uso

#### **💰 Sin Costos Iniciales (A Menos que los Elijas)**
**Modelo predeterminado:**
- **Comenzar inmediatamente** - Sin proceso de adquisición
- **Pagar mensualmente** - Ciclos de facturación predecibles
- **Escalar orgánicamente** - Hacer crecer la infraestructura con el negocio
- **Compromisos opcionales** - Elegir términos más largos para descuentos

### 🏗️ **Qué Impulsa los Costos de AWS**

#### **🖥️ Costos de Cómputo**
**Factores que afectan los precios de cómputo:**
- **Tipo de instancia** - CPU, memoria, rendimiento de red
- **Tamaño de instancia** - Pequeña vs grande dentro de la misma familia
- **Sistema operativo** - Licenciamiento Linux vs Windows
- **Región** - La ubicación geográfica afecta los precios
- **Tiempo de uso** - Facturado por segundo (mínimo 1 minuto)

#### **💾 Costos de Almacenamiento**
**Factores de precios de almacenamiento:**
- **Tipo de almacenamiento** - SSD vs HDD, niveles de rendimiento
- **Volumen** - Cantidad de datos almacenados
- **Patrones de acceso** - Acceso frecuente vs infrecuente
- **Duración** - Cuánto tiempo se almacenan los datos
- **Solicitudes** - Número de operaciones de lectura/escritura

#### **🌐 Costos de Red**
**Precios de transferencia de datos:**
- **Entrante** - Usualmente gratis (datos llegando a AWS)
- **Saliente** - Cobrado por GB (datos saliendo de AWS)
- **Entre regiones** - Entre regiones de AWS
- **Entre AZ** - Entre Zonas de Disponibilidad
- **CloudFront** - Uso de red de entrega de contenido

#### **🔧 Servicios Adicionales**
**Otros factores de costo:**
- **Balanceadores de carga** - Por hora + datos procesados
- **Gateways NAT** - Por hora + datos procesados
- **Llamadas API** - Muchos servicios cobran por solicitud
- **Planes de soporte** - Niveles de soporte pagados opcionales

---

## 💻 Precios Bajo Demanda

### 🎯 **¿Qué son los Precios Bajo Demanda?**

Piensa en Bajo Demanda como **pedir comida a domicilio**:
- **Pagar precio completo del menú** - Sin descuentos, pero máxima conveniencia
- **Disponible inmediatamente** - Sin espera o planificación requerida
- **Pagar por pedido** - Solo pagas cuando realmente pides
- **Sin pedidos mínimos** - Pide tan poco o tanto como quieras

### ⚡ **Características de Bajo Demanda**

#### **💳 Modelo de Pago**
- **Pagar por hora** - La mayoría de servicios facturan por hora
- **Pagar por segundo** - EC2 y algunos otros (mínimo 1 minuto)
- **Pagar por solicitud** - Lambda, API Gateway, muchos servicios administrados
- **Sin pago inicial** - Comenzar a usar inmediatamente

#### **🚀 Beneficios**
- **Máxima flexibilidad** - Iniciar y detener en cualquier momento
- **Sin planificación requerida** - Sin planificación de capacidad o pronósticos
- **Perfecto para experimentación** - Probar nuevos servicios sin riesgo
- **Ideal para cargas de trabajo impredecibles** - El tráfico varía significativamente

#### **💰 Compromisos**
- **Costo más alto por unidad** - Modelo de precios más caro
- **Sin descuentos por volumen** - Cada hora cuesta lo mismo
- **Impredecibilidad presupuestaria** - Los costos varían con el uso

### 🎯 **Cuándo Usar Bajo Demanda**

#### **✅ Escenarios Perfectos**
- **Desarrollo y pruebas** - Crear recursos según sea necesario
- **Proyectos a corto plazo** - Proyectos que duran días o semanas
- **Cargas de trabajo impredecibles** - Los patrones de tráfico varían significativamente
- **Aprendizaje y experimentación** - Explorar nuevos servicios de AWS
- **Recuperación ante desastres** - Recursos necesarios solo durante emergencias

#### **📊 Casos de Uso de Ejemplo**

**🔬 Entorno de Desarrollo**
```
Patrón de Uso Diario:
├── 9 AM - 6 PM: Desarrollo activo (9 horas)
├── 6 PM - 9 AM: Apagar para ahorrar costos (15 horas)
└── Fines de semana: Uso ocasional (variable)

Optimización de Costos:
- Usar Bajo Demanda para horarios flexibles
- Apagar cuando no se necesite
- Sin compromiso requerido
```

**📈 Campaña de Marketing**
```
Duración de Campaña: 2 semanas
├── Semana 1: Aumentar tráfico gradualmente
├── Semana 2: Tráfico pico, luego declive rápido
└── Post-campaña: Tráfico mínimo

Por qué Bajo Demanda:
- Patrones de tráfico desconocidos
- Duración corta
- Necesidad de escalar rápidamente
```

---

## 🏦 Instancias Reservadas

### 🏠 **¿Qué son las Instancias Reservadas?**

Piensa en las Instancias Reservadas como **firmar una membresía de gimnasio**:
- **Pagar por adelantado** por una membresía de 1 o 3 años
- **Obtener descuentos significativos** comparado con pases diarios
- **Compromiso requerido** - No puedes cancelar sin perder dinero
- **Mejor valor** si lo usas consistentemente

### 💰 **Tipos de Instancias Reservadas**

#### **📊 Instancias Reservadas Estándar**
**Máximos ahorros, menor flexibilidad**

**Características:**
- **Hasta 75% de ahorros** vs Bajo Demanda
- **Términos de 1 o 3 años** - Términos más largos = mayores descuentos
- **Alcance regional** - Usar en cualquier lugar de la región seleccionada
- **Familia de instancia bloqueada** - No puedes cambiar el tipo de instancia significativamente

**Opciones de Pago:**
- **Todo por Adelantado** - Pagar todo el costo por adelantado (máximo descuento)
- **Parcial por Adelantado** - Pagar algo por adelantado, resto mensual
- **Sin Adelanto** - Pagar mensualmente (menor descuento)

#### **🔄 Instancias Reservadas Convertibles**
**Buenos ahorros, más flexibilidad**

**Características:**
- **Hasta 54% de ahorros** vs Bajo Demanda (menos que Estándar)
- **Capacidad de intercambio** - Cambiar tipos de instancia, SO, tenencia
- **Mismas opciones de pago** - Todo, Parcial, o Sin Adelanto
- **Preparación para el futuro** - Adaptarse a necesidades cambiantes

**Ejemplos de Intercambio:**
```
Original: m5.large Linux → m5.xlarge Linux (más grande)
Original: m5.large Linux → c5.large Linux (familia diferente)
Original: m5.large Linux → m5.large Windows (SO diferente)
```

#### **🎯 Instancias Reservadas Programadas**
**Para uso recurrente predecible**

**Casos de Uso:**
- **Solo horas de negocio** - 9 AM - 5 PM, Lunes-Viernes
- **Procesamiento por lotes** - Misma hora cada noche
- **Reportes semanales** - Cada domingo por 4 horas
- **Patrones estacionales** - Procesamiento de días festivos

### 📊 **Ejemplos de Ahorros de Instancias Reservadas**

#### **💻 Ejemplo: Servidor Web**
```
Escenario: instancia m5.large funcionando 24/7 por 1 año

Costo Bajo Demanda:
├── $0.096 por hora × 24 horas × 365 días = $841.60/año

Reservada Estándar (1 año, Todo por Adelantado):
├── $504 pago por adelantado = $504/año
└── Ahorros: $337.60 (40% de ahorros)

Reservada Estándar (3 años, Todo por Adelantado):
├── $304 pago por adelantado = $304/año
└── Ahorros: $537.60 (64% de ahorros)
```

#### **🗄️ Ejemplo: Servidor de Base de Datos**
```
Escenario: base de datos r5.xlarge funcionando continuamente

Costo Bajo Demanda: $0.252/hora × 8,760 horas = $2,207.52/año

Opciones de Instancia Reservada:
├── 1 año Estándar: $1,460 (34% de ahorros)
├── 3 años Estándar: $1,200 (46% de ahorros)
└── 3 años Convertible: $1,350 (39% de ahorros)

Mejor Opción: 3 años Estándar si los requisitos no cambiarán
Alternativa: 3 años Convertible para flexibilidad
```

### 🎯 **Mejores Prácticas de Instancias Reservadas**

#### **📊 Análisis de Uso**
**Antes de comprar Instancias Reservadas:**
1. **Analizar uso histórico** - 3-6 meses de datos
2. **Identificar cargas de trabajo estables** - Uso consistente 24/7
3. **Considerar crecimiento** - No comprar en exceso
4. **Considerar familias de instancias** - Estándar vs Convertible

#### **🔄 Estrategias de Gestión**
- **Comenzar con términos de 1 año** - Menor compromiso para aprender
- **Mezclar opciones de pago** - Equilibrar ahorros vs flujo de caja
- **Usar Convertible para incertidumbre** - Cuando las necesidades futuras no están claras
- **Monitorear utilización** - Asegurar que obtienes valor

---

## ⚡ Instancias Spot

### 🎰 **¿Qué son las Instancias Spot?**

Piensa en las Instancias Spot como **boletos de avión en lista de espera**:
- **Descuentos enormes** (hasta 90% de descuento) si eres flexible
- **Disponibles cuando hay capacidad de sobra**
- **Pueden ser retiradas** con aviso de 2 minutos
- **Perfectas para cargas de trabajo flexibles y tolerantes a fallos**

### 🔧 **Cómo Funcionan las Instancias Spot**

#### **💰 Precios Spot**
```
Ejemplo de Fluctuación de Precio Spot:
├── Lunes: $0.05/hora (alta disponibilidad)
├── Martes: $0.15/hora (demanda moderada)
├── Miércoles: $0.45/hora (alta demanda)
└── Jueves: $0.08/hora (baja demanda otra vez)

Tu Oferta: $0.20/hora
├── Lunes-Martes: Instancia funciona (precio debajo de oferta)
├── Miércoles: Instancia terminada (precio arriba de oferta)
└── Jueves: Instancia disponible otra vez
```

#### **⚡ Ciclo de Vida de Instancia Spot**
1. **Solicitar Instancia Spot** - Establecer precio máximo que pagarás
2. **Instancia se lanza** - Cuando precio spot ≤ tu oferta
3. **Instancia funciona normalmente** - Funcionalidad completa de EC2
4. **Precio aumenta** - Arriba de tu oferta máxima
5. **Aviso de 2 minutos** - Notificación de interrupción de instancia spot
6. **Instancia termina** - Automáticamente detenida o terminada

### 🎯 **Casos de Uso Perfectos para Instancias Spot**

#### **✅ Cargas de Trabajo Ideales**
- **Procesamiento por lotes** - Trabajos que pueden reiniciar
- **Análisis de datos** - Trabajos MapReduce, analíticos
- **Procesamiento de imagen/video** - Renderizado, transcodificación
- **Rastreo web** - Tolerante a fallos por naturaleza
- **Pipelines CI/CD** - Entornos de construcción y prueba
- **Entrenamiento de aprendizaje automático** - Puede hacer checkpoint y reanudar

#### **❌ Evitar Instancias Spot Para**
- **Servidores web de producción** - Necesitan disponibilidad garantizada
- **Bases de datos** - Riesgo de pérdida de datos en terminación
- **Aplicaciones en tiempo real** - No pueden tolerar interrupciones
- **Trabajos sin checkpointing** - No pueden reanudar desde donde se quedaron

### 🛠️ **Estrategias de Instancias Spot**

#### **🔄 Flota Spot**
**Mezcla de tipos de instancia para mejor disponibilidad:**
```
Configuración de Flota Spot:
├── Tipos de Instancia: m5.large, m5.xlarge, c5.large, c5.xlarge
├── Zonas de Disponibilidad: us-east-1a, us-east-1b, us-east-1c
├── Estrategia de Asignación: Diversificada
└── Capacidad Objetivo: 10 instancias

Beneficios:
├── Mayor disponibilidad (múltiples tipos de instancia)
├── Mejor precio (puede elegir el más barato disponible)
└── Reemplazo automático (si las instancias son terminadas)
```

#### **💾 Estrategia de Checkpointing**
**Guardar progreso regularmente:**
```
Diseño de Trabajo por Lotes:
├── Procesar datos en fragmentos
├── Guardar progreso cada 30 minutos
├── Almacenar checkpoint en S3
├── Reanudar desde último checkpoint si se interrumpe
└── Resultados finales guardados en almacenamiento persistente
```

### 📊 **Ejemplos de Ahorros de Instancias Spot**

#### **🔬 Procesamiento de Datos**
```
Carga de Trabajo: 100 horas de procesamiento de datos por mes
Instancia: c5.2xlarge

Costo Bajo Demanda:
├── $0.34/hora × 100 horas = $34/mes

Costo Spot (promedio 70% descuento):
├── $0.10/hora × 100 horas = $10/mes
└── Ahorros: $24/mes (70% de ahorros)

Ahorros Anuales: $288 (significativo para cargas de trabajo continuas)
```

#### **🎥 Procesamiento de Video**
```
Carga de Trabajo: Transcodificación nocturna de video
Duración: 4 horas/noche × 30 días = 120 horas/mes
Instancia: m5.4xlarge

Comparación:
├── Bajo Demanda: $0.768/hora × 120 = $92.16/mes
├── Promedio Spot: $0.20/hora × 120 = $24/mes
└── Ahorros: $68.16/mes (74% de ahorros)

Mitigación de Riesgo:
├── Trabajo diseñado para reanudar desde interrupción
├── Múltiples tipos de instancia en Flota Spot
└── Respaldo a Bajo Demanda si es necesario
```

---

## 💰 Planes de Ahorro

### 🎯 **¿Qué son los Planes de Ahorro?**

Piensa en los Planes de Ahorro como **comprar energía al por mayor** para tu hogar:
- **Comprometerse a usar** cierta cantidad de electricidad por hora
- **Obtener descuentos** en todo tu uso eléctrico
- **Flexibilidad** en cómo usas esa electricidad
- **Aplicación automática** a tus facturas más altas primero

### 🔄 **Tipos de Planes de Ahorro**

#### **💻 Planes de Ahorro de Cómputo**
**Más flexibles, buenos ahorros**

**Características:**
- **Hasta 66% de ahorros** vs Bajo Demanda
- **Se aplica a uso de EC2, Lambda y Fargate**
- **Flexibilidad de familia de instancia** - Cambiar tamaños, SO, tenencia
- **Flexibilidad de región** - Mover cargas de trabajo entre regiones

**Mejor Para:**
- **Cargas de trabajo mixtas** - EC2 + serverless
- **Entornos dinámicos** - Requisitos cambiantes
- **Despliegues multi-región**

#### **🖥️ Planes de Ahorro de Instancias EC2**
**Máximos ahorros, enfocado en EC2**

**Características:**
- **Hasta 72% de ahorros** vs Bajo Demanda (máximos ahorros)
- **Solo instancias EC2** - No se aplica a Lambda/Fargate
- **Compromiso de familia de instancia** - Bloqueado a familia específica
- **Flexibilidad de tamaño y SO** - Puede cambiar dentro de la familia

**Mejor Para:**
- **Cargas de trabajo EC2 estables** - Necesidades de cómputo predecibles
- **Entornos estandarizados** - Familias de instancia consistentes
- **Máximos ahorros** - Cuando no se necesita flexibilidad

### 📊 **Planes de Ahorro vs Instancias Reservadas**

| **Característica** | **Planes de Ahorro** | **Instancias Reservadas** |
|--------------------|----------------------|---------------------------|
| **Flexibilidad** | Alta | Media (Convertible) / Baja (Estándar) |
| **Servicios** | EC2, Lambda, Fargate | Solo EC2 |
| **Compromiso** | Uso $/hora | Tipo de instancia específico |
| **Ahorros** | Hasta 72% | Hasta 75% |
| **Gestión** | Aplicación automática | Coincidencia manual de instancia |
| **Mejor Para** | Cargas mixtas/dinámicas | Cargas estables, predecibles |

### 🎯 **Ejemplos de Planes de Ahorro**

#### **💡 Plan de Ahorro de Cómputo**
```
Compromiso: $10/hora por 1 año

Escenario de Uso:
├── Instancias EC2: $6/hora de uso
├── Funciones Lambda: $2/hora de uso
├── Contenedores Fargate: $1/hora de uso
└── Total cubierto: $9/hora

Beneficios:
├── Todo el uso obtiene tarifas de Plan de Ahorro
├── $1/hora de compromiso restante sin usar
├── Tarifas Bajo Demanda se aplican a uso arriba de $10/hora
└── Flexibilidad para cambiar mezcla de servicios
```

#### **🖥️ Plan de Ahorro de Instancias EC2**
```
Uso Actual: 10 × instancias m5.large (24/7)
Costo Mensual Bajo Demanda: $691.20

Análisis de Plan de Ahorro:
├── Compromiso: $0.062/hora por instancia
├── Costo Mensual Plan de Ahorro: $446.40
├── Ahorros Mensuales: $244.80 (35% de ahorros)
└── Ahorros Anuales: $2,937.60

Beneficios de Flexibilidad:
├── Puede cambiar a m5.xlarge (menos instancias)
├── Puede cambiar a Windows si es necesario
├── Puede moverse entre AZs en la misma región
└── Aplicación automática a costos más altos
```

---

## 🆓 Nivel Gratuito de AWS

### 🎁 **¿Qué es el Nivel Gratuito de AWS?**

Piensa en el Nivel Gratuito de AWS como **muestras gratis en una tienda**:
- **Probar antes de comprar** - Experimentar servicios de AWS sin costo
- **Cantidades limitadas** - Cantidades específicas de cada servicio
- **Límites de tiempo** - La mayoría de beneficios duran 12 meses
- **Sin trucos de tarjeta de crédito** - Verdaderamente gratis con monitoreo de uso

### 📅 **Categorías del Nivel Gratuito**

#### **🗓️ Nivel Gratuito de 12 Meses**
**Comienza desde la fecha de creación de tu cuenta AWS**

**Servicios Clave:**
```
Amazon EC2:
├── 750 horas/mes de instancias t2.micro o t3.micro
├── Linux y Windows cubiertos
└── Suficiente para 1 instancia funcionando 24/7

Amazon S3:
├── 5 GB de almacenamiento estándar
├── 20,000 solicitudes GET
├── 2,000 solicitudes PUT
└── 15 GB de transferencia de datos saliente

Amazon RDS:
├── 750 horas/mes de instancia db.t2.micro
├── 20 GB de almacenamiento de base de datos
├── 20 GB de almacenamiento de respaldo
└── MySQL, PostgreSQL, MariaDB cubiertos

Amazon CloudFront:
├── 50 GB transferencia de datos saliente
├── 2,000,000 solicitudes HTTP/HTTPS
└── Ubicaciones de borde globales incluidas
```

#### **♾️ Siempre Gratis**
**Sin expiración - gratis para siempre**

**Servicios Clave:**
```
AWS Lambda:
├── 1 millón de solicitudes por mes
├── 400,000 GB-segundos de tiempo de cómputo
└── Perfecto para aplicaciones pequeñas

Amazon DynamoDB:
├── 25 GB de almacenamiento
├── 2.5 millones de solicitudes de lectura
├── 1 millón de solicitudes de escritura
└── Suficiente para aplicaciones pequeñas

Amazon SNS:
├── 1 millón de publicaciones
├── 100,000 entregas HTTP/S
├── 1,000 entregas de email
└── Necesidades básicas de notificación

AWS CloudFormation:
├── 1,000 operaciones de stack por mes
└── Fundamentos de Infraestructura como Código
```

#### **🧪 Ofertas de Prueba**
**Pruebas a corto plazo para servicios específicos**

**Ejemplos:**
```
Amazon Elasticsearch:
├── 750 horas/mes por 1 mes
├── instancia t2.small.elasticsearch
└── Bueno para probar funcionalidad de búsqueda

Amazon Inspector:
├── Prueba gratuita de 90 días
├── Servicio de evaluación de seguridad
└── Evaluar cumplimiento de seguridad

Amazon GuardDuty:
├── Prueba gratuita de 30 días
├── Servicio de detección de amenazas
└── Monitorear actividad maliciosa
```

### 🚨 **Monitoreo y Alertas del Nivel Gratuito**

#### **📊 Seguimiento de Uso**
- **Panel del Nivel Gratuito** - Monitorear uso en todos los servicios
- **Alertas de uso** - Notificaciones por email al 85% de los límites
- **Desglose detallado** - Seguimiento de uso servicio por servicio
- **Datos históricos** - Rastrear patrones de uso a lo largo del tiempo

#### **⚠️ Evitar Cargos Inesperados**
```
Mejores Prácticas:
├── Configurar alertas de facturación en $1, $5, $10
├── Monitorear panel del Nivel Gratuito semanalmente
├── Usar AWS Budgets para monitoreo proactivo
├── Etiquetar recursos para identificación fácil
├── Detener/terminar recursos no usados rápidamente
└── Entender qué NO está cubierto por el Nivel Gratuito
```

### 🎯 **Estrategia de Aprendizaje del Nivel Gratuito**

#### **🌟 Ruta de Aprendizaje Recomendada**
```
Mes 1-2: Servicios Básicos
├── EC2: Lanzar y gestionar servidores virtuales
├── S3: Almacenar y recuperar archivos
├── RDS: Configurar bases de datos administradas
└── VPC: Crear redes aisladas

Mes 3-4: Servicios Avanzados
├── Lambda: Cómputo sin servidor
├── CloudFormation: Infraestructura como Código
├── CloudWatch: Monitoreo y alertas
└── IAM: Gestión de identidad y acceso

Mes 5-6: Integración y Optimización
├── API Gateway: Crear APIs
├── DynamoDB: Base de datos NoSQL
├── SNS/SQS: Servicios de mensajería
└── Técnicas de optimización de costos
```

---

## 📊 Precios Específicos por Servicio

### 🖥️ **Profundización en Precios de Amazon EC2**

#### **🔧 Tipos y Familias de Instancias**
```
Propósito General (M5):
├── m5.large: $0.096/hora (2 vCPU, 8 GB RAM)
├── m5.xlarge: $0.192/hora (4 vCPU, 16 GB RAM)
└── m5.2xlarge: $0.384/hora (8 vCPU, 32 GB RAM)

Optimizado para Cómputo (C5):
├── c5.large: $0.085/hora (2 vCPU, 4 GB RAM)
├── c5.xlarge: $0.17/hora (4 vCPU, 8 GB RAM)
└── c5.2xlarge: $0.34/hora (8 vCPU, 16 GB RAM)

Optimizado para Memoria (R5):
├── r5.large: $0.126/hora (2 vCPU, 16 GB RAM)
├── r5.xlarge: $0.252/hora (4 vCPU, 32 GB RAM)
└── r5.2xlarge: $0.504/hora (8 vCPU, 64 GB RAM)
```

#### **💾 Precios de Almacenamiento**
```
Tipos de Volúmenes EBS:
├── SSD de Propósito General (gp3): $0.08/GB/mes
├── SSD de IOPS Provisionadas (io2): $0.125/GB/mes + $0.065/IOPS
├── HDD Optimizado para Rendimiento (st1): $0.045/GB/mes
└── HDD Frío (sc1): $0.025/GB/mes

Costos Adicionales:
├── Instantáneas EBS: $0.05/GB/mes
├── Transferencia de datos entre AZs: $0.01/GB cada dirección
└── Direcciones IP Elásticas: Gratis si está adjunta, $0.005/hora si no se usa
```

### 💾 **Precios de Amazon S3**

#### **🗂️ Clases de Almacenamiento**
```
S3 Estándar:
├── Primeros 50 TB: $0.023/GB/mes
├── Siguientes 450 TB: $0.022/GB/mes
└── Más de 500 TB: $0.021/GB/mes

S3 Intelligent-Tiering:
├── Monitoreo: $0.0025 por 1,000 objetos
├── Acceso Frecuente: Igual que S3 Estándar
└── Acceso Infrecuente: $0.0125/GB/mes

S3 Glacier:
├── Almacenamiento: $0.004/GB/mes
├── Recuperación: $0.01/GB (estándar)
└── Duración mínima: 90 días

S3 Glacier Deep Archive:
├── Almacenamiento: $0.00099/GB/mes
├── Recuperación: $0.02/GB (estándar)
└── Duración mínima: 180 días
```

#### **🔄 Precios de Solicitudes**
```
Solicitudes S3 Estándar:
├── PUT, COPY, POST, LIST: $0.0005 por 1,000 solicitudes
├── GET, SELECT: $0.0004 por 1,000 solicitudes
└── DELETE: Gratis

Transferencia de Datos:
├── Transferencia de datos ENTRANTE: Gratis
├── Transferencia de datos SALIENTE: $0.09/GB (primer 1 GB gratis)
└── Transferencia a CloudFront: Gratis
```

### 🗄️ **Precios de Amazon RDS**

#### **💻 Precios de Instancias**
```
MySQL db.t3.micro (Nivel Gratuito):
├── vCPU: 2 (expandible)
├── Memoria: 1 GB
└── Costo: Gratis por 750 horas/mes

MySQL db.t3.small:
├── vCPU: 2 (expandible)
├── Memoria: 2 GB
└── Costo: $0.017/hora

MySQL db.m5.large:
├── vCPU: 2
├── Memoria: 8 GB
└── Costo: $0.096/hora
```

#### **💾 Almacenamiento y Características**
```
Opciones de Almacenamiento:
├── SSD de Propósito General: $0.115/GB/mes
├── SSD de IOPS Provisionadas: $0.125/GB/mes + $0.10/IOPS
└── Magnético: $0.10/GB/mes

Características Adicionales:
├── Despliegue Multi-AZ: 2x costo de instancia
├── Réplicas de lectura: Costos de instancia adicionales
├── Respaldos automatizados: Gratis (hasta tamaño de BD)
├── Instantáneas manuales: $0.095/GB/mes
└── Transferencia de datos: Tarifas estándar de AWS
```

---

## 🧮 Estimación de Costos

### 🛠️ **Calculadora de Precios de AWS**

#### **🎯 ¿Qué es la Calculadora de Precios de AWS?**
**Herramienta gratuita para estimar costos de AWS:**
- **Estimaciones específicas por servicio** - Desgloses detallados de costos
- **Múltiples escenarios** - Comparar diferentes arquitecturas
- **Funcionalidad de exportación** - Guardar y compartir estimaciones
- **Actualizaciones regulares** - Siempre actualizada con los últimos precios

#### **📊 Cómo Usar la Calculadora**
```
Proceso Paso a Paso:
├── 1. Seleccionar servicios que planeas usar
├── 2. Configurar cada servicio (tipos de instancia, almacenamiento, etc.)
├── 3. Especificar patrones de uso (horas/mes, transferencia de datos)
├── 4. Elegir modelo de precios (Bajo Demanda, Reservado, etc.)
├── 5. Revisar costos totales mensuales/anuales
└── 6. Exportar estimación para documentación
```

### 💡 **Ejemplos de Estimación de Costos**

#### **🏪 Sitio Web de E-commerce Pequeño**
```
Requisitos de Arquitectura:
├── Servidores web: 2 × instancias t3.medium
├── Base de datos: 1 × instancia RDS db.t3.small
├── Almacenamiento: 100 GB para imágenes de productos
├── CDN: CloudFront para entrega global
└── Balanceador de carga: Application Load Balancer

Estimación de Costo Mensual:
├── Instancias EC2: $60.32 (2 × $30.16)
├── Base de datos RDS: $24.82
├── Almacenamiento S3: $2.30
├── CloudFront: $8.50 (estimado)
├── Balanceador de carga: $22.27
└── Total: ~$118/mes
```

#### **📊 Plataforma de Análisis de Datos**
```
Requisitos de Arquitectura:
├── Procesamiento: 10 × instancias Spot c5.xlarge (8 horas/día)
├── Almacenamiento: 1 TB S3 Estándar, 5 TB S3 Glacier
├── Base de datos: instancia RDS r5.large
├── Red: Transferencia de datos mínima
└── Adicional: Lambda para automatización

Estimación de Costo Mensual:
├── Instancias Spot: $408 (70% descuento aplicado)
├── S3 Estándar: $23
├── S3 Glacier: $20
├── RDS: $90.72
├── Lambda: $5 (estimado)
└── Total: ~$547/mes

Comparación con Bajo Demanda:
├── Instancias Bajo Demanda: $1,360
├── Total con Bajo Demanda: $1,499/mes
└── Ahorros con Spot: $952/mes (63% reducción)
```

### 🎯 **Optimización de Costos Durante la Planificación**

#### **💰 Optimización Pre-Despliegue**
```
Estrategia de Dimensionamiento Correcto:
├── Comenzar con instancias más pequeñas
├── Monitorear rendimiento después del despliegue
├── Escalar hacia arriba solo cuando sea necesario
├── Usar Auto Scaling para cargas de trabajo variables
└── Planificar compras de Instancias Reservadas

Optimización de Almacenamiento:
├── Usar clases de almacenamiento S3 apropiadas
├── Implementar políticas de ciclo de vida
├── Considerar compresión para archivos
├── Usar CloudFront para contenido estático
└── Planificar patrones de transferencia de datos
```

#### **📊 Planificación de Escenarios**
```
Crear Múltiples Estimaciones:
├── Producto mínimo viable (MVP)
├── Escenario de crecimiento esperado
├── Escenario de carga pico
├── Escenario optimizado para costos
└── Escenario de alta disponibilidad

Comparar Opciones:
├── Diferentes tamaños de instancia
├── Reservado vs Bajo Demanda vs Spot
├── Diferentes arquitecturas
├── Diferencias de precios regionales
└── Impactos de planes de soporte
```

---

## 🧠 Ayudas de Memoria

### 💰 **Mnemónico de Modelos de Precios: "ROSS"**
- **R**eservado - Compromiso a largo plazo, grandes ahorros
- **O**n-Demand (Bajo Demanda) - Pagar según uses, máxima flexibilidad
- **S**pot - Ofertar en capacidad de sobra, descuentos enormes
- **S**avings Plans (Planes de Ahorro) - Compromiso flexible, buenos ahorros

### 🎯 **Cuándo Usar Cada Modelo: "SURE"**
- **S**pot - Cargas de trabajo tolerantes a fallos, flexibles
- **U**npredictable (Impredecible) - Bajo Demanda para uso variable
- **R**egular - Reservado para cargas de trabajo estables, predecibles
- **E**verything (Todo) - Planes de Ahorro para cargas de trabajo mixtas

### 🆓 **Memoria del Nivel Gratuito: "12-Siempre-Prueba"**
- **12** meses - La mayoría de servicios gratis el primer año
- **Siempre** - Algunos servicios gratis para siempre
- **Prueba** - Pruebas a corto plazo para servicios especializados

---

## 📝 Preguntas de Práctica

### Pregunta 1
Una empresa tiene una aplicación web con tráfico predecible que funciona 24/7 durante todo el año. Quieren minimizar costos mientras mantienen confiabilidad. ¿Qué modelo de precios proporcionaría los mayores ahorros de costos?

**A)** Instancias Bajo Demanda  
**B)** Instancias Spot  
**C)** Instancias Reservadas  
**D)** Planes de Ahorro  

<details>
<summary>🔍 Clic para Respuesta</summary>

**Respuesta: C) Instancias Reservadas**

**Explicación:** Para cargas de trabajo predecibles y estables que funcionan 24/7, las Instancias Reservadas proporcionan los máximos ahorros (hasta 75%) comparado con precios Bajo Demanda. Las características de la carga de trabajo la hacen perfecta para un compromiso a largo plazo.

</details>

### Pregunta 2
Una startup quiere ejecutar trabajos de procesamiento por lotes que pueden ser interrumpidos y reiniciados sin pérdida de datos. Los trabajos funcionan por varias horas en momentos impredecibles. ¿Qué modelo de precios sería más costo-efectivo?

**A)** Instancias Bajo Demanda  
**B)** Instancias Reservadas  
**C)** Instancias Spot  
**D)** Hosts Dedicados  

<details>
<summary>🔍 Clic para Respuesta</summary>

**Respuesta: C) Instancias Spot**

**Explicación:** Las Instancias Spot son perfectas para cargas de trabajo tolerantes a fallos e interrumpibles como procesamiento por lotes. Pueden proporcionar hasta 90% de ahorros comparado con Bajo Demanda, y dado que los trabajos pueden manejar interrupciones, la startup puede aprovechar los ahorros significativos de costos.

</details>

### Pregunta 3
¿Qué está incluido en el Nivel Gratuito de AWS para Amazon EC2?

**A)** Uso ilimitado de instancias t2.nano  
**B)** 750 horas por mes de instancias t2.micro o t3.micro por 12 meses  
**C)** 1,000 horas por mes de cualquier tipo de instancia por 6 meses  
**D)** Una instancia m5.large funcionando 24/7 por 12 meses  

<details>
<summary>🔍 Clic para Respuesta</summary>

**Respuesta: B) 750 horas por mes de instancias t2.micro o t3.micro por 12 meses**

**Explicación:** El Nivel Gratuito de AWS incluye 750 horas por mes de instancias t2.micro o t3.micro durante los primeros 12 meses después de la creación de la cuenta. Esto es suficiente para ejecutar una instancia pequeña 24/7 durante todo el mes.

</details>

### Pregunta 4
Una empresa tiene cargas de trabajo mixtas incluyendo instancias EC2, funciones Lambda y contenedores Fargate. Quieren comprometerse a cierto nivel de uso para ahorros de costos pero necesitan flexibilidad para cambiar su mezcla de servicios. ¿Qué opción es más apropiada?

**A)** Instancias Reservadas Estándar  
**B)** Instancias Reservadas Convertibles  
**C)** Planes de Ahorro de Cómputo  
**D)** Planes de Ahorro de Instancias EC2  

<details>
<summary>🔍 Clic para Respuesta</summary>

**Respuesta: C) Planes de Ahorro de Cómputo**

**Explicación:** Los Planes de Ahorro de Cómputo proporcionan flexibilidad a través de servicios EC2, Lambda y Fargate mientras ofrecen ahorros significativos (hasta 66%). Permiten cambiar la mezcla de servicios mientras mantienen los beneficios de costo de un compromiso de uso.

</details>

---

## 🎯 Puntos Clave

### 🌟 **El Panorama General**
- **Los precios de AWS son flexibles** - Múltiples modelos para diferentes necesidades
- **Pagar solo por lo que uses** - Sin costos iniciales a menos que los elijas
- **El compromiso trae ahorros** - Compromisos más largos = mayores descuentos
- **El nivel gratuito habilita aprendizaje** - Probar servicios de AWS sin costo

### 🎯 **Para el Examen**
- **Saber cuándo usar cada modelo de precios** - Basado en características de carga de trabajo
- **Entender límites del Nivel Gratuito** - Qué está incluido y por cuánto tiempo
- **Recordar porcentajes de ahorros** - Reservado (hasta 75%), Spot (hasta 90%)
- **Factores de precios** - Tipo de instancia, región, SO, patrones de uso

### 💡 **Para Aplicación del Mundo Real**
- **Comenzar con Bajo Demanda** - Aprender tus patrones de uso primero
- **Usar Nivel Gratuito para aprender** - Experimentar sin preocupaciones de costo
- **Planificar para Instancias Reservadas** - Una vez que entiendas cargas de trabajo estables
- **Considerar Spot para cargas de trabajo apropiadas** - Procesamiento por lotes, desarrollo

### 🚀 **Mejores Prácticas**
- **Monitorear patrones de uso** - Entender antes de comprometerse
- **Mezclar modelos de precios** - Usar el modelo correcto para cada carga de trabajo
- **Usar la calculadora de precios** - Estimar costos antes del despliegue
- **Configurar alertas de facturación** - Evitar cargos sorpresa
- **Revisiones regulares de costos** - Optimizar modelos de precios según cambien las necesidades

---

## 🔗 Navegación

**← Anterior:** [Dominio 4: Facturación y Soporte](./README.md)  
**→ Siguiente:** [Herramientas de Gestión de Facturación y Costos](./cost-management.md)  
**↑ Arriba:** [Dominio 4: Facturación y Soporte](./README.md)  
**🏠 Inicio:** [Guía de Estudio AWS Cloud Practitioner](../README.md)

---

> 💡 **Consejo Pro:** El examen frecuentemente pregunta sobre elegir el modelo de precios correcto para escenarios específicos. Enfócate en entender las características de cada carga de trabajo (predecible vs. impredecible, tolerante a fallos vs. crítica, corto plazo vs. largo plazo) en lugar de memorizar números exactos de precios!
