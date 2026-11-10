# 01. Presupuestos municipales

## La situación

Trabajas en el área económica de la Diputación. Te han ido llegando, año a año,
las liquidaciones de los presupuestos de **20 municipios de la provincia de
Málaga** entre 2019 y 2024, un fichero de Excel por año, en `datos/`, tal como
los mandaron. Te piden un análisis rápido de cómo ha evolucionado el gasto.

## Las variables

| Columna | Qué es |
|---|---|
| `municipio`, `provincia` | Identificación del municipio |
| `poblacion` | Habitantes a 1 de enero (padrón) |
| `ingresos_no_financieros` | Capítulos 1 a 7 de ingresos (derechos reconocidos netos) |
| `gastos_no_financieros` | Capítulos 1 a 7 de gastos (obligaciones reconocidas netas) |
| `gasto_personal` | Capítulo 1 de gastos |
| `inversiones` | Capítulo 6 de gastos (inversiones reales) |
| `deuda_viva` | Deuda viva a 31 de diciembre |

Importes en euros.

## Fuente

Datos **simulados** con fines docentes. Imitan la estructura de las
liquidaciones de las entidades locales que publica el Ministerio de Hacienda,
y las magnitudes son verosímiles, pero no son las cifras reales de ningún
ayuntamiento.
