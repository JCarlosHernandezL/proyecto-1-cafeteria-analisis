# 🍽️ Cafetería La Corriente — Auditoría Operacional Mayo 2025
### *Cafeteria Operations Audit — May 2025*

> **Proyecto #1 de Portafolio | Portfolio Project #1**  
> Programa: Data Analyst con IA | Program: Data Analyst with AI  
> Herramientas: Excel · Python · Análisis Estadístico | Tools: Excel · Python · Statistical Analysis

---

## 📋 Descripción del Proyecto | Project Description

**ES:** Auditoría completa de operaciones de una cafetería corporativa ubicada cerca de oficinas de gobierno. El análisis cubre un mes completo de operación (Mayo 2025) con 3,426 transacciones de venta, e incluye análisis financiero, comportamiento de clientes, optimización de personal y recomendaciones estratégicas ejecutables.

**EN:** Full operations audit of a corporate cafeteria located near government offices. The analysis covers one complete month of operation (May 2025) with 3,426 sales transactions, including financial analysis, customer behavior, staff optimization, and actionable strategic recommendations.

---

## 🎯 Preguntas de Negocio | Business Questions

| # | Pregunta ES | Question EN |
|---|---|---|
| 1 | ¿Cuánto necesita vender la cafetería cada día para no perder dinero? | What is the daily break-even point? |
| 2 | ¿Qué 20% de productos genera el 80% del ingreso? | Which 20% of products drive 80% of revenue? |
| 3 | ¿Los clientes gastan más en quincena o fuera de ella? | Do customers spend more during or outside payday? |
| 4 | ¿Cuál es la hora más rentable del día — no solo la más concurrida? | What is the most profitable hour — not just the busiest? |
| 5 | ¿Qué categoría deja más pesos en la caja al final del mes? | Which category generates the most margin pesos at month end? |
| 6 | ¿En qué horas conviene reducir personal sin sacrificar ingreso? | When can staff be reduced without sacrificing revenue? |

---

## 📊 Dataset

| Atributo | Detalle |
|---|---|
| **Fuente** | Dataset simulado con lógica de negocio real |
| **Source** | Simulated dataset with real business logic |
| **Período** | Mayo 2025 (22 días hábiles) |
| **Registros** | 3,426 líneas de venta / 1,897 transacciones |
| **Productos** | 75 productos en 8 categorías |
| **Variables** | Fecha, hora, día, quincena, producto, categoría, precio, costo, margen, método de pago, cliente |

**Supuestos documentados:**
- Costo variable estimado = 35% del precio de venta
- Cafetería opera Lunes–Viernes, 7am–6pm
- Sueldos sin IMSS (figura de asociados operativos)
- Lógica de quincena: días 15–16 y 30–31 con +25% de demanda; días 13–14 y 28–29 con –20%

---

## 🔍 Metodología | Methodology

```
ASK → PREPARE → PROCESS → ANALYZE → SHARE → ACT
```
*(Google Data Analytics Framework)*

1. **ASK** — Definición de preguntas de negocio con criterios SMART
2. **PREPARE** — Generación y documentación del dataset con supuestos explícitos
3. **PROCESS** — Limpieza, estructuración y enriquecimiento de datos en Python
4. **ANALYZE** — 6 análisis independientes con hallazgos y recomendaciones
5. **SHARE** — Reporte ejecutivo bilingüe en Excel (una página por idioma)
6. **ACT** — Plan de acción con impacto financiero proyectado

---

## 💡 Hallazgos Principales | Key Findings

### 1️⃣ Punto de Equilibrio | Break-Even
- PE diario: **$3,434 MXN**
- 7 de 22 días operativos estuvieron por debajo del PE
- El **miércoles** es el día más débil de forma consistente
- **Acción:** Promoción fija de miércoles con combo al 9% de descuento

### 2️⃣ Pareto del Menú | Menu Pareto
- **39 productos** (52% del menú) generan el 80% del ingreso
- **16 productos** están en la "cola" — candidatos a eliminación
- El **44.2% de tickets** son de un solo ítem → oportunidad de combos
- Market Basket Analysis: top combo → Torta de Guisado + Salchipapas

### 3️⃣ Ciclo de Quincena | Pay Cycle
- Q1 y Q2 casi idénticas en ingreso total ($45,929 vs $45,720)
- Días de cobro generan **$5,300/día** vs $3,100 en días pre-quincena
- Postres y Bebidas sube **+12% en Q2** cuando hay más liquidez
- **Acción:** Menú económico en días 13–14 y 28–29

### 4️⃣ Hora más Rentable | Most Profitable Hour
- **13hrs** es el pico de tráfico (29 ítems/día, ROI 5.0x)
- La **tarde (15–17hrs)** tiene el ticket promedio más alto: $50.11
- El **desayuno (7–9hrs)** representa el 27.6% del ingreso total — subestimado
- La **hora 18** era la única no rentable (–$7/día) → ya eliminada con cierre a 5pm

### 5️⃣ Margen por Categoría | Margin by Category
- **Desayunos** lidera en margen total: **$12,631** (21.2%)
- La **Comida Corrida** tiene el mejor margen por unidad: **$32.50**
- Categoría **Saludable**: solo 164 unidades pero $24.70 de margen/unidad — subutilizada
- El % de margen igual en todos los productos NO implica igual valor en pesos

### 6️⃣ Optimización de Personal | Staff Optimization
- Costo total personal: **$17,750/mes** (19.4% del ingreso)
- Solo la hora 18 generaba pérdida operativa
- Horas 10–11am: bajas en volumen pero rentables (ROI 1.7x) → prep y descansos
- Estructura óptima: Cocinero 7–5pm | Cajera 7–5pm | Ayudante 12–4pm

---

## 💰 Impacto Financiero Proyectado | Projected Financial Impact

| Iniciativa | Impacto Mensual |
|---|---|
| Optimización horario y personal | +$2,082 |
| Estrategia de combos (5% conversión) | +$1,800 |
| Ajuste de precios en Antojitos (+$2) | +$1,534 |
| **TOTAL MENSUAL ESTIMADO** | **+$5,416** |
| **TOTAL ANUAL PROYECTADO** | **+$64,992** |

---

## 📁 Estructura del Archivo | File Structure

```
Cafeteria_LaCorreiente_Mayo2025.xlsx
│
├── Resumen Ejecutivo EN     ← Executive summary (English)
├── Resumen Ejecutivo ES     ← Resumen ejecutivo (Español)
├── Transacciones            ← 3,426 líneas de venta (raw data)
├── Catálogo Productos       ← 75 productos con costos y márgenes
├── Resumen Ejecutivo        ← KPIs generales del mes
├── Gastos Fijos             ← P&L completo del negocio
├── Utilidad Neta Diaria     ← Rentabilidad por día hábil
├── Insight 1 — Punto Equilibrio
├── Insight 2 — Pareto & Basket
├── Insight 3 — Quincenas
├── Insight 4 — Horas Rentables
├── Insight 5 — Margen Categoria
└── Insight 6 — Optimizacion Hrs
```

---

## 🛠️ Herramientas Utilizadas | Tools Used

| Herramienta | Uso |
|---|---|
| **Python 3.12** | Generación del dataset, cálculos, automatización |
| **Pandas** | Manipulación y agrupación de datos |
| **OpenPyXL** | Construcción y formato del archivo Excel |
| **Excel** | Visualización final y entrega al cliente |
| **Market Basket Analysis** | Identificación de pares de productos frecuentes |
| **Pareto Analysis** | Clasificación estratégica del menú |

---

## 📚 Conceptos Aplicados | Applied Concepts

- `GROUP BY` y agregaciones (equivalente SQL en Pandas)
- Análisis de punto de equilibrio (Break-Even Analysis)
- Ley de Pareto (Regla 80/20)
- Market Basket Analysis (análisis de canasta)
- Costeo por actividad — por qué NO distribuir gastos fijos por producto
- ROI operativo por franja horaria
- Análisis de ciclo de pago (comportamiento por quincena)
- Documentación de supuestos como práctica profesional

---

## 👤 Autor | Author

**J. Carlos Hernández**  
Analista de Datos en Formación | Data Analyst in Training  
Programa: Data Analyst con IA — Proyecto #1 de 6  

---

## ⚠️ Nota sobre los Datos | Data Note

**ES:** Los datos de transacciones fueron generados sintéticamente con lógica de negocio real (patrones de quincena, horas pico, preferencias por categoría). Los precios y costos provienen de un menú real de cafetería. Este proyecto es con fines educativos y de portafolio.

**EN:** Transaction data was synthetically generated with real business logic (pay-cycle patterns, peak hours, category preferences). Prices and costs come from a real cafeteria menu. This project is for educational and portfolio purposes.

---

*Proyecto completado: Junio 2025 | Project completed: June 2025*
