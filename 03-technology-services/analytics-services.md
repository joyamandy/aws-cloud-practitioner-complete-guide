# 📊 Servicios de Analítica

> **Convierte Datos en Insights | Tiempo de Estudio: ~2 horas**

Piensa en los servicios de analítica como **diferentes tipos de detectives de datos**:
- **Amazon Athena** es como un **detective con visión de rayos X** - ve patrones en los datos sin moverlos
- **Amazon Kinesis** es como un **reportero de noticias en vivo** - captura y analiza eventos mientras suceden
- **Amazon QuickSight** es como un **maestro narrador** - convierte datos complejos en historias visuales claras
- **AWS Glue** es como un **organizador de datos** - prepara y cataloga datos para análisis
- **Amazon EMR** es como un **equipo de investigación poderoso** - maneja tareas masivas de procesamiento de datos

¡Exploremos cómo AWS te ayuda a desbloquear el valor oculto en tus datos! 🔍

---

## 📋 Tabla de Contenidos

- [🎯 Objetivos de Aprendizaje](#-objetivos-de-aprendizaje)
- [💡 Fundamentos de Analítica](#-fundamentos-de-analítica)
- [🔍 Amazon Athena](#-amazon-athena)
- [📡 Amazon Kinesis](#-amazon-kinesis)
- [📊 Amazon QuickSight](#-amazon-quicksight)
- [🔧 AWS Glue](#-aws-glue)
- [⚡ Amazon EMR](#-amazon-emr)
- [🗄️ Amazon Redshift](#-amazon-redshift)
- [🔎 Amazon OpenSearch](#-amazon-opensearch)
- [🎮 Escenarios del Mundo Real](#-escenarios-del-mundo-real)
- [📝 Preguntas de Práctica](#-preguntas-de-práctica)

---

## 🎯 Objetivos de Aprendizaje

Al final de este capítulo, podrás:

✅ **Entender diferentes tipos de servicios de analítica** y sus casos de uso  
✅ **Identificar el servicio de analítica correcto** para escenarios específicos  
✅ **Reconocer patrones de procesamiento en tiempo real vs por lotes**  
✅ **Entender capacidades de visualización de datos** con QuickSight  
✅ **Saber cuándo usar soluciones de analítica serverless vs gestionadas**  

---

## 💡 Fundamentos de Analítica

### 🎯 **Categorías de Servicios de Analítica**

#### **🔍 Servicios de Consulta**
- **Amazon Athena** - Consultas SQL serverless en datos de S3
- **Amazon Redshift** - Data warehouse para inteligencia de negocios

#### **📡 Analítica de Streaming**
- **Amazon Kinesis** - Streaming y procesamiento de datos en tiempo real
- **Amazon OpenSearch** - Búsqueda y analítica en tiempo real

#### **🔧 Procesamiento de Datos**
- **AWS Glue** - Servicio ETL (Extraer, Transformar, Cargar)
- **Amazon EMR** - Procesamiento de big data con Hadoop/Spark

#### **📊 Visualización**
- **Amazon QuickSight** - Inteligencia de negocios y dashboards

### 🎯 **Cuándo Elegir Qué**

#### **✅ Elige Analítica en Tiempo Real Cuando:**
- **Insights inmediatos** son críticos para decisiones de negocio
- **Detección de fraude** o **detección de anomalías** es necesaria
- **Dashboards en vivo** y **monitoreo** son requeridos
- **Experiencia del cliente** depende de respuestas instantáneas

#### **✅ Elige Analítica por Lotes Cuando:**
- **Análisis histórico** e **identificación de tendencias** es el objetivo
- **Procesamiento complejo** requiere tiempo significativo de cómputo
- **Optimización de costos** es más importante que la velocidad
- **Reportes regulatorios** con requisitos de tiempo específicos

---

## 🔍 Amazon Athena

### ⚡ **¿Qué es Amazon Athena?**

Piensa en Athena como **tener visión de rayos X para tus datos**:
- **Consultar datos directamente en S3** - No necesitas mover o cargar datos
- **SQL estándar** - Usa comandos SQL familiares
- **Pago por consulta** - Solo pagas por las consultas que ejecutas
- **Serverless** - No hay infraestructura que gestionar

### 🎯 **Características Clave de Athena**

#### **💰 Serverless y Costo-Efectivo**
- **No hay servidores que aprovisionar** - Servicio completamente gestionado
- **Pago por TB escaneado** - Solo pagas por datos procesados
- **Escalado automático** - Maneja consultas concurrentes
- **Sin costos iniciales** - Sin tarifas mínimas

#### **🔧 Fácil de Usar**
- **SQL estándar** - Compatible con ANSI SQL
- **Drivers JDBC/ODBC** - Conecta con herramientas de BI
- **Interfaz de AWS Console** - Editor de consultas basado en web
- **Integración API** - Acceso programático

### 🎯 **Casos de Uso de Athena**

#### **📊 Análisis de Datos Ad-hoc**
**Insights rápidos sin configuración compleja**

**Ejemplo:**
```sql
-- Analizar patrones de tráfico del sitio web
SELECT 
    date_format(request_time, '%Y-%m-%d') as day,
    COUNT(*) as page_views,
    COUNT(DISTINCT user_id) as unique_users
FROM web_logs 
WHERE request_time >= date('2024-01-01')
GROUP BY date_format(request_time, '%Y-%m-%d')
ORDER BY day;
```

#### **📈 Inteligencia de Negocios**
- **Reportes de ventas** - Analizar datos de transacciones
- **Analítica de clientes** - Entender comportamiento de usuarios
- **Análisis de costos** - Rastrear patrones de gasto
- **Métricas de rendimiento** - Monitorear KPIs

#### **🔍 Análisis de Logs**
- **Logs de aplicaciones** - Depurar y monitorear aplicaciones
- **Logs de seguridad** - Analizar patrones de acceso
- **Logs de servicios AWS** - CloudTrail, VPC Flow Logs
- **Logs de servidor web** - Análisis de rendimiento del sitio web

---

## 📡 Amazon Kinesis

### 🚀 **¿Qué es Amazon Kinesis?**

Piensa en Kinesis como **una red de noticias en vivo para tus datos**:
- **Streaming de datos en tiempo real** - Captura datos mientras suceden
- **Múltiples fuentes de datos** - IoT, aplicaciones, logs
- **Escalado automático** - Maneja cualquier volumen de datos
- **Procesamiento inmediato** - Analiza datos en tiempo real

### 🎯 **Servicios de Kinesis**

#### **📡 Kinesis Data Streams**
**Plataforma de streaming de datos en tiempo real**

**Características Clave:**
- **Ingesta en tiempo real** - Captura datos con latencia de sub-segundo
- **Múltiples consumidores** - Muchas aplicaciones pueden leer el mismo stream
- **Retención** - Almacena datos por 1-365 días
- **Capacidad de replay** - Procesa datos históricos

**Casos de Uso:**
- Recolección de datos de sensores IoT
- Streaming de logs de aplicaciones
- Procesamiento de feeds de redes sociales
- Monitoreo de transacciones financieras

#### **🔥 Kinesis Data Firehose**
**Carga datos de streaming en almacenes de datos**

**Características Clave:**
- **Completamente gestionado** - No requiere administración
- **Casi tiempo real** - Entrega dentro de 60 segundos
- **Transformaciones integradas** - Formatea y comprime datos
- **Múltiples destinos** - S3, Redshift, OpenSearch, Splunk

**Casos de Uso:**
- Ingesta de data lake
- Carga de data warehouse
- Agregación de logs
- Preparación de analítica

#### **⚡ Kinesis Analytics**
**Analítica en tiempo real sobre datos de streaming**

**Características Clave:**
- **SQL sobre datos de streaming** - Usa sintaxis SQL familiar
- **Machine learning** - Algoritmos ML integrados
- **Funciones de ventana** - Agregaciones basadas en tiempo
- **Insights en tiempo real** - Procesa datos mientras llegan

**Casos de Uso:**
- Dashboards en tiempo real
- Detección de fraude
- Tablas de clasificación en vivo
- Monitoreo y alertas

### 🎯 **Ejemplo de Arquitectura Kinesis**

#### **Pipeline de Analítica IoT**
```
Sensores IoT → Kinesis Data Streams → Kinesis Analytics → Dashboard
              ↓
          Kinesis Firehose → S3 → Athena → QuickSight
```

**Beneficios:**
- **Monitoreo en tiempo real** de dispositivos IoT
- **Análisis histórico** de datos de sensores
- **Alertas automatizadas** para anomalías
- **Almacenamiento costo-efectivo** en S3

---

## 📊 Amazon QuickSight

### 📈 **¿Qué es Amazon QuickSight?**

Piensa en QuickSight como **un maestro narrador para tus datos**:
- **Dashboards interactivos** - Crea visualizaciones atractivas
- **Insights de machine learning** - Detección automática de anomalías
- **Serverless** - No hay infraestructura que gestionar
- **Rendimiento rápido** - Motor de cálculo en memoria (SPICE)

### 🎯 **Características Clave de QuickSight**

#### **📊 Capacidades de Visualización**
- **Gráficos y diagramas** - Barras, líneas, pastel, gráficos de dispersión
- **Mapas** - Visualizaciones geoespaciales
- **Tablas dinámicas** - Exploración interactiva de datos
- **Cálculos personalizados** - Métricas derivadas y KPIs

#### **🤖 Características de Machine Learning**
- **Detección de anomalías** - Encuentra automáticamente valores atípicos
- **Pronósticos** - Predice tendencias futuras
- **Consultas en lenguaje natural** - Haz preguntas en inglés simple
- **Insights inteligentes** - Recomendaciones impulsadas por ML

#### **🔐 Características Empresariales**
- **Seguridad a nivel de fila** - Controla acceso a datos por usuario
- **Integración con Active Directory** - Autenticación empresarial
- **Analítica embebida** - Integra en aplicaciones
- **Precios por sesión** - Costo-efectivo para bases de usuarios grandes

### 🎯 **Casos de Uso de QuickSight**

#### **📈 Dashboards Ejecutivos**
**Métricas de negocio de alto nivel para liderazgo**

**Visualizaciones Comunes:**
- Tendencias de ingresos y pronósticos
- Métricas de adquisición de clientes
- KPIs operacionales
- Mapas de rendimiento geográfico

#### **📊 Analítica de Autoservicio**
**Permite a usuarios de negocio explorar datos independientemente**

**Beneficios:**
- **Carga reducida de TI** - Los usuarios crean sus propios reportes
- **Insights más rápidos** - No esperar por reportes de TI
- **Exploración interactiva** - Profundizar en detalles
- **Acceso móvil** - Ver dashboards en cualquier lugar

---

## 🔧 AWS Glue

### 🛠️ **¿Qué es AWS Glue?**

Piensa en Glue como **un asistente de preparación de datos**:
- **Extraer, Transformar, Cargar (ETL)** - Prepara datos para análisis
- **Catálogo de datos** - Descubre y cataloga datos automáticamente
- **Serverless** - Sin gestión de infraestructura
- **Descubrimiento de esquemas** - Entiende automáticamente la estructura de datos

### 🎯 **Componentes de Glue**

#### **📚 Catálogo de Datos de Glue**
**Repositorio centralizado de metadatos**

**Características:**
- **Descubrimiento automático** - Los crawlers encuentran y catalogan datos
- **Evolución de esquemas** - Rastrea cambios en estructura de datos
- **Integración** - Funciona con Athena, EMR, Redshift
- **Permisos** - Control de acceso granular

#### **🔄 Trabajos ETL de Glue**
**Transformación de datos serverless**

**Capacidades:**
- **ETL visual** - Interfaz de arrastrar y soltar
- **Generación de código** - Auto-genera código Python/Scala
- **Transformaciones integradas** - Operaciones comunes de datos
- **Código personalizado** - Escribe tus propias transformaciones

### 🎯 **Casos de Uso de Glue**

#### **🏗️ Preparación de Data Lake**
**Prepara datos en bruto para analítica**

**Proceso:**
1. **Rastrear fuentes de datos** - Descubrir datos en S3, bases de datos
2. **Crear catálogo de datos** - Metadatos para todos los datasets
3. **Transformar datos** - Limpiar, formatear y enriquecer
4. **Almacenar en data lake** - Datos organizados, listos para análisis

#### **📊 Carga de Data Warehouse**
**Pipeline ETL para Redshift**

**Flujo de Trabajo:**
```
Sistemas Fuente → Glue ETL → S3 → Redshift → QuickSight
               ↓
           Catálogo de Datos (Metadatos)
```

---

## ⚡ Amazon EMR

### 🚀 **¿Qué es Amazon EMR?**

Piensa en EMR como **un equipo de investigación poderoso para big data**:
- **Elastic MapReduce** - Framework de big data gestionado
- **Múltiples frameworks** - Hadoop, Spark, HBase, Presto
- **Clusters escalables** - Maneja petabytes de datos
- **Costo-efectivo** - Usa Spot Instances para ahorros significativos

### 🎯 **Características Clave de EMR**

#### **🔧 Frameworks Soportados**
- **Apache Hadoop** - Almacenamiento y procesamiento distribuido
- **Apache Spark** - Procesamiento rápido en memoria
- **Apache HBase** - Base de datos NoSQL para big data
- **Presto** - Consultas SQL interactivas
- **Apache Hive** - Software de data warehouse
- **Apache Pig** - Plataforma para analizar grandes datasets

#### **💰 Optimización de Costos**
- **Spot Instances** - Hasta 90% de ahorro en costos
- **Auto Scaling** - Ajusta tamaño de cluster basado en carga de trabajo
- **Reserved Instances** - Descuentos para cargas de trabajo predecibles
- **Flotas de instancias** - Mezcla de tipos de instancia para optimización

### 🎯 **Casos de Uso de EMR**

#### **📊 Procesamiento de Big Data**
**Procesa grandes datasets que no caben en máquinas individuales**

**Ejemplos:**
- **Análisis de logs** - Procesa terabytes de logs web
- **Modelado financiero** - Análisis de riesgo en grandes datasets
- **Investigación científica** - Genómica, modelado climático
- **Machine learning** - Entrena modelos en grandes datasets

#### **🔄 ETL a Escala**
**Transforma cantidades masivas de datos**

**Flujo de Trabajo:**
```
Datos en Bruto (S3) → Cluster EMR → Datos Procesados (S3/Redshift)
                         ↓
                  Herramientas de Analítica (Athena, QuickSight)
```

---

## 🗄️ Amazon Redshift

### 🏢 **¿Qué es Amazon Redshift?**

Piensa en Redshift como **un data warehouse de alto rendimiento**:
- **Almacenamiento columnar** - Optimizado para consultas analíticas
- **Procesamiento masivamente paralelo** - Distribuye consultas entre nodos
- **Escala de petabytes** - Maneja datasets muy grandes
- **SQL estándar** - Usa herramientas de base de datos familiares

### 🎯 **Características Clave de Redshift**

#### **⚡ Rendimiento**
- **Almacenamiento columnar** - 10x más rápido que bases de datos tradicionales
- **Cache de resultados** - Cachea resultados de consultas frecuentes
- **Vistas materializadas** - Resultados de consultas pre-computados
- **Gestión automática de carga de trabajo** - Optimiza asignación de recursos

#### **📈 Escalabilidad**
- **Empezar pequeño** - Clusters de un solo nodo para desarrollo
- **Escalar hacia afuera** - Agregar nodos mientras los datos crecen
- **Redimensionar clusters** - Cambiar tamaño de cluster sin tiempo de inactividad
- **Escalado de concurrencia** - Maneja cargas de consultas en ráfagas

### 🎯 **Casos de Uso de Redshift**

#### **📊 Inteligencia de Negocios**
**Impulsa reportes empresariales y analítica**

**Escenarios Comunes:**
- **Reportes financieros** - Análisis de ingresos, ganancias, costos
- **Analítica de ventas** - Seguimiento de rendimiento, pronósticos
- **Analítica de clientes** - Análisis de comportamiento, segmentación
- **Reportes operacionales** - Dashboards de KPI, monitoreo

#### **📈 Data Warehousing**
**Repositorio central para datos organizacionales**

**Arquitectura:**
```
Sistemas Fuente → Proceso ETL → Redshift → Herramientas BI
      ↓               ↓              ↓            ↓
 Sistemas        Transformar   Data Warehouse   Reportes
Transaccionales   y Cargar       (OLAP)       Dashboards
```

---

## 🔎 Amazon OpenSearch

### 🔍 **¿Qué es Amazon OpenSearch?**

Piensa en OpenSearch como **un motor de búsqueda para tus datos**:
- **Búsqueda de texto completo** - Encuentra información en grandes datasets de texto
- **Analítica en tiempo real** - Analiza datos de streaming
- **Analítica de logs** - Monitorea logs de aplicaciones y sistemas
- **Visualización** - Dashboards Kibana integrados

### 🎯 **Características Clave de OpenSearch**

#### **🔍 Capacidades de Búsqueda**
- **Búsqueda de texto completo** - Busca a través de documentos y logs
- **Consultas complejas** - Coincidencias booleanas, comodín, difusas
- **Agregaciones** - Análisis estadístico de resultados de búsqueda
- **Auto-completado** - Sugerencias y completado de búsqueda

#### **📊 Características de Analítica**
- **Analítica en tiempo real** - Procesa datos de streaming
- **Análisis de series temporales** - Analiza datos a lo largo del tiempo
- **Consultas geoespaciales** - Analítica basada en ubicación
- **Machine learning** - Detección de anomalías y pronósticos

### 🎯 **Casos de Uso de OpenSearch**

#### **📋 Analítica de Logs**
**Monitorea y analiza logs de aplicaciones**

**Arquitectura de Ejemplo:**
```
Aplicaciones → Kinesis Firehose → OpenSearch → Dashboards Kibana
                ↓
            Indexación en Tiempo Real → Búsqueda y Analítica
```

#### **🔍 Búsqueda de Aplicaciones**
**Agrega funcionalidad de búsqueda a aplicaciones**

**Casos de Uso:**
- **E-commerce** - Búsqueda de productos y recomendaciones
- **Plataformas de contenido** - Búsqueda de artículos y documentos
- **Sistemas de soporte** - Búsqueda en base de conocimientos
- **Búsqueda empresarial** - Descubrimiento de documentos internos

---

## 🎮 Escenarios del Mundo Real

### 🏪 **Escenario 1: Plataforma de Analítica E-commerce**

**Requisitos:**
- **Monitoreo en tiempo real** de ventas y comportamiento de usuarios
- **Análisis histórico** para identificación de tendencias
- **Dashboards interactivos** para diferentes equipos de negocio
- **Solución costo-efectiva** que escale con el negocio

**Arquitectura de Analítica:**
```
Acciones de Cliente → Kinesis Data Streams → Kinesis Analytics → Alertas en Tiempo Real
                                ↓
                      Kinesis Firehose → S3 Data Lake
                                            ↓
                                 Glue ETL → Redshift → Dashboards QuickSight
                                     ↓
                               Athena (Consultas Ad-hoc)
```

**Beneficios:**
- **Detección de fraude en tiempo real** con Kinesis Analytics
- **Análisis de tendencias históricas** con Redshift y QuickSight
- **Optimización de costos** con almacenamiento de data lake S3
- **Analítica de autoservicio** para equipos de negocio

### 📱 **Escenario 2: Procesamiento de Datos IoT**

**Situación:**
- Ciudad inteligente con miles de sensores
- Necesidad de monitoreo en tiempo real y análisis histórico
- Múltiples consumidores de datos con diferentes requisitos
- Restricciones presupuestarias que requieren optimización de costos

**Arquitectura de Solución:**
```
Sensores IoT → Kinesis Data Streams → Múltiples Consumidores:
                       ↓                    ├── Kinesis Analytics (Tiempo Real)
                       ↓                    ├── Lambda (Triggers/Alertas)
                       ↓                    └── EMR (Procesamiento por Lotes)
                       ↓
               Kinesis Firehose → S3 → Athena (Análisis Ad-hoc)
                                   ↓
                             Glue → Catálogo de Datos → QuickSight
```

**Resultados:**
- **Monitoreo en tiempo real** de infraestructura de la ciudad
- **Mantenimiento predictivo** usando machine learning de EMR
- **Ahorro de costos** del 60% usando servicios serverless
- **Escalable** a millones de sensores

### 🏥 **Escenario 3: Analítica de Salud**

**Requisitos:**
- **Cumplimiento HIPAA** para datos de pacientes
- **Monitoreo en tiempo real** de signos vitales de pacientes
- **Analítica de investigación** en datos anonimizados
- **Integración** con sistemas hospitalarios existentes

**Arquitectura Conforme:**
```
Dispositivos Médicos → Kinesis (Cifrado) → Lambda (Procesamiento HIPAA)
                                               ↓
                                   S3 (Cifrado) → Glue ETL
                                                      ↓
                                Redshift (VPC) → QuickSight (Asegurado)
```

**Características de Cumplimiento:**
- **Cifrado de extremo a extremo** para todos los datos
- **Despliegue VPC** para aislamiento de red
- **Políticas IAM** para control de acceso granular
- **Registro de auditoría** con CloudTrail

---

## 📝 Preguntas de Práctica

### Pregunta 1
Una empresa quiere analizar sus logs de servidor web almacenados en S3 usando consultas SQL sin gestionar infraestructura. ¿Qué servicio deberían usar?

**A)** Amazon EMR  
**B)** Amazon Athena  
**C)** Amazon Redshift  
**D)** AWS Glue  

<details>
<summary>🔍 Haz clic para ver la Respuesta</summary>

**Respuesta: B) Amazon Athena**

**Explicación:** Athena es un servicio de consultas serverless que te permite analizar datos en S3 usando SQL estándar sin gestionar infraestructura. Es perfecto para análisis ad-hoc de archivos de log.

</details>

---

### Pregunta 2
Una aplicación IoT necesita procesar millones de lecturas de sensores en tiempo real y activar alertas inmediatas para anomalías. ¿Qué combinación de servicios es más apropiada?

**A)** S3 + Athena + QuickSight  
**B)** Kinesis Data Streams + Kinesis Analytics + Lambda  
**C)** EMR + Redshift + QuickSight  
**D)** Glue + S3 + Athena  

<details>
<summary>🔍 Haz clic para ver la Respuesta</summary>

**Respuesta: B) Kinesis Data Streams + Kinesis Analytics + Lambda**

**Explicación:** Esta combinación proporciona ingesta de datos en tiempo real (Kinesis Data Streams), analítica en tiempo real (Kinesis Analytics), y capacidades de respuesta inmediata (Lambda) para detección de anomalías IoT.

</details>

---

### Pregunta 3
Un analista de negocios quiere crear dashboards interactivos con insights impulsados por machine learning sin escribir código. ¿Qué servicio es más adecuado para este requisito?

**A)** Amazon Athena  
**B)** Amazon QuickSight  
**C)** Amazon EMR  
**D)** AWS Glue  

<details>
<summary>🔍 Haz clic para ver la Respuesta</summary>

**Respuesta: B) Amazon QuickSight**

**Explicación:** QuickSight es un servicio de inteligencia de negocios que proporciona dashboards interactivos con características de machine learning integradas como detección de anomalías y pronósticos, sin requerir código.

</details>

---

## 🧠 Ayudas de Memoria

### 🎯 **Selección de Servicios de Analítica: "ARKEG"**
- **A**thena - Consultas SQL ad-hoc en datos de S3
- **R**edshift - Data warehouse para inteligencia de negocios  
- **K**inesis - Procesamiento de datos de streaming en tiempo real
- **E**MR - Procesamiento de big data con Hadoop/Spark
- **G**lue - Servicio ETL para preparación de datos

### 🔄 **Procesamiento en Tiempo Real vs por Lotes**

| **Requisito** | **Tiempo Real** | **Por Lotes** |
|---|---|---|
| **Latencia** | Milisegundos-segundos | Minutos-horas |
| **Caso de Uso** | Detección de fraude, monitoreo | Reportes, analítica |
| **Servicio AWS** | Kinesis Analytics | EMR, Glue |
| **Costo** | Mayor por registro | Menor por registro |

### 📊 **Guías de Volumen de Datos**
- **Datasets pequeños** (< 1TB) → Athena
- **Datasets medianos** (1-100TB) → Redshift
- **Datasets grandes** (> 100TB) → EMR + S3
- **Datos de streaming** → Kinesis

---

## ✅ Puntos Clave

### 🎯 **Puntos Esenciales para el Examen AWS**

1. **Athena** = Consultas SQL serverless en datos de S3
2. **Kinesis** = Procesamiento de datos de streaming en tiempo real
3. **QuickSight** = Inteligencia de negocios y visualización
4. **Glue** = Servicio ETL serverless
5. **EMR** = Hadoop/Spark gestionado para big data
6. **Redshift** = Data warehouse para analítica
7. **OpenSearch** = Búsqueda y analítica de logs

### 📈 **Combinaciones de Servicios**
- **Data Lake**: S3 + Glue + Athena + QuickSight
- **Analítica en Tiempo Real**: Kinesis + Lambda + OpenSearch
- **Data Warehouse**: Glue + Redshift + QuickSight
- **Procesamiento de Big Data**: EMR + S3 + Athena

### 💰 **Consejos de Optimización de Costos**
- Usa **Athena** para consultas infrecuentes
- Usa **Redshift Spectrum** para cargas de trabajo mixtas
- Usa **Spot Instances** con EMR
- Usa **S3 Intelligent Tiering** para data lakes

---

## 📝 Lista de Verificación del Capítulo

{{ ... }}
## 🔗 Navegación

**Anterior:** [💻 Servicios de Cómputo](./compute-services.md)  
**Siguiente:** [📶 Servicios de Redes](./networking-services.md)  
**Inicio:** [🏠 Guía AWS Cloud Practitioner](../README.md)

---

> 💡 **Consejo Pro:** Las preguntas de analítica a menudo involucran elegir entre procesamiento en tiempo real y por lotes. Busca palabras clave como "inmediato," "tiempo real," o "streaming" para identificar escenarios en tiempo real, versus "histórico," "reportes," o "periódico" para escenarios por lotes!
