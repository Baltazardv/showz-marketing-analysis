# Análisis de Marketing Digital - Showz

Proyecto de análisis de datos para optimización de gastos de marketing en una plataforma de venta de entradas de eventos.

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-2.0+-green.svg)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)

---

## 📊 Descripción del Proyecto

Análisis completo de 19 meses de datos (junio 2017 - diciembre 2018) para una plataforma de venta de entradas de eventos, abarcando 359,400 visitas, 50,415 pedidos y datos de inversión en múltiples canales de marketing.

**Objetivo:** Optimizar gastos de marketing identificando canales rentables, calculando métricas clave de negocio (CAC, LTV, ROMI) y proponiendo estrategias accionables de retención de clientes.

---

## 🎯 Hallazgos Principales

- **Tasa de conversión global:** 4.47% - Oportunidad de mejora en el funnel de compra
- **Retención de clientes:** Solo 18.2% realiza más de una compra (principal área de oportunidad)
- **Marketing ineficiente:** Identificados canales con ROMI negativo consumiendo presupuesto significativo
- **Gap entre dispositivos:** Diferencia notable en conversión entre dispositivos sugiere problemas de UX
- **Conversión inmediata:** 67.3% de compradores convierten el mismo día de la visita
- **Tiempo promedio hasta conversión:** 7.8 días para quienes no compran inmediatamente

---

## 🛠️ Tecnologías Utilizadas

- **Python 3.9+** - Lenguaje principal
- **Pandas** - Manipulación y análisis de datos
- **NumPy** - Operaciones numéricas y cálculos
- **Matplotlib & Seaborn** - Visualización de datos
- **Jupyter Notebook** - Desarrollo interactivo y documentación

---

## 📈 Métricas Analizadas

### Métricas de Adquisición
- **CAC (Customer Acquisition Cost)** - Costo de adquisición por canal de marketing
- **Tasa de conversión** - Por canal, dispositivo y cohorte temporal
- **Análisis de cohortes** - Tiempo desde primera visita hasta conversión

### Métricas de Valor
- **LTV (Lifetime Value)** - Valor de vida del cliente
- **AOV (Average Order Value)** - Valor promedio de pedido
- **Análisis de segmentación** - Clientes por valor (bajo, medio, alto, VIP)

### Métricas de Marketing
- **ROMI (Return on Marketing Investment)** - Retorno de inversión por canal
- **Eficiencia de gasto** - Distribución de presupuesto vs resultados
- **Performance temporal** - Evolución de métricas mes a mes

### Métricas de Retención
- **Tasa de retención** - Usuarios que regresan al sitio
- **Compras repetidas** - Clientes con más de un pedido
- **Frecuencia de compra** - Análisis de comportamiento de compra

---

## 📁 Estructura del Proyecto

showz-marketing-analysis/
│
├── README.md                          # Este archivo
├── .gitignore                         # Archivos a ignorar en Git
├── requirements.txt                   # Dependencias del proyecto
│
├── notebooks/
│   ├── 02_marketing_analysis.ipynb   # Análisis completo (principal)
│   └── 03_conclusions.md             # Conclusiones personales
│
├── data/
│   ├── raw/                          # Datos originales
│   │   ├── visits_log_us.csv         # Logs de visitas (359.4K registros)
│   │   ├── orders_log_us.csv         # Pedidos (50.4K registros)
│   │   └── costs_us.csv              # Costos marketing (2.5K registros)
│   └── README.md                     # Descripción de datos
│
└── reports/
└── figures/                      # Gráficos exportados
├── user_behavior.png
├── conversion_analysis.png
└── romi_analysis.png

📊 Análisis Realizados
1. Análisis de Comportamiento de Usuarios

Usuarios únicos por día, semana y mes
Patrones de sesiones y duración promedio
Frecuencia de retorno de usuarios
Actividad por día de la semana y hora del día

2. Análisis de Conversión

Tiempo hasta primera compra (análisis de cohortes)
Categorización de conversiones: 0d, 1d, 1-7d, 8-30d, 30d+
Tasa de conversión por canal de marketing
Análisis de funnel de conversión

3. Análisis de Ventas

Distribución de valor de pedidos
LTV por segmento de cliente
Pedidos por usuario y frecuencia de compra
Análisis temporal de ingresos

4. Análisis de Marketing

CAC por canal de adquisición
ROMI por fuente de tráfico
Evolución temporal de gastos
Identificación de canales rentables vs no rentables

5. Análisis por Dispositivo

Performance de conversión por tipo de dispositivo
Diferencias en comportamiento y valor
Oportunidades de optimización específicas


## 💡 Recomendaciones Principales
Prioridad Alta (Implementar inmediatamente)

Pausar canales no rentables - Reasignar presupuesto de fuentes con ROMI < 0
Optimizar experiencia en dispositivo específico - Cerrar gap de conversión entre dispositivos
Implementar remarketing básico - 95.5% de usuarios no convierte en primera visita

Prioridad Media (1-3 meses)

Estrategia de retención - Email marketing post-compra y programa de fidelidad
Escalar canales rentables - Aumentar inversión gradual en top 3 canales
A/B testing en checkout - Reducir fricción en proceso de compra

Métricas de Éxito Esperadas (90 días)

ROMI global: >2.0x (actual: 1.15x)
Tasa de conversión: +15-20%
Retención de clientes: >25% (actual: 18.2%)
CAC promedio: -20%


## 📚 Aprendizajes Técnicos
Skills de Data Analysis

Limpieza y validación de datos reales con inconsistencias
Cálculo e interpretación de métricas de marketing (CAC, LTV, ROMI)
Análisis de cohortes para entender comportamiento temporal
Segmentación de clientes por valor y comportamiento

Skills de Visualización

Creación de dashboards informativos con matplotlib/seaborn
Visualización de funnels de conversión
Gráficos de evolución temporal y tendencias
Matrices de decisión para estrategia de marketing

Skills de Business Intelligence

Traducción de hallazgos técnicos a recomendaciones de negocio
Priorización de acciones basada en impacto potencial
Comunicación efectiva de insights a stakeholders no técnicos
Establecimiento de KPIs y métricas de seguimiento


## 🔍 Limitaciones y Trabajo Futuro
Limitaciones del Análisis Actual

No incluye datos de márgenes de ganancia por producto
Falta información cualitativa sobre por qué usuarios no regresan
Sin datos de competencia para benchmarking
No considera estacionalidad de eventos específicos

Análisis Futuros Sugeridos

Segmentación RFM (Recency, Frequency, Monetary) más profunda
Análisis predictivo de churn de clientes
Modelos de propensión a compra para remarketing
Análisis de valor de vida del cliente por cohorte de adquisición
