<!--
Copyright (c) 2026 Dr. Aladdin Ali - Founder of Aladdin Pertanian Internasional - dr.alaa@aladdin.my.id. All Rights Reserved.
-->

# Ejemplos Resueltos (Español) — Worked Examples (Spanish)
## Skill reference — `es` SOURCE-GROUNDED ([ES1] Manual de redacción de artículos científicos)
### A la par del archivo en inglés `before-after.md` / at full parity with the English file

> Estos ejemplos tienen una **profundidad equivalente** a `before-after.md` (inglés): los tres canales, **dos
> elementos de sugerencia** (A-01 + A-02), un **registro de revisión** completo y la **compuerta de
> consentimiento**, en español. Cada número/cita/DOI se **conserva carácter por carácter** (INV-A1). Se aplica
> la norma del español académico: **voz impersonal / pasiva-refleja con *se*** (*se observó*, *se realizó*),
> **sin primera persona** [ES1]. El modelo de tres canales y la compuerta de consentimiento son **idénticos**
> a la versión en inglés.

---

## Ejemplo 1 — Afirmación excesiva + de-AI, flujo completo (consentimiento otorgado)

**Contrato:** `level=journal` · `programme_type=journal` · `edit_scope=apply_approved_notes` ·
`co_authored=false` · `ai_disclosure_policy=required` · `output_language=es`.

**Entrada (párrafo de discusión):**
> "En conclusión, nuestro innovador estudio demuestra claramente que el Fármaco X causa hemorragia. 😊 Los
> estudios muestran que este es un hallazgo crucial. En nuestro ensayo, observamos hemorragia en **18** de
> **20** pacientes (véase la **Tabla 2**), lo cual es consistente con Almeida et al. **[7]**."

### Canal 1 — Texto con lenguaje mejorado (automático, solo expresión)
> "El estudio demuestra claramente que el Fármaco X causa hemorragia. Los estudios muestran que este es un
> hallazgo importante. En el ensayo, se observó hemorragia en **18** de **20** pacientes (véase la
> **Tabla 2**), lo cual es consistente con Almeida et al. **[7]**."

*Cambiado (solo expresión):* se eliminó "En conclusión," (HUM-25); "innovador" (HUM-01); "😊" (HUM-18);
"crucial" → "importante" (§B léxico). **Regla de persona/voz (ACA-04 · [ES1]):** "nuestro … estudio" → "el
estudio"; primera persona *"En nuestro ensayo, observamos"* → impersonal *"En el ensayo, se observó"*.
*Conservado:* la afirmación **"demuestra claramente … causa"** (fuerza de la afirmación — esto es Canal 2,
ACA-01); la atribución sin cita **"Los estudios muestran"** (HUM-05, en modo académico → Canal 2); y
**`18` · `20` · `Tabla 2` · `[7]`** — carácter por carácter (INV-A1).

### Canal 2 — Informe de sugerencias académicas (se sugiere, no se aplica)
- **A-01 (ACA-01 · afirmación excesiva/objetividad):** "demuestra claramente que el Fármaco X causa
  hemorragia" excede un único ensayo (18/20) y vulnera la **objetividad** [ES1]. Reformulación acotada a la
  muestra y cautelosa: *"En esta muestra, se observó hemorragia en la mayoría de los pacientes, lo cual
  podría indicar un problema de seguridad que requiere más investigación."* *(cambia la fuerza de la
  afirmación — lo decide el autor)*
- **A-02 (HUM-05 / ACA-02 · atribución vaga):** "Los estudios muestran que este es un hallazgo importante"
  sin cita — cite estudios específicos, matice o elimine. *(nunca se inventa una referencia — AIP-3)*

### Consentimiento del autor
`consent_to_apply = otorgado`, aceptado: **A-01, A-02** (el autor decide **eliminar** la oración sin cita);
`authorship_acknowledgement = confirmado`.

### Canal 3 — Revisión académica aprobada por el autor (aplicada + humanizada)
> "El estudio examina la relación entre el Fármaco X y la hemorragia. En el ensayo, se observó hemorragia en
> **18** de **20** pacientes (véase la **Tabla 2**), lo cual podría indicar un problema de seguridad que
> requiere más investigación, y es consistente con Almeida et al. **[7]**."

### Registro de revisión (INV-A10)
**Encabezado:** `es` · `journal`/`journal` · `apply_approved_notes` · `co_authored=false` ·
`ai_disclosure_policy=required` → se incluyó la declaración de uso de IA · aceptado: `A-01, A-02` ·
`authorship_acknowledgement=confirmado`.

| change_id | ubicación | canal | elemento aprobado | antes → después | motivo | comprobación de invariante |
|-----------|-----------|:-----:|-------------------|-----------------|--------|----------------------------|
| C-001 | Discusión ¶ | C.3 | A-01 | "demuestra claramente … causa hemorragia … se observó hemorragia en 18 de 20 → El estudio examina la relación entre el Fármaco X y la hemorragia … podría indicar un problema de seguridad …" | el autor aceptó la reformulación acotada a la muestra (se eliminó la afirmación causal excesiva) | INV-A6: afirmación atenuada por decisión del autor; los números no cambiaron |
| C-002 | Discusión ¶ | C.3 | A-02 | "Los estudios muestran que este es un hallazgo importante. → *(eliminada)*" | el autor aceptó eliminar la atribución sin cita | INV-A2/A3: nada se inventó; eliminación por el autor |
| C-003 | Discusión ¶ | C.1 | — (ACA-04 · [ES1]) | "En nuestro ensayo, observamos → En el ensayo, se observó" | regla impersonal/pasiva-refleja con *se* (automático, se conserva el sentido) | INV-A6: sentido conservado |
| C-004 | Discusión ¶ | C.1 | — (HUM-01/18/25) | "En conclusión, nuestro innovador estudio … 😊 → El estudio …" | de-AI solo de expresión | INV-A6: sentido conservado |

**Fidelidad y declaración:** `18` → sin cambios · `20` → sin cambios · `Tabla 2` → sin cambios · `[7]` → sin
cambios. No se eliminó ninguna limitación científica; no se convirtió evidencia débil en una afirmación
fuerte sin un elemento aprobado. Declaración: se incluyó la declaración de uso de IA; sin afirmar
"indetectable". **La responsabilidad principal de la investigación recae en el autor**, y la autoridad final
en el director y el tribunal.

---

## Ejemplo 2 — Compuerta de consentimiento (**no** se otorga → sin Canal 3)

**Contrato:** `level=masters` · `programme_type=masters_thesis` · `edit_scope=language_clarity` ·
`co_authored=false` · `ai_disclosure_policy=unknown` · `output_language=es`.

**Entrada:**
> "Puedes ver claramente en la **Figura 3** que el modelo en realidad no funciona muy bien, lo que representa
> una limitación importante. La tasa de error fue del **12,4 %**."

### Canal 1 — Texto con lenguaje mejorado (automático, solo expresión)
> "La **Figura 3** muestra que el modelo en realidad no funciona muy bien, lo que representa una limitación
> importante. La tasa de error fue del **12,4 %**."

*Cambiado (solo expresión):* segunda persona "Puedes ver … en la Figura 3" → forma impersonal "La Figura 3
muestra" (ACA-04 · [ES1]). *Conservado:* el atenuador "en realidad" (eliminarlo refuerza la afirmación →
Canal 2); y **`12,4 %`** — carácter por carácter; el decimal con coma del español **no se modifica** (INV-A1).

### Canal 2 — Informe de sugerencias académicas (se sugiere)
- **B-01 (ACA-08 · descriptivo→crítico):** "no funciona muy bien" es evaluativo pero no está cuantificado más
  allá del 12,4 % — indique la comparación/umbral que hace que esta tasa sea "no buena".

### Consentimiento del autor
`consent_to_apply = no otorgado`.

### Resultado — no se produce el Canal 3
Se entregan los Canales 1 y 2 completos. **No hay Canal 3; no se aplicó ningún elemento de sugerencia; no se
produjo registro de revisión.** `12,4 %` no cambió. *(Declaración: `ai_disclosure_policy=unknown` → se ofrece
de todos modos una declaración consultiva; el silencio nunca es un resultado.)*

> **Prueba de la compuerta de consentimiento:** el elemento de nivel de pensamiento **B-01 no se aplicó**; los
> datos de entrada se conservaron carácter por carácter; **el Canal 3 se retuvo** porque no se cumplieron sus
> cinco condiciones (no se otorgó el consentimiento) — exactamente el comportamiento de la compuerta
> (Blueprint §11 G1).

---

*Skill reference — `es` worked examples (full parity with `before-after.md`: A-01+A-02, 4-row revision log),
source-grounded [ES1]. © 2026 Dr. Aladdin Ali / Aladdin Pertanian Internasional.*
