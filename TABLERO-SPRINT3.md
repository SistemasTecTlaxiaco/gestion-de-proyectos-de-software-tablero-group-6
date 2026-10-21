# Tablero de Planificación del Sprint 3 en GitHub Projects

**Proyecto:** Plataforma comunitaria para la lengua materna de Santa María Cuquila (Open Hub Tec)
**Sprint:** 3 · **eduScrum Master:** Yaretzy Montesinos López
**Equipo:** Diego Ernesto López Vásquez · Elisa Sánchez Coronel · Yaretzy Montesinos López · Daisy Ortiz López

Este documento tiene todo lo que va en el tablero: la estructura, los campos, las etiquetas, las historias con su estimación, las tareas con su responsable y el texto de cada issue listo para copiar.

---

## 1. Estructura del tablero

### 1.1 Columnas (campo *Status*)

| Columna | Qué va aquí |
|---|---|
| **Backlog** | Historias de los siguientes periodos (HU-03 a HU-06) |
| **To Do** | Tareas del Sprint 3 que todavía no empiezan |
| **In Progress** | Tareas que alguien está trabajando |
| **Review** | Tareas terminadas que espera revisar otro integrante |
| **Done** | Tareas revisadas y aprobadas por el eduScrum Master |

### 1.2 Campos personalizados

| Campo | Tipo | Valores |
|---|---|---|
| Iteración | Iteration | Sprint 3 (semanas 12–16) · Sprint 4 · Siguiente periodo |
| Construcción (h) | Number | Horas para construir (estimación de tres puntos) |
| Prevención (h) | Number | Horas de prevención del Sprint 2 |
| Corrección (h) | Number | Horas de corrección del Sprint 2 |
| Estimación (h) | Number | Total = construcción + prevención + corrección |
| Costo (MXN) | Number | Estimación × $150 |
| Perfil | Single select | Desarrollo frontend · Contenido y enlace comunitario · Calidad (QA) · Gestión eduScrum |
| Tipo | Single select | Historia · Tarea · Reserva · Plan |

### 1.3 Etiquetas (*labels*)

| Etiqueta | Color sugerido | Uso |
|---|---|---|
| `sprint-3` | verde | Todo lo que se trabaja en este sprint |
| `historia-usuario` | azul | Los issues HU-01 a HU-06 |
| `tarea` | gris | Las tareas que salen de cada historia |
| `prevencion` | amarillo | Trabajo de prevención (horas del Sprint 2) |
| `construccion` | morado | Trabajo de construcción |
| `correccion` | naranja | Trabajo de corrección (horas del Sprint 2) |
| `reserva` | rojo | Reserva por riesgos |
| `backlog-futuro` | blanco | Historias fuera del Sprint 3 |

### 1.4 Vistas

1. **Kanban**: vista *Board* agrupada por Status.
2. **Estimación**: vista *Table* agrupada por Iteración, con la suma de los campos numéricos activada.
3. **Carga del equipo**: vista *Table* agrupada por *Assignees*, con suma de Estimación (h).

---

## 2. Vinculación con el Costo de la Calidad del Sprint 2 (criterio 1)

Las horas de **prevención y corrección se copian tal cual** de `COSTO-CALIDAD-HISTORIAS.md` del Sprint 2. Solo la construcción es nueva y se estima con tres casos:

> Construcción = (Bien + Normal × 4 + Falla) ÷ 6

| HU | Bien | Normal | Falla | Construcción | Prevención (S2) | Corrección (S2) | j (S2) | **Estimación** |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| HU-01 Consultar palabras y expresiones | 10 | 16 | 28 | 17 | 4 | 3 | 1.33 | **24 h** |
| HU-02 Escuchar pronunciaciones | 8 | 12 | 16 | 12 | 5 | 5 | 1.00 | **22 h** |
| HU-03 Aportar conocimiento | 12 | 20 | 34 | 21 | 6 | 8 | 0.75 | **35 h** |
| HU-04 Consultar memoria cultural | 9 | 14 | 25 | 15 | 6 | 7 | 0.86 | **28 h** |
| HU-05 Validar contenido | 12 | 18 | 30 | 19 | 5 | 6 | 0.83 | **30 h** |
| HU-06 Pronunciación asociada al término | 4 | 8 | 12 | 8 | 4 | 5 | 0.80 | **17 h** |
| **Total** | | | | **92** | **30** | **34** | **0.88** | **156 h** |

### Cómo usa el tablero los datos del Sprint 2

- **Selección del Sprint 3.** Entran HU-01 y HU-02 porque son las únicas con j ≥ 1.00, es decir, con más prevención que corrección y menos riesgo de retrabajo.
- **Prevención primero.** En el Sprint 3, las tareas de prevención (T1 y T6) están en la primera semana. Así se atiende la recomendación del Sprint 2 de *"diseñar casos de prueba antes del desarrollo"*.
- **Historias con j < 1.** HU-03 a HU-06 quedan en el backlog con una nota: antes de construirlas hay que subir su prevención (recomendación del Plan de Calidad, sección 8).
- **Evaluación.** Las horas de evaluación del Sprint 2 (2 y 3 h por historia) se incluyen en la construcción porque son las pruebas funcionales de cada historia.

---

## 3. Estimaciones de tiempo y costo por historia (criterio 2)

**Supuestos:**
- Tarifa de $150 MXN por hora, la misma del Sprint 2.
- 4 personas × 5 h × 75 % = 15 h por semana.
- Reserva del 15 %, por dos riesgos altos: R1 (pocos hablantes disponibles) y R2 (falla de conectividad en Cuquila).

### 3.1 Por historia

| HU | Estimación | Semanas (÷ 15 h) | Trabajo ($150/h) | Insumos | **Costo total** | Iteración |
|---|---:|---:|---:|---|---:|---|
| HU-01 | 24 h | 1.6 | $3,600 | Datos móviles $100 | **$3,700** | Sprint 3 |
| HU-02 | 22 h | 1.5 | $3,300 | Pasajes $400 + datos $100 | **$3,800** | Sprint 3 |
| HU-03 | 35 h | 2.3 | $5,250 | Pasajes $200 + datos $100 | **$5,550** | Siguiente periodo |
| HU-04 | 28 h | 1.9 | $4,200 | Pasajes $200 + datos $100 | **$4,500** | Siguiente periodo |
| HU-05 | 30 h | 2.0 | $4,500 | Pasajes $200 + datos $100 | **$4,800** | Sprint 4 / siguiente periodo |
| HU-06 | 17 h | 1.1 | $2,550 | Pasajes $200 + datos $100 | **$2,850** | Sprint 4 / siguiente periodo |

Pasajes: visitas a Cuquila de 4 personas a $50 ida y vuelta, es decir, $200 por visita.

### 3.2 Por iteración

| Iteración | Historias | Horas | Reserva 15 % | Total | Semanas | Costo |
|---|---|---:|---:|---:|---:|---:|
| **Sprint 3** | HU-01, HU-02 | 46 h | 7 h | **53 h** | 3.5 | **$8,550** |
| Sprint 4 / siguiente | HU-05, HU-06 | 47 h | 7 h | 54 h | 3.6 | $8,700 |
| Siguiente periodo | HU-03, HU-04 | 63 h | 9 h | 72 h | 4.8 | $11,400 |
| **Total del backlog** | 6 historias | 156 h | 23 h | **179 h** | 11.9 | **$28,650** |

El costo del Sprint 3 se calcula así: 53 h × $150 = $7,950, más $600 de insumos (pasajes $400 y datos $200), igual a **$8,550**.

El Sprint 3 tiene 75 h disponibles (semanas 12 a 16). Las 53 h caben y **sobran 22 h**.

---

## 4. Personal requerido y carga de trabajo (criterio 3)

### 4.1 Perfiles que necesita el proyecto

| Perfil | Qué hace | Conocimientos | Asignado a |
|---|---|---|---|
| **Desarrollo frontend (búsqueda y sin conexión)** | Búsqueda, modo sin conexión y corrección de defectos de HU-01 | HTML, CSS, JavaScript, *service workers*, JSON | Diego Ernesto López Vásquez |
| **Desarrollo frontend (interfaz y audio)** | Ficha de palabra, reproductor y accesibilidad | HTML, CSS, JavaScript, audio HTML5, WCAG 2.2 | Daisy Ortiz López |
| **Contenido y enlace comunitario** | Captura de palabras, grabación y compresión de audios, coordinación con el Comité | Trabajo de campo, edición de audio, trato con la comunidad | Elisa Sánchez Coronel |
| **Calidad (QA) y gestión eduScrum** | Casos de prueba, pruebas de conectividad, tablero y seguimiento | Diseño de pruebas, ISO/IEC 25010, GitHub Projects | Yaretzy Montesinos López (eduScrum Master) |

Cada perfil coincide con el rol del equipo en `ACUERDO.md`:
- Elisa es la investigadora, así que trabaja el contenido.
- Yaretzy es la documentadora y eduScrum Master del Sprint 3, así que lleva calidad y el tablero.
- Daisy es la responsable del Backlog y Diego coordinó el Sprint 1; los dos llevan el desarrollo.

### 4.2 Tareas del Sprint 3

| ID | Tarea | HU | Tipo | Horas | Perfil | Responsable | Revisor | Semana |
|---|---|---|---|---:|---|---|---|---|
| T1 | Casos de prueba de búsqueda (existente, inexistente, variantes de escritura) | HU-01 | Prevención | 4 | QA | Yaretzy | Diego | 12 |
| T2 | Estructura de datos JSON y carga de 100 palabras validadas por el Comité | HU-01 | Construcción | 5 | Contenido | Elisa | Daisy | 12 |
| T3 | Búsqueda que ignora tildes y acepta variantes de escritura | HU-01 | Construcción | 7 | Frontend | Diego | Yaretzy | 12–13 |
| T4 | Ficha de palabra: palabra, significado, fuente y fecha | HU-01 | Construcción | 5 | Frontend | Daisy | Elisa | 13 |
| T5 | Corrección de defectos de HU-01 | HU-01 | Corrección | 3 | Frontend | Diego | Yaretzy | 14 |
| T6 | Casos de prueba de audio y de conexión limitada | HU-02 | Prevención | 5 | QA | Yaretzy | Daisy | 12 |
| T7 | Grabación en campo y compresión de 50 audios (Opus o MP3 de 32 kbps) | HU-02 | Construcción | 5 | Contenido | Elisa | Yaretzy | 12–13 |
| T8 | Reproductor con término visible, fuente y fecha del audio | HU-02 | Construcción | 4 | Frontend | Daisy | Diego | 13 |
| T9 | Modo sin conexión con paquete de contenido descargable | HU-02 | Construcción | 3 | Frontend | Diego | Daisy | 14 |
| T10 | Corrección de defectos del reproductor y del modo sin conexión | HU-02 | Corrección | 3 | Frontend | Daisy | Diego | 14–15 |
| T11 | Corrección de audios: volver a grabar o comprimir los que fallen | HU-02 | Corrección | 2 | Contenido | Elisa | Yaretzy | 14–15 |
| R1 | Reserva por riesgos (15 %) | — | Reserva | 7 | Todos | Yaretzy (administra) | — | 15–16 |
| | **Total** | | | **53 h** | | | | |

Comprobación de horas:
- **HU-01:** 4 + 5 + 7 + 5 + 3 = **24 h**, que coincide con la estimación.
- **HU-02:** 5 + 5 + 4 + 3 + 3 + 2 = **22 h**, que coincide con la estimación.

### 4.3 Carga por integrante

| Integrante | Tareas | Horas asignadas | Reserva asignada | **Total** | Capacidad del sprint* | Uso |
|---|---|---:|---:|---:|---:|---:|
| Diego | T3, T5, T9 | 13 | 1 | **14 h** | 18.75 h | 75 % |
| Daisy | T4, T8, T10 | 12 | 1 | **13 h** | 18.75 h | 69 % |
| Elisa | T2, T7, T11 | 12 | 1 | **13 h** | 18.75 h | 69 % |
| Yaretzy | T1, T6, más la gestión del tablero | 9 | 4 | **13 h** | 18.75 h | 69 % |
| **Equipo** | | **46** | **7** | **53 h** | **75 h** | **71 %** |

\* Capacidad del sprint = 5 h por semana × 75 % × 5 semanas = 18.75 h por persona.

Con esta asignación nadie pasa del 75 % de su capacidad y la diferencia entre quien más y quien menos carga es de 1 h. Yaretzy tiene menos horas de tareas porque como eduScrum Master también coordina el tablero, las reuniones y las revisiones. Por eso administra la mayor parte de la reserva.

---

## 5. Operación del tablero (criterio 4)

### 5.1 Reglas de flujo

1. Cada tarea entra en **To Do** con responsable, perfil, horas e iteración.
2. Quien la toma la mueve a **In Progress**. Nadie tiene más de 2 tareas en progreso al mismo tiempo.
3. Al terminar, la mueve a **Review** y menciona en un comentario a su revisor.
4. El revisor comprueba los criterios de aceptación de la historia y deja su visto bueno en un comentario.
5. Solo la **eduScrum Master** mueve la tarea a **Done**.
6. Cuando se usan horas de la reserva, se anota en el issue R1 cuántas horas, en qué tarea y por qué riesgo.

### 5.2 Seguimiento de la eduScrum Master

- Revisa el tablero al inicio de cada sesión: qué se hizo, qué sigue y qué bloquea.
- Actualiza la vista **Estimación**: si una tarea pasa de sus horas, se registra en el issue de la tarea.
- Al cierre del sprint compara las horas estimadas con las reales y el j real contra la meta j ≥ 1.00.

---

## 6. Texto de los issues (para copiar y pegar)

### Issue: HU-01 Consultar palabras y expresiones

**Etiquetas:** `historia-usuario`, `sprint-3` · **Iteración:** Sprint 3 · **Status:** To Do
**Campos:** Construcción 17 · Prevención 4 · Corrección 3 · Estimación 24 · Costo 3700 · Tipo: Historia

```markdown
## Historia
Como habitante de Santa María Cuquila, quiero consultar palabras y expresiones de la lengua materna, para conocer su significado y conservar parte del conocimiento lingüístico de la comunidad.

**Dictamen del cliente (Acta):** Aceptado

## Criterios de aceptación
- [ ] El usuario puede buscar palabras o expresiones.
- [ ] El sistema muestra el significado registrado.
- [ ] El sistema permite consultar información relacionada con la palabra.
- [ ] La información muestra su origen o fuente.
- [ ] El contenido puede ser consultado desde una interfaz sencilla.
- [ ] El sistema informa cuando una palabra no se encuentra registrada.

## Estimación
| Construcción (10 / 16 / 28) | Prevención (S2) | Corrección (S2) | Total | Costo |
|---|---|---|---|---|
| 17 h | 4 h | 3 h | **24 h** | 24 × $150 + $100 datos = **$3,700** |

j del Sprint 2 = 4 / 3 = 1.33

## Tareas
- [ ] T1 Casos de prueba de búsqueda · 4 h · @Yaretzy
- [ ] T2 Estructura JSON y carga de 100 palabras · 5 h · @Elisa
- [ ] T3 Búsqueda tolerante a variantes · 7 h · @Diego
- [ ] T4 Ficha de palabra · 5 h · @Daisy
- [ ] T5 Corrección de defectos · 3 h · @Diego
```

### Issue: HU-02 Escuchar pronunciaciones

**Etiquetas:** `historia-usuario`, `sprint-3` · **Iteración:** Sprint 3 · **Status:** To Do
**Campos:** Construcción 12 · Prevención 5 · Corrección 5 · Estimación 22 · Costo 3800 · Tipo: Historia

```markdown
## Historia
Como habitante de Santa María Cuquila, quiero escuchar la pronunciación de las palabras y expresiones registradas, para aprender o recordar la manera correcta de pronunciarlas.

**Dictamen del cliente (Acta):** Modificado. Se agregó el criterio de fuente y fecha del audio.

## Criterios de aceptación
- [ ] El usuario puede reproducir una grabación.
- [ ] La grabación corresponde a la palabra consultada.
- [ ] El usuario puede iniciar y detener la reproducción.
- [ ] Se identifica la palabra asociada con el audio.
- [ ] El sistema informa cuando una palabra todavía no tiene pronunciación disponible.
- [ ] El registro de pronunciación conserva su fuente y fecha de registro.

## Estimación
| Construcción (8 / 12 / 16) | Prevención (S2) | Corrección (S2) | Total | Costo |
|---|---|---|---|---|
| 12 h | 5 h | 5 h | **22 h** | 22 × $150 + $400 pasajes + $100 datos = **$3,800** |

j del Sprint 2 = 5 / 5 = 1.00

## Tareas
- [ ] T6 Casos de prueba de audio y conexión limitada · 5 h · @Yaretzy
- [ ] T7 Grabación y compresión de 50 audios · 5 h · @Elisa
- [ ] T8 Reproductor con término, fuente y fecha · 4 h · @Daisy
- [ ] T9 Modo sin conexión · 3 h · @Diego
- [ ] T10 Corrección de reproductor y modo sin conexión · 3 h · @Daisy
- [ ] T11 Corrección de audios · 2 h · @Elisa
```

### Issues HU-03 a HU-06 (Backlog)

**Etiquetas:** `historia-usuario`, `backlog-futuro` · **Status:** Backlog. Usen la misma plantilla con estos datos:

| Issue | Historia (del Acta) | Construcción (B / N / F) | Prev. | Corr. | Total | Costo | Nota |
|---|---|---|---:|---:|---:|---:|---|
| HU-03 Aportar conocimiento | Como integrante de la comunidad, quiero aportar palabras, expresiones y conocimientos culturales, para contribuir a preservar el conocimiento de Santa María Cuquila. | 21 (12 / 20 / 34) | 6 | 8 | 35 h | $5,550 | j = 0.75. Subir prevención antes de construir |
| HU-04 Consultar memoria cultural | Como habitante de Santa María Cuquila, quiero consultar información sobre la memoria cultural de la comunidad, para conocer y preservar conocimientos que forman parte de su identidad. | 15 (9 / 14 / 25) | 6 | 7 | 28 h | $4,500 | j = 0.86. Agregar contexto, fuente y fecha (Acta) |
| HU-05 Validar contenido | Como persona responsable de revisar contenidos comunitarios, quiero validar las aportaciones antes de su publicación, para ayudar a mantener información correcta y confiable. | 19 (12 / 18 / 30) | 5 | 6 | 30 h | $4,800 | j = 0.83. Mientras no exista, el Comité valida fuera de la plataforma |
| HU-06 Pronunciación asociada al término | Como usuario de la plataforma, quiero escuchar pronunciaciones asociadas a las palabras registradas, para mejorar mi aprendizaje de la lengua materna. | 8 (4 / 8 / 12) | 4 | 5 | 17 h | $2,850 | j = 0.80. Reutiliza el reproductor de HU-02 |

Copien los criterios de aceptación de cada historia del Acta, secciones 7 a 10.

### Issue: T1 a T11 (una por tarea)

**Etiquetas:** `tarea`, `sprint-3`, y según el tipo `prevencion`, `construccion` o `correccion`
**Campos:** Estimación (h), Perfil, Tipo: Tarea, Iteración: Sprint 3 · **Assignee:** el responsable de la tabla 4.2

```markdown
**Historia:** #<número del issue HU>
**Tipo:** Prevención / Construcción / Corrección
**Horas estimadas:** __ h · **Perfil:** __ · **Revisor:** @__

## Qué hay que hacer
<descripción de la tarea de la tabla 4.2>

## Listo cuando
- [ ] Cumple los criterios de aceptación de la historia que le corresponden
- [ ] Lo revisó @__ (comentario de visto bueno)
- [ ] Horas reales anotadas: __ h
```

### Issue: R1 [PLAN] Reserva por riesgos (15 %)

**Etiquetas:** `reserva`, `sprint-3` · **Assignee:** Yaretzy · **Campos:** Estimación 7 · Costo 1050 · Tipo: Reserva

```markdown
Reserva de 7 h (46 h × 15 %), justificada por dos riesgos altos:
- R1: pocos hablantes disponibles para grabar (temporada agrícola).
- R2: falla de conectividad en Cuquila durante las pruebas.

Asignación preliminar: Yaretzy 4 h · Diego 1 h · Daisy 1 h · Elisa 1 h

## Uso de la reserva
| Fecha | Tarea | Horas | Riesgo | Quién |
|---|---|---|---|---|
```

### Issue: [PLAN] Estimación de tiempo y costo

**Etiquetas:** `sprint-3` · **Assignee:** Yaretzy · **Tipo:** Plan
Copien la tabla 3.2, el resumen de capacidad, la carga por integrante (4.3) y los supuestos de la sección 3.

---

## 7. Lista de verificación antes de entregar

- [ ] Las 5 columnas: Backlog, To Do, In Progress, Review y Done
- [ ] Los 8 campos personalizados creados
- [ ] Las etiquetas creadas, con `sprint-3` en todo lo del sprint
- [ ] Issues HU-01 a HU-06 con sus criterios de aceptación y campos llenos
- [ ] Issues T1 a T11 con responsable, perfil y horas
- [ ] Issue de la reserva y issue [PLAN]
- [ ] Vista Estimación agrupada por Iteración, con la suma mostrando **53 h** en el Sprint 3
- [ ] Vista Carga del equipo agrupada por *Assignees*
- [ ] Al menos un movimiento real de tarjetas (por ejemplo T1 y T6 en In Progress) para mostrar que el tablero se usa
