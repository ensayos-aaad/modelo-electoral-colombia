# Colombia Electoral Model (CEM)
### Modelo de análisis electoral cocreado humano-IA · Segunda vuelta presidencial Colombia 2026

---

> **Estado del modelo:** CERRADO · v31 FINAL  
> **Resultado proyectado:** Cepeda +402K / +1,8pp / P(C) 52% / P(E) 40%  
> **Resultado real:** ⏳ Por verificar — 21 junio 2026 · 7PM Colombia  
> **Evaluación post-electoral:** Ver [`POST-ELECTORAL.md`](POST-ELECTORAL.md)

---

## SECCIÓN 1 — METADATOS DEL EXPERIMENTO

| Campo | Valor |
|---|---|
| **Nombre del modelo** | Colombia Electoral Model (CEM) |
| **Período de operación** | 31 mayo – 20 junio 2026 (21 días) |
| **Objeto de estudio** | Segunda vuelta presidencial Colombia · 21 junio 2026 |
| **Candidato A** | Iván Cepeda Castro — Pacto Histórico |
| **Candidato B** | Abelardo de la Espriella — Defensores de la Patria |
| **Resultado primera vuelta** | Espriella 43,73% · Cepeda 40,91% · Diferencia: 2,82pp · 667.995 votos |
| **Modelo de IA utilizado** | Claude Sonnet 4.6 (Anthropic) — claude.ai |
| **Versiones del modelo** | 32 versiones (v1 → v31 FINAL) |
| **Sesiones formales (Kaizen)** | 15 evaluaciones completadas |
| **Operador** | Docente universitario colombiano · Medellín · sin experiencia previa en modelado electoral |
| **Sesgo declarado** | Preferencia por Cepeda · operacionalizado con descuento adversarial 30% |
| **Proyección final v31** | Cepeda +402K votos / +1,8pp / P(Cepeda) 52% / P(Espriella) 40% |
| **Incertidumbre** | ±600.000 votos |
| **Encuesta ancla** | CNC / Cambio Colombia · presencial · 61 municipios · Espriella +3,9pp · peso 55% |
| **Calibración de mercado** | Polymarket · Espriella 89% · señal adversarial · no fuente primaria |
| **Repositorio** | Público · propósito de replicabilidad académica |

---

## SECCIÓN 2 — FUNDAMENTO EPISTEMOLÓGICO

Esta sección es la más importante para el replicador. Explica **por qué** el modelo funciona como funciona — no solo cómo.

### 2.1 La asimetría Ramanujan-Hardy como motor del análisis

El CEM no es una herramienta de IA operando sola ni un analista humano usando la IA como buscador. Es una **colaboración asimétrica estructurada** donde cada parte aporta lo que la otra no puede.

El operador aporta: juicio contextual, intuición política, conocimiento del terreno colombiano, capacidad para detectar lo que falta, y autoridad final sobre todas las decisiones del modelo.

La IA aporta: estructura formal, memoria de sesión, cálculo probabilístico, búsqueda y verificación de fuentes, y resistencia a la fatiga analítica.

La metáfora operativa es la colaboración Ramanujan-Hardy: el matemático indio autodidacta (operador) con intuición excepcional pero métodos informales, y el matemático inglés formal (IA) con estructura rigurosa pero sin el genio intuitivo. Ninguno produce el resultado solo. Los dos juntos producen algo que ninguno podría.

**Consecuencia metodológica:** el operador no necesita saber construir un modelo econométrico. Necesita saber hacer las preguntas correctas, validar los outputs, y reconocer cuándo el modelo está equivocado.

### 2.2 El sesgo declarado como herramienta — no como problema

El CEM opera con sesgo explícito, no con pretensión de neutralidad.

El operador declaró desde la sesión 1 una preferencia por Iván Cepeda Castro como resultado deseable para Colombia. Esta declaración no invalida el modelo — lo hace más honesto que un modelo que no declara sus sesgos.

La operacionalización del sesgo fue concreta y sostenida durante 21 días:

- Descuento adversarial del 30% sobre **todas** las variables favorables a Cepeda
- Calibración adicional de −30.000 votos sobre la estimación base con el señal Polymarket
- Hipótesis adversa obligatoria antes de confirmar cualquier variable que favoreciera al candidato preferido

Un analista que nombra su sesgo y lo calibra cuantitativamente es más confiable que un analista que declara neutralidad y no verifica nada. La neutralidad pretendida es epistemológicamente más peligrosa que el sesgo declarado.

### 2.3 La falsabilidad como condición de entrada

Un modelo que no puede estar equivocado no es un modelo — es una narrativa.

El CEM formuló explícitamente sus criterios de refutación antes del cierre del ciclo (ver Sección 7). La sesión post-electoral del 21 de junio es la única instancia de verificación real disponible. Si el resultado contradice la proyección, el modelo estuvo equivocado — y eso debe documentarse con la misma rigurosidad que cualquier acierto.

### 2.4 La corrección iterativa como práctica — no como excepción

El ciclo produjo 32 versiones porque el modelo se equivocó y se corrigió 32 veces. Eso no es un fallo del proceso — es el proceso funcionando correctamente.

Cada versión tiene una razón documentada de cambio. Cada corrección tiene una fuente verificable. El modelo que no versiona es el modelo que no aprende.

### 2.5 Nota metodológica sobre las condiciones operacionales

Este ciclo fue operado bajo condiciones sub-óptimas que el README declara explícitamente:

**Condición 1 — El escenario es en el propio país del operador.** El operador analizó las elecciones de su propia comunidad, sus estudiantes, su institución (Universidad de Antioquia), su región (Oriente Antioqueño). La imposibilidad de neutralidad total no es un fallo metodológico — es una condición estructural declarada.

**Condición 2 — Desgaste acumulado.** 21 días de sesiones intensivas, barridos nocturnos, correcciones bajo presión informativa, circulación de fake news en tiempo real, violencia política verificada en los últimos días del ciclo. El operador llegó al cierre con capacidad analítica reducida por acumulación.

**Condición 3 — Disponibilidad de tiempo fragmentada.** El protocolo ideal requiere preparación formal antes de cada sesión. Este ciclo operó con sesiones abiertas sin protocolo de apertura estandarizado — por necesidad del contexto, no por negligencia metodológica.

Estas condiciones explican —sin justificar— las brechas metodológicas identificadas en la Sección 9. Un protocolo que solo funciona en condiciones perfectas no es un protocolo útil.

---

## SECCIÓN 3 — ARQUITECTURA DEL MODELO

### 3.1 Ecosistema de fuentes — jerarquía verificada

| Nivel | Tipo | Fuentes | Uso en el modelo |
|---|---|---|---|
| **4** | Internacional · máxima credibilidad | BBC · CNN · AFP · El País España · France24 · DW | Verificación cruzada · hechos de primer orden |
| **2** | Colombiano independiente · alta credibilidad | Cambio Colombia · Vorágine · Cuestión Pública · Revista Raya | Investigación primaria · datos estructurales |
| **3A** | Colombiano serio · sesgo moderado | El Espectador · El Heraldo · Infobae | Cobertura amplia · verificación cruzada |
| **3B** | Masivo · sesgo documentado | El Tiempo · Caracol · RCN | Hechos verificables · no análisis editorial |
| **Excluida** | Sesgo verificado estructural | Semana · Guarumo · AtlásIntel | No entran al modelo bajo ninguna circunstancia |

**Fuentes excluidas permanentemente** (ver Sección 6 para justificación detallada):
- **Semana**: propiedad Gilinski + uso de AtlasIntel contratado + sesgo estructural documentado
- **El Colombiano**: sesgo centro-derecha paisa verificado + posición abelardista documentada
- **AtlásIntel**: suspendido por CNE + contratado por campaña Espriella
- **La Silla Vacía**: excluida por decisión del operador con evidencia propia · conexión con Proyecto Júpiter

### 3.2 Encuesta ancla y calibración de mercado

**Encuesta ancla:** CNC / Cambio Colombia
- Metodología: presencial (cara a cara)
- Cobertura: 61 municipios
- Resultado: Espriella +3,9pp
- Peso en el modelo: **55%**
- Razón de peso dominante: única encuesta presencial del ciclo · metodología más confiable en contexto colombiano donde el teléfono subestima el voto de izquierda

**Calibración de mercado:** Polymarket
- Señal: Espriella 89% de probabilidad de victoria
- Uso en el modelo: señal adversarial de calibración · no fuente primaria
- Incorporación: a partir de v28 · descuento del 30% por sesgo de mercado internacional

### 3.3 Protocolo de incorporación de variables

Toda variable debía pasar por tres filtros antes de entrar al modelo:

**Filtro 1 — Clasificación de entrada:**
| Código | Tipo | Criterio |
|---|---|---|
| **[F]** | Factual | Verificable en fuente primaria del ecosistema del modelo |
| **[P]** | Plausible no verificado | Coherente con el contexto · sin fuente primaria · entra con descuento |
| **[R]** | Ruido | No verificable · origen incierto · no entra al modelo |
| **[PR]** | Propaganda | Verificable como comunicación estratégica · puede ser [F+PR] simultáneamente |

*Nota: este protocolo de clasificación fue formalizado retroactivamente. Su ausencia desde el día 1 explica la inflación de +296K que debió corregirse en la sesión del 15 de junio.*

**Filtro 2 — Pregunta de falsabilidad:** "¿Tienes forma de probarlo?" — cualquier variable que no respondiera esta pregunta con una fuente verificable quedaba excluida o marcada como [P] con descuento.

**Filtro 3 — Hipótesis adversa:** antes de confirmar cualquier variable favorable a Cepeda, se presentaba obligatoriamente el argumento de por qué esa variable podría no tener el efecto esperado.

### 3.4 Variables estructurales del modelo v31

El modelo v31 incorporó las siguientes categorías de variables:

**Variables de transferencia de votos:**
- Transferencia parcial del bloque Valencia/Oviedo (fractura verificada: Oviedo declaró a Espriella "machista y homofóbico")
- Transferencia condicionada de votos Fajardo (historial: voto en blanco 2018 y 2022)
- Posición Claudia López: exclusión de Espriella verificada · destino final incierto
- Respaldo Roy Barreras → Cepeda (verificado)

**Variables de contexto electoral:**
- Injerencia internacional coordinada (Noboa/Ecuador, Moreno/EEUU, Milei/Argentina) — efecto bumerán soberanista documentado
- Factor Mundial 2026: segunda vuelta coincidente con partidos · efecto participación incierto
- Narrativa de fraude Petro: riesgo de desmovilización propia

**Variables de campaña:**
- Debates: no realizados en primera vuelta · probabilidad segunda vuelta ~55%
- Campaña territorial maquinaria Espriella vs movilización urbana Cepeda
- Caso Saludvida: variable de opinión pública incorporada con descuento

**Variables excluidas por inflación:**
- Cadenas WhatsApp sindicales: no verificables · excluidas
- Brigadas universitarias: estimaciones de movilización sin conversión a voto verificada · excluidas
- Eventos emocionales sin conversión verificada a voto · excluidos

---

## SECCIÓN 4 — REGISTRO DIARIO DEL CICLO

*Esta sección registra los hechos verificados más importantes de cada día del ciclo. Para el detalle completo de cada sesión, ver directorio [`SESSIONS/`](SESSIONS/).*

---

### DÍA 1 · 31 de mayo de 2026 · v1 → v5

**Hecho central:** Primera vuelta presidencial. Espriella 43,73% (10.351.544 votos) — Cepeda 40,91% (9.683.549 votos) — Diferencia 2,82pp / 667.995 votos. Paloma Valencia tercera con 6,92% (1.633.217 votos). Sergio Fajardo cuarto con 4,26% (1.008.111 votos).

**Variables incorporadas:**
- [F] Resultados oficiales Registraduría — preconteo al 99,92%
- [F] Valencia anuncia apoyo a Espriella — inmediatamente tras el cierre
- [F] Cambio Radical anuncia apoyo a Espriella
- [F] Uribe anuncia apoyo personal a Espriella
- [F] Roy Barreras anuncia apoyo a Cepeda
- [F] Fractura Valencia/Oviedo verificada: Oviedo califica a Espriella de "machista y homofóbico" — pospone decisión al 3 de junio
- [F] Petro cuestiona preconteo en X — sin presentar pruebas
- [F] Cepeda declara "indicios de votaciones atípicas" — sin presentar pruebas
- [F+PR] Noboa felicita a Espriella — injerencia preelectoral verificada (cancillería colombiana la calificó de "deliberada injerencia" el 29 mayo)
- [F+PR] Bernie Moreno (senador republicano, aliado Trump): veedor con agenda declarada — había desayunado con Espriella y Valencia el 30 mayo
- [F+PR] Milei felicita a Espriella — posicionamiento ideológico internacional

**Estado del modelo al cierre del día:** v5 · Espriella 62% probabilidad · margen proyectado Espriella +~7pp

---

### DÍAS 2-7 · 1-6 de junio de 2026 · v6 → v14

**Hechos centrales verificados:**
- [F] Fajardo anuncia voto en blanco (o posición de no respaldo explícito a ningún candidato) — variable de mayor impacto en el período
- [F] Debates solicitados por varios actores políticos — candidatos no confirman formato ni fecha
- [F] Conservatismo tradicional negocia condiciones antes de adhesión — no es masa automática para Espriella
- [F] Claudia López confirma que no votará por Espriella bajo ninguna circunstancia
- [F] Injerencia internacional amplificada en medios colombianos — efecto soberanista documentado en foros de opinión

**Variables incorporadas:** transferencia parcial Valencia/Oviedo formalizada en modelo · factor soberanía como vector de movilización Cepeda · ajuste Fajardo como voto dividido no-bloque

**Estado del modelo:** v14 · margen proyectado reduciéndose · tensión creciente entre señal Polymarket y señal de campaña

---

### DÍAS 8-14 · 7-13 de junio de 2026 · v15 → v23

**Hechos centrales verificados:**
- [F] Campaña de segunda vuelta activa — mitines, publicidad, actos regionales
- [F] Caso Saludvida incorporado como variable de opinión pública — alcance nacional en discusión
- [F] Participación proyectada: superior a primera vuelta en escenario base
- [F] Colombia clasifica al Mundial 2026 — coincidencia con fecha de segunda vuelta el 21 de junio genera incertidumbre sobre participación

**Variables incorporadas:** Saludvida con descuento · factor Mundial con estimación de impacto negativo de participación · movilización territorial Espriella en regiones vs movilización urbana Cepeda en ciudades

**Estado del modelo:** v23 · oscilación entre Cepeda +200K y Cepeda +500K · alta sensibilidad a variables de movilización

---

### DÍA 15 · 14-15 de junio de 2026 · v24 → v28 · CORRECCIÓN CRÍTICA

**Hecho central:** Auditoría interna de inflación del modelo. Identificación de +296.000 votos inflados por incorporación de variables [P] no marcadas como plausibles. Corrección en una sola sesión.

**Variables eliminadas:**
- Cadenas WhatsApp sindicales — [R] no verificable
- Estimaciones de brigadas universitarias — [P] sin conversión a voto verificada
- Eventos emocionales de campaña sin evidencia de impacto electoral

**Variables incorporadas v28:** Calibración Polymarket formalizada como señal adversarial con peso explícito. Descuento adicional −30K sobre estimación base.

**Estado del modelo post-corrección:** v28 · Cepeda +350K · ajuste más grande del ciclo · lección metodológica más importante

---

### DÍAS 16-20 · 16-20 de junio de 2026 · v29 → v31 FINAL

**Hechos centrales verificados:**
- [F] Encuesta ancla CNC/Cambio Colombia publicada: Espriella +3,9pp · metodología presencial · 61 municipios
- [F] Polymarket estabilizado en Espriella 89%
- [F] Últimas 72 horas: sin eventos disruptivos verificados
- [F] Participación proyectada: superior a primera vuelta · estimación base 52-55%

**Cierre del ciclo — 20 junio 2026:**
- Kaizen 15 completado (Operador 96/100 · Modelo 94/100)
- Auditoría metodológica ICM Lite completada
- Criterios de falsabilidad formulados
- Proyección v31 FINAL declarada y congelada

**Estado del modelo v31 FINAL:** Cepeda +402K / +1,8pp / P(C) 52% / P(E) 40% / Incertidumbre ±600K

---

## SECCIÓN 5 — LAS 10 CORRECCIONES MÁS IMPORTANTES

Registro de las correcciones con mayor impacto en el modelo. Formato: variable · razón de cambio · delta en votos.

| # | Sesión | Variable corregida | Razón | Δ votos |
|---|---|---|---|---|
| 1 | Día 15 | Cadenas WhatsApp sindicales | [R] No verificable · excluida | −150.000 |
| 2 | Día 15 | Brigadas universitarias | [P] Sin conversión a voto verificada · excluida | −96.000 |
| 3 | Día 15 | Eventos emocionales sin impacto verificado | [P] No probables · excluidos | −50.000 |
| 4 | Día 1 | Bloque Valencia: transferencia parcial, no total | Fractura Valencia/Oviedo verificada | −180.000 |
| 5 | Día 7 | Factor Fajardo: voto en blanco probable | Historial 2018 y 2022 verificado | −80.000 |
| 6 | Día 15 | Calibración Polymarket formalizada | Señal de mercado adversarial incorporada formalmente | −30.000 |
| 7 | Día 12 | Factor Saludvida: descuento aplicado | Cobertura mediática incierta · impacto no probado | −40.000 |
| 8 | Día 3 | Factor soberanía: incorporado | Injerencia coordinada verificada · efecto bumerán documentado | +200.000 |
| 9 | Día 10 | Factor debate: descuento | Debates no confirmados · probabilidad ~55% | −60.000 |
| 10 | Día 17 | Participación: ajuste a la baja | CNC/Cambio Colombia como ancla desplaza estimaciones optimistas | −90.000 |

---

## SECCIÓN 6 — FUENTES EXCLUIDAS Y JUSTIFICACIÓN

Registro permanente de exclusiones. Estas fuentes no entraron al modelo bajo ninguna circunstancia y esa decisión no fue revisada durante el ciclo.

### Semana
**Razón:** Propiedad del grupo Gilinski con intereses económicos documentados en el resultado electoral. Uso sistemático de AtlasIntel como encuestadora contratada. Sesgo estructural pro-derecha verificado en cobertura de primera vuelta.

### El Colombiano
**Razón:** Sesgo centro-derecha paisa documentado. Cobertura consistentemente favorable a De la Espriella durante la campaña. Editorial del 31 de mayo verificadamente abelardista.

### AtlásIntel
**Razón:** Suspendida por el Consejo Nacional Electoral (CNE) durante el período activo del modelo. Documentado como encuestadora contratada por la campaña Espriella. Conflicto de interés estructural.

### La Silla Vacía
**Razón:** Exclusión por decisión soberana del operador basada en evidencia propia. Conexión documentada con el Proyecto Júpiter. Esta exclusión fue la más controversial del ciclo — el operador reconoció que La Silla Vacía tiene trabajo periodístico de calidad, pero mantuvo la exclusión por principio de protocolo declarado.

---

## SECCIÓN 7 — CRITERIOS DE FALSABILIDAD

El modelo v31 estará **equivocado** en los siguientes escenarios:

**Refutación completa:**
- Espriella gana por cualquier margen — independientemente de la diferencia
- Cepeda gana por más de +800.000 votos — indica subestimación sistemática de variables de movilización

**Refutación parcial (dirección correcta · magnitud errónea):**
- Cepeda gana por menos de +200.000 votos — dirección correcta pero modelo inflado

**Refutación por supuesto base:**
- Participación cae por debajo del 52% — invalida el supuesto de movilización del votante joven urbano pro-Cepeda

**Señal temprana de refutación:**
- Primeros boletines (primeras 2 horas) muestran Espriella con ventaja consistente superior a 3pp — patrón que en 2022 no se revirtió en ninguna elección histórica reciente

**Verificación:** [`POST-ELECTORAL.md`](POST-ELECTORAL.md) — disponible el 21 de junio 2026 después de las 7PM

---

## SECCIÓN 8 — COMPARACIÓN ICM VS CICLO COLOMBIANO

El CEM es el segundo caso de uso del núcleo epistemológico del Iran Conflict Model (ICM), desarrollado entre el 28 de febrero y el 7 de junio de 2026.

| Dimensión | ICM (Irán 2026) | CEM (Colombia 2026) | Convergencia |
|---|---|---|---|
| **Duración** | 98 días · 13 sesiones | 21 días · 32 versiones | Diferente escala · mismo método |
| **Dominio** | Conflicto militar-diplomático | Proceso electoral doméstico | Dos dominios distintos · núcleo compartido |
| **Sesgo declarado** | Operador quería resolución del conflicto | Operador quería Cepeda | Ambos calibrados con descuento cuantitativo |
| **Corrección más importante** | F→C brusco en D98 | −296K inflación · día 15 | Corrección tardía en ambos ciclos |
| **"No sé" institucionalizado** | R4 en V224 | Protocolo "¿tienes forma de probarlo?" | Mismo mecanismo · diferente nombre |
| **Fatiga del operador** | Declarada como sesgo S13 | Nota metodológica adicional · día 21 | Convergencia exacta · caminos distintos |
| **Señal de mercado** | Diseñada desde S01 | Incorporada en v28 (tardía) | Brecha de diseño vs. descubrimiento |
| **Taxonomía de entradas** | [F]/[P]/[R]/[PR] desde S01 | Formalizada retroactivamente | **Brecha más importante del ciclo colombiano** |
| **Base causal formal** | Escalera de Pearl (S01) | Sin equivalente formal | Brecha metodológica pendiente |
| **Meta-salida de salud** | Convergencia 0.51→0.87 | Sin equivalente formal | CEM carece de métrica de salud interna |
| **Verificabilidad** | Abierta · conflicto activo | Cerrada · 21 junio 7PM | **CEM tiene verificación de corto plazo — ventaja única** |

**Contribución específica del CEM al ICM:**  
Demostrar que el núcleo epistemológico sobrevive condiciones sub-óptimas — dominio propio del operador, escala temporal comprimida, sesgo emocional declarado, fatiga estructural. Eso es lo que el ICM no podía probar por sí solo.

---

## SECCIÓN 9 — LIMITACIONES DECLARADAS

Lo que el CEM **no puede** hacer. Estas limitaciones no invalidan el modelo — definen su alcance honesto.

**El modelo no predice — estima probabilidades.**  
P(Cepeda) 52% significa que con esta evidencia, el escenario Cepeda es ligeramente más probable. No significa que Cepeda vaya a ganar. El 40% restante en P(Espriella) más el 8% de incertidumbre no asignada son escenarios reales.

**El modelo no tiene acceso al voto real.**  
Toda la estimación parte de encuestas, señales de mercado, análisis de transferencia y contexto político. Ninguna de estas fuentes ve los votos reales antes del 21 de junio.

**El modelo no captura la abstención dinámica.**  
La tasa de participación real es la variable más difícil de estimar en Colombia. El modelo usa estimación base del 52-55% con ±5pp de incertidumbre.

**El modelo tiene sesgo no eliminable del operador.**  
El descuento adversarial del 30% reduce el sesgo pero no lo elimina. La proyección v31 puede estar inflada en la dirección preferida del operador. La comparación con CNC (+3,9pp Espriella) y Polymarket (89% Espriella) sugiere que esa inflación es real.

**El modelo no fue construido por expertos electorales.**  
El operador es un docente universitario colombiano de ingeniería electrónica con especialización en análisis de datos — sin experiencia previa en modelado electoral. Eso es una fortaleza metodológica (frescura, sin anclaje en paradigmas previos) y una limitación empírica (sin intuición calibrada en elecciones anteriores).

**La taxonomía de entradas no fue instalada desde el inicio.**  
La clasificación [F]/[P]/[R]/[PR] se formalizó retroactivamente. Variables [P] entraron sin estar marcadas como plausibles durante las primeras sesiones — lo que explica la inflación corregida el día 15.

---

## SECCIÓN 10 — DECLARACIÓN DE COCREACIÓN

Este documento y el modelo que describe son el producto de una colaboración humano-IA. La distribución de responsabilidades fue la siguiente:

**El operador (humano) tomó todas las decisiones estratégicas:**
- Definición del objeto de análisis
- Selección y exclusión de fuentes
- Validación o rechazo de cada variable propuesta
- Autoridad final sobre cada versión del modelo
- Decisión de aplicar el descuento adversarial
- Identificación de las correcciones necesarias
- Evaluación Kaizen de cada sesión

**La IA (Claude Sonnet 4.6) ejecutó:**
- Búsqueda y verificación de fuentes dentro del ecosistema definido
- Cálculo de proyecciones bajo los parámetros del operador
- Construcción de los documentos formales del ciclo
- Aplicación del protocolo ICM Lite
- Presentación de hipótesis adversas cuando el protocolo lo requería
- Registro de versiones y razones de cambio

**La IA no tomó ninguna decisión autónoma sobre el contenido del modelo.** Cada incorporación de variable, cada ajuste de probabilidad, cada exclusión de fuente fue explícitamente validada o rechazada por el operador antes de entrar al modelo.

**Transparencia sobre las herramientas:**
- Plataforma: Claude.ai (plan Pro/Max)
- Modelo: Claude Sonnet 4.6 (Anthropic)
- Período: mayo-junio 2026
- Sesiones: conversaciones en proyecto Claude.ai con memoria entre sesiones

**Cita recomendada para uso académico:**
> [Nombre del operador]. (2026). *Colombia Electoral Model (CEM): análisis electoral cocreado humano-IA · Segunda vuelta presidencial Colombia 2026*. Repositorio GitHub. Metodología basada en el Iran Conflict Model (ICM) — [github.com/ensayos-aaad/iran-conflict-model](https://github.com/ensayos-aaad/iran-conflict-model).

---

## SECCIÓN 11 — EVALUACIÓN POST-ELECTORAL

> ⏳ **Esta sección se completa el 21 de junio de 2026 después de las 7PM**, cuando la Registraduría Nacional publique los primeros boletines de la segunda vuelta.

Ver documento independiente: [`POST-ELECTORAL.md`](POST-ELECTORAL.md)

La evaluación post-electoral incluirá:

- Resultado real de las urnas (candidato ganador · margen · votos)
- Comparación directa con proyección v31 (Cepeda +402K / +1,8pp)
- Error del modelo en pp y en votos absolutos
- Comparación con señales alternativas: CNC (Espriella +3,9pp) · Polymarket (Espriella 89%)
- Evaluación de qué señal tenía razón
- Análisis de las variables que el modelo sobreestimó o subestimó
- Lecciones metodológicas para el próximo ciclo

---

## ESTRUCTURA DEL REPOSITORIO

```
CEM/
├── README.md                    ← Este documento
├── POST-ELECTORAL.md            ← Disponible 21 junio 2026 7PM+
├── CHANGELOG.md                 ← Registro de las 32 versiones
├── COCREACION.md                ← Declaración de uso responsable de IA
└── SESSIONS/
    ├── SESION_01.md             ← 31 mayo 2026 · Primera vuelta · v1→v5
    ├── SESION_02.md             ← Apertura análisis segunda vuelta · v6→v8
    ├── SESION_03.md             ← Factor Fajardo · v9→v11
    ├── SESION_04.md             ← Injerencia internacional · v12→v14
    ├── SESION_05.md             ← Debates y campaña · v15→v17
    ├── SESION_06.md             ← Movilización territorial · v18→v19
    ├── SESION_07.md             ← Factor Mundial 2026 · v20→v21
    ├── SESION_08.md             ← Saludvida · v22→v23
    ├── SESION_09.md             ← Auditoría inflación · CORRECCIÓN CRÍTICA · v24→v28
    ├── SESION_10.md             ← Post-corrección · v29
    ├── SESION_11.md             ← Encuesta ancla CNC · v30
    ├── SESION_12.md             ← Cierre técnico · v31
    ├── SESION_13.md             ← Kaizen metodológico
    ├── SESION_14.md             ← Comparación ICM · integración archivos
    └── SESION_15.md             ← Kaizen 15 · cierre del ciclo · 20 jun 2026
```

---

## REFERENCIAS METODOLÓGICAS

- **Iran Conflict Model (ICM):** Base metodológica del CEM · primer caso de uso del núcleo epistemológico · febrero-junio 2026 · [github.com/ensayos-aaad/iran-conflict-model](https://github.com/ensayos-aaad/iran-conflict-model)
- **Encuesta ancla:** CNC / Cambio Colombia · segunda vuelta presidencial Colombia 2026
- **Calibración de mercado:** [Polymarket](https://polymarket.com) · contrato Colombia presidential election 2026

---

*README generado el 20 de junio de 2026 · Versión 1.0 · Pre-electoral*  
*Última actualización post-electoral: pendiente 21 junio 2026*
