# SESIÓN 04 · 4-5 de junio de 2026
**Versiones:** v10 → v11 · **Kaizen:** 3

---

## HECHOS VERIFICADOS INCORPORADOS

- `[F]` Segunda vuelta: 21 de junio de 2026 — mismo día de partidos del Mundial 2026. Fuente: FIFA / Registraduría.
- `[F]` Alianza Verde: respaldo formal a Cepeda confirmado. Fuente: declaración oficial partido.
- `[F]` Clara López (ex-candidata): adhiere formalmente a Cepeda. Fuente: declaración pública.
- `[F]` Mapa de bloques consolidado al cierre de primera semana: Bloque Espriella ~12M votos (~50,6%) · Bloque Cepeda ~11,1M votos (~46,9%). Fuente: cálculo propio sobre datos Registraduría.

---

## CORRECCIONES APLICADAS

- Estimaciones de participación optimistas para Cepeda ajustadas a la baja por factor Mundial. **Δ: −30.000 votos Cepeda.**

---

## VARIABLES NUEVAS INCORPORADAS

| Variable | Clasificación | Fuente | Δ votos |
|---|---|---|---|
| Factor Mundial / participación | `[F]` | FIFA / Registraduría | −30.000 |
| Alianza Verde formal | `[F]` | Declaración partido | +20.000 |
| Clara López adhesión | `[F]` | Declaración pública | +15.000 |

---

## DECISIONES METODOLÓGICAS

- **Factor Mundial:** incorporado como reducción de participación en segmentos urbanos jóvenes — exactamente el segmento más pro-Cepeda. Efecto estimado: −2 a −4pp en participación urbana.
- **Mapa de bloques:** formalizado como punto de referencia estructural. Las diferencias brutas favorecen a Espriella — la pregunta es qué porcentaje de los bloques se convierte en voto efectivo.
- **Cepeda necesita:** alta participación urbana + transferencia parcial pero real de votos de centro.

---

## ESTADO DEL MODELO AL CIERRE

| Variable | Valor |
|---|---|
| Versión | v11 |
| Margen proyectado | Espriella −680.000 votos |
| P(Cepeda) | 45% |
| P(Espriella) | 55% |
| Variable pivote | Conversión real de bloques a voto efectivo |

---

## KAIZEN DE LA SESIÓN

**Operador:** 86/100 — identificó el factor Mundial como variable de participación real.
**Modelo:** 84/100 — mapa de bloques bien construido y útil como ancla estructural.
**Muda más importante:** los bloques de voto en primera vuelta no son transferibles automáticamente. El modelo necesitaba incorporar tasas de conversión reales, no transferencias en bloque.
