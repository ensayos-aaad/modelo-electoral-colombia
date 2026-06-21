# SESIÓN 05 · 6-7 de junio de 2026
**Versiones:** v12 → v13 · **Kaizen:** 4

---

## HECHOS VERIFICADOS INCORPORADOS

- `[F]` Campaña territorial Espriella activa en regiones costeras y Caribe. Fuente: medios nivel 3A/3B.
- `[F]` Campaña urbana Cepeda activa en Bogotá, Medellín, Cali. Fuente: medios nivel 3A/3B.
- `[F]` Colombia confirma partidos del Mundial el 21 de junio coincidentes con segunda vuelta. Fuente: FIFA.

---

## CORRECCIONES APLICADAS

- Descuento por factor Mundial aplicado sobre estimaciones de participación urbana. **Δ: −40.000 votos Cepeda.**

---

## VARIABLES NUEVAS INCORPORADAS

| Variable | Clasificación | Fuente | Δ votos |
|---|---|---|---|
| Movilización maquinaria Espriella regiones | `[P]` | Medios nivel 3B | −60.000 |
| Movilización urbana Cepeda | `[P]` | Medios nivel 3A | +120.000 |
| Factor Mundial participación | `[F]` | FIFA / análisis propio | −40.000 |

⚠️ **Nota retrospectiva:** las variables de movilización `[P]` incorporadas en esta sesión contribuyeron a la inflación corregida en la Sesión 10. Entraron sin marcación explícita de plausibilidad.

---

## DECISIONES METODOLÓGICAS

- **Distinción geográfica:** modelo empieza a diferenciar entre voto regional (Espriella más fuerte) y voto urbano (Cepeda más fuerte).
- **Sesgo de cobertura:** la prensa de nivel 3A cubre más la campaña urbana de Cepeda — puede generar sobreestimación de la movilización pro-Cepeda.

---

## ESTADO DEL MODELO AL CIERRE

| Variable | Valor |
|---|---|
| Versión | v13 |
| Margen proyectado | Espriella −600.000 votos |
| P(Cepeda) | 46% |
| P(Espriella) | 54% |
| Variable pivote | Ratio movilización urbana/rural real |

---

## KAIZEN DE LA SESIÓN

**Operador:** 84/100 — identificó la distinción geográfica como variable estructural.
**Modelo:** 82/100
**Muda más importante:** variables de movilización `[P]` entrando sin descuento suficiente. Primera señal de inflación acumulándose.
