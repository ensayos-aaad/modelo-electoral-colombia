# COCREACION.md — Colombia Electoral Model (CEM)
### Declaración de cocreación humano-IA · Uso responsable · Transparencia metodológica

---

## 1. NATURALEZA DEL DOCUMENTO

Este documento declara de forma transparente cómo fue construido el Colombia Electoral Model (CEM): quién tomó cada tipo de decisión, qué hizo la IA, qué hizo el humano, y cuáles son las implicaciones éticas y metodológicas de ese proceso.

No es un documento de resultados ni de análisis. Es una declaración de proceso — el equivalente a la sección de metodología de un paper académico, escrita en lenguaje accesible para cualquier replicador.

---

## 2. PRINCIPIO CENTRAL

> **La IA puede cometer errores. Por eso el humano valida cada output.**

Este principio no es una advertencia de descargo — es la columna vertebral del método. El CEM no es un sistema de IA operando de forma autónoma. Es una colaboración estructurada donde el humano mantiene la autoridad epistemológica en todo momento.

---

## 3. DISTRIBUCIÓN DE ROLES

### 3.1 Lo que hizo el operador humano

El operador tomó **todas** las decisiones estratégicas del modelo:

- Definición del objeto de análisis y del período de cobertura
- Selección de las fuentes del ecosistema y exclusión permanente de fuentes con sesgo documentado
- Validación o rechazo de cada variable propuesta por la IA antes de incorporarla al modelo
- Decisión de aplicar el descuento adversarial del 30% sobre variables favorables al candidato preferido
- Identificación de la inflación acumulada y solicitud de auditoría en la sesión del 15 de junio
- Exclusión de variables específicas cuando no superaron el protocolo "¿tienes forma de probarlo?"
- Evaluación Kaizen de cada sesión con calificación explícita al operador y al modelo
- Decisión de cierre del ciclo y congelamiento de la proyección v31 FINAL

El operador también tomó las decisiones que **no están en el modelo**: qué no investigar, qué no incluir, cuándo detener una línea de análisis. Las decisiones de exclusión son tan importantes como las de inclusión.

### 3.2 Lo que hizo la IA

La IA ejecutó las instrucciones del operador dentro de los parámetros definidos por él:

- Búsqueda y verificación de fuentes dentro del ecosistema definido por el operador
- Cálculo de proyecciones bajo los parámetros cuantitativos aprobados por el operador
- Presentación de hipótesis adversas cuando el protocolo lo requería
- Construcción de los documentos formales del ciclo (este documento incluido)
- Registro de versiones y razones de cambio bajo instrucción del operador
- Aplicación del protocolo ICM Lite según las reglas establecidas por el operador

### 3.3 Lo que la IA NO hizo

- No incorporó ninguna variable sin validación explícita del operador
- No tomó decisiones sobre qué fuentes incluir o excluir
- No decidió qué peso asignar a la encuesta ancla
- No aplicó el descuento adversarial de forma autónoma — lo ejecutó bajo instrucción
- No cerró ninguna versión del modelo sin confirmación del operador
- No generó conclusiones políticas propias — generó proyecciones probabilísticas bajo parámetros aprobados

---

## 4. EL SESGO COMO VARIABLE DECLARADA

El operador del CEM tiene una preferencia política verificada: considera que una victoria de Iván Cepeda Castro sería más beneficiosa para Colombia que una victoria de Abelardo de la Espriella.

Esta preferencia no fue ocultada. Fue declarada en la primera sesión del ciclo y operacionalizada de la siguiente manera:

**Descuento adversarial:** el 30% del valor estimado de toda variable favorable a Cepeda fue eliminado de la proyección antes de incorporarla. Si una variable valía +100.000 votos para Cepeda, el modelo incorporaba +70.000.

**Calibración de mercado:** Polymarket (señal adversarial de mercado, Espriella 89%) fue incorporado formalmente como contrapeso desde v22.

**Hipótesis adversa obligatoria:** antes de confirmar cualquier variable favorable a Cepeda, el modelo presentaba obligatoriamente el argumento de por qué esa variable podría no tener el efecto esperado.

**Consecuencia declarada:** la proyección v31 puede estar inflada en la dirección del candidato preferido por el operador. La comparación con la encuesta ancla CNC (Espriella +3,9pp) y con Polymarket (Espriella 89%) sugiere que esa inflación es real. El replicador debe tener esto en cuenta al evaluar el modelo.

---

## 5. PROTOCOLO DE VERIFICACIÓN ACTIVA

El CEM operó con un protocolo de verificación que el operador aplicó de forma sostenida durante 21 días:

**Pregunta estándar:** "¿Tienes forma de probarlo?"

Cualquier variable que no pudiera ser respondida con una fuente verificable del ecosistema del modelo quedaba excluida o incorporada con clasificación `[P]` (plausible no verificado) y descuento.

La corrección más importante del ciclo — la eliminación de +296.000 votos el 15 de junio — fue el resultado directo de este protocolo aplicado de forma sistemática sobre las variables de movilización acumuladas en las semanas previas.

---

## 6. LIMITACIONES ÉTICAS DEL USO DE IA EN ANÁLISIS ELECTORAL

El CEM fue construido con consciencia de las siguientes limitaciones éticas:

**6.1 El modelo no influye — analiza.** El CEM fue diseñado para analizar un proceso electoral, no para influir en él. Sus proyecciones no fueron difundidas públicamente durante el ciclo activo del modelo. Este repositorio se publica con fines de replicabilidad metodológica, no de propaganda electoral.

**6.2 La IA no es árbitro electoral.** Las proyecciones del CEM no tienen valor vinculante. El único árbitro legítimo del resultado electoral es la Registraduría Nacional del Estado Civil de Colombia con sus mecanismos de escrutinio verificado.

**6.3 El sesgo del operador es declarado pero no eliminado.** Cualquier persona que use este modelo o sus documentos debe tener en cuenta que fue construido por un operador con preferencia política explícita por uno de los candidatos. El descuento adversarial reduce el sesgo — no lo elimina.

**6.4 La IA no tiene acceso privilegiado a información.** Toda la información que procesó la IA provino de fuentes públicas verificables del ecosistema definido por el operador. La IA no tiene acceso a datos privados, encuestas internas de campaña, o información no disponible públicamente.

**6.5 El modelo es un experimento metodológico, no una predicción.** El propósito principal del CEM no fue predecir el resultado electoral — fue demostrar que un método de análisis estructurado humano-IA es replicable, falseable y metodológicamente honesto. La falsabilidad se verifica el 21 de junio de 2026 en [`POST-ELECTORAL.md`](POST-ELECTORAL.md).

---

## 7. CONDICIONES OPERACIONALES DEL CICLO

El CEM fue operado bajo condiciones que cualquier replicador debe conocer:

**El operador analizó las elecciones de su propio país.** No existe distancia emocional ni geográfica. El operador es un ciudadano colombiano cuya vida, institución de trabajo (Universidad de Antioquia) y comunidad (El Santuario, Oriente Antioqueño) están directamente afectadas por el resultado electoral. Esta condición amplifica el sesgo declarado y reduce la capacidad de neutralidad analítica — ambas cosas son registradas aquí, no negadas.

**El operador no es un experto electoral.** El operador es un docente universitario con formación en ingeniería electrónica y análisis de datos. No tiene experiencia previa en modelado electoral, no proviene de la ciencia política, y no tiene vínculos con ninguna campaña, partido o organización electoral. Eso es simultáneamente una limitación empírica y una fortaleza metodológica.

**El ciclo operó bajo fatiga acumulada.** 21 días de sesiones intensivas, análisis bajo presión informativa, circulación de desinformación en tiempo real y carga emocional por el escenario. El operador declaró explícitamente fatiga acumulada al cierre del ciclo — lo que es metodológicamente honesto registrar.

---

## 8. TRAZABILIDAD Y REPLICABILIDAD

Todos los elementos necesarios para replicar el experimento están disponibles en este repositorio:

| Documento | Contenido | Propósito |
|---|---|---|
| `README.md` | Metadatos · epistemología · arquitectura · limitaciones | Marco general del experimento |
| `CHANGELOG.md` | 32 versiones con razón de cambio y delta en votos | Trazabilidad del modelo |
| `SESSIONS/` | 15 archivos de sesión con hechos verificados | Registro operacional día a día |
| `COCREACION.md` | Este documento | Transparencia metodológica |
| `POST-ELECTORAL.md` | Resultado real vs proyección v31 | Verificación de falsabilidad |

**Base metodológica:** el CEM es el segundo caso de uso del núcleo epistemológico del Iran Conflict Model (ICM). El ICM está disponible en [github.com/ensayos-aaad/iran-conflict-model](https://github.com/ensayos-aaad/iran-conflict-model).

---

## 9. INSTRUCCIONES PARA EL REPLICADOR

Si desea replicar este experimento en otro proceso electoral o geopolítico:

**Antes de comenzar:**
1. Declare su sesgo explícitamente — no pretenda neutralidad
2. Defina el ecosistema de fuentes antes de la primera sesión
3. Instale la taxonomía `[F]`/`[P]`/`[R]`/`[PR]` desde el inicio — no retroactivamente
4. Formule los criterios de falsabilidad antes de la primera proyección

**Durante el ciclo:**
5. Aplique el descuento adversarial sobre todas las variables que favorezcan al resultado que prefiere
6. Use la pregunta "¿tienes forma de probarlo?" antes de incorporar cualquier variable
7. Registre la razón de cada cambio de versión — si no puede explicar por qué cambió, el cambio no debería haberse hecho
8. Evalúe al final de cada sesión: ¿qué hice bien el operador? ¿qué hizo bien el modelo?

**Al cerrar:**
9. Congele la proyección antes del resultado — no la modifique retroactivamente
10. Publique los criterios de falsabilidad antes de conocer el resultado
11. Complete el documento post-electoral con el resultado real, sin suavizar el error si lo hubo

---

## 10. DECLARACIÓN FINAL

El Colombia Electoral Model fue construido en buena fe, con los mejores datos disponibles, con sesgo declarado y calibrado, y con el propósito explícito de demostrar que el análisis estructurado humano-IA es metodológicamente honesto y replicable.

No es un modelo perfecto. Tiene las limitaciones declaradas en la Sección 9 del README. Fue construido bajo condiciones sub-óptimas que también están declaradas. Y puede estar equivocado — los criterios de esa equivocación están en `POST-ELECTORAL.md`.

Lo que sí es: el registro más transparente posible de cómo se construyó un análisis probabilístico en tiempo real, con qué herramientas, bajo qué sesgos, con qué fuentes, y con qué resultado. Eso es lo que lo hace replicable.

---

*COCREACION.md generado el 20 de junio de 2026*
*Colombia Electoral Model (CEM) · Segunda vuelta presidencial Colombia 2026*
*Base metodológica: [Iran Conflict Model](https://github.com/ensayos-aaad/iran-conflict-model)*
