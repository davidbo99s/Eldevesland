# Sistema de Medicina

El médico de campo no es simplemente quien usa el kit de sanador cuando alguien cae. Es quien conoce las condiciones del cuerpo, aplica tratamientos con técnica y puede, en el momento crítico, salvar una vida que los hechizos de curación no alcanzaron. Este sistema desarrolla la medicina como una disciplina profunda, complementaria pero no subordinada a la magia.

---

## Herramientas y Requisitos

- **Kit de Sanador**: La herramienta básica. Incluye vendas, agujas, hilo, antisépticos naturales, tablillas, y medicamentos simples. Cada kit tiene **10 usos** antes de agotarse. Costo: 5 po.
- **Kit Médico Avanzado**: Kit mejorado con instrumentos quirúrgicos básicos, suturas de calidad, ampolla antiséptica concentrada y un manual de anatomía. 20 usos. Costo: 50 po.
- **Proficiencia en Kit de Sanador**: Necesaria para realizar cualquier procedimiento médico más allá de estabilizar a alguien.
- **Habilidades relevantes**: Medicina (primaria), Naturaleza (identificar causas naturales), Percepción (diagnosticar), Manos Firmes (Destreza para cirugía).

---

## Mecánicas Generales

### La Tirada de Medicina

Todas las acciones médicas relevantes se resuelven con **Medicina + Sabiduría** o, para procedimientos quirúrgicos, con **Medicina + Destreza**. El DM puede permitir usar Inteligencia en situaciones académicas o de diagnóstico puro.

### Categorías de Atención Médica

| Categoría | Descripción | Requiere |
|---|---|---|
| Estabilización | Llevar a 0 HP a condición estable | Acción, sin tirada (kit de sanador) |
| Primeros Auxilios | Tratamiento inmediato post-combate | Tirada Medicina DC 10 |
| Tratamiento | Curar condiciones específicas | Tirada variable |
| Cirugía | Procedimientos invasivos | Tirada Medicina (Des) DC variable |
| Diagnóstico | Identificar enfermedades, venenos, condiciones | Tirada Medicina DC variable |
| Atención Prolongada | Recuperación acelerada | Descanso + tiradas diarias |

---

## Estabilización y Primeros Auxilios

### Estabilizar (Regla Estándar Modificada)

- Acción completa. Sin tirada con **Kit de Sanador** (consume 1 uso).
- Sin kit: Tirada de Medicina DC 10.
- La criatura estabilizada queda en 0 HP pero no hace tiradas de muerte.

### Primeros Auxilios Post-Combate

Administrado dentro de los **10 minutos** tras el combate:

- **DC 10**: La criatura recupera 1 dado de vida inmediatamente (sin descanso).
- **DC 14**: La criatura recupera 2 dados de vida.
- **DC 18**: La criatura recupera 3 dados de vida y el médico puede tratar también una condición menor (ver sección de condiciones).

Cada personaje puede recibir primeros auxilios **una sola vez** por combate.

---

## Diagnóstico

El diagnóstico es el primer paso en cualquier tratamiento desconocido.

### Examinar a un Paciente

**Acción**: 5-10 minutos de examinación física y conversación.
**Tirada**: Medicina DC variable.

| DC | Qué se puede diagnosticar |
|---|---|
| 10 | Heridas físicas obvias, fiebre, traumatismo |
| 13 | Envenenamiento genérico, infección, fractura |
| 16 | Tipo específico de veneno, enfermedad identificada |
| 19 | Enfermedad exótica, maldición física, condición mágica con síntomas físicos |
| 22 | Patología rarísima, efecto de plano alternativo, maldición disfrazada |

- Un fallo **no dice nada**. Un fallo crítico puede confundir dos condiciones.
- Con herramientas especializadas (+kit médico avanzado): +2 a la tirada.
- Con acceso a biblioteca médica o manual de anatomía: +2 a la tirada.

---

## Tratamiento de Condiciones

### Curar Condiciones Físicas

Las siguientes condiciones pueden tratarse médicamente, sin magia:

#### Envenenado
- **DC de tratamiento**: Varía según el veneno (ver tabla abajo).
- **Tiempo**: 10 minutos.
- **Insumos**: Kit de Sanador (1 uso) + posible antídoto del [[Sistema de Herbolario|herbolario]].
- **Efecto en éxito**: Se reduce la DC de las TS contra el veneno en 5, o se elimina si el veneno era de bajo nivel.

| Nivel de Veneno | DC de Tratamiento |
|---|---|
| Débil (DC 10-12) | DC 13 |
| Moderado (DC 13-15) | DC 15 |
| Fuerte (DC 16-18) | DC 18 |
| Letal (DC 19+) | DC 21 |

#### Herida Sangrante (Condición Homebrew)
Si un personaje recibió un golpe crítico o un ataque dirigido que causó hemorragia, pierde 1d4 HP al inicio de cada turno hasta que se trate.

- **DC de tratamiento**: DC 12.
- **Tiempo**: 1 acción en combate o 2 minutos fuera de combate.
- **Insumos**: Kit de Sanador (1 uso).
- **En combate**: El médico puede gastar su acción para tratar al paciente adyacente. El paciente debe estar estable y no puede atacar en el mismo turno.

#### Fractura
- **DC de tratamiento**: DC 14 (inmovilizar y entablillar).
- **Tiempo**: 30 minutos.
- **Insumos**: Kit de Sanador (2 usos), tablillas.
- **Efecto**: Con tratamiento, el personaje recupera la funcionalidad completa tras 2 semanas. Sin tratamiento: la fractura puede complicarse o sanar mal (desventaja permanente en el miembro afectado hasta tratarla).

#### Quemaduras
- **Leves** (1d6 de daño): DC 10, 1 uso de kit. Sin efecto secundario.
- **Moderadas** (2d6-3d6): DC 14, 2 usos. Sin tratar: desventaja en pruebas físicas del área quemada.
- **Graves** (4d6+): DC 18, 3 usos. Sin tratar: cicatriza mal, penalización permanente hasta cirugía o magia.

#### Agotamiento por Frío o Calor
- **DC de tratamiento**: DC 12.
- **Tiempo**: 1 hora de atención.
- **Efecto**: Elimina 1 nivel de Agotamiento adquirido por exposición ambiental. Solo funciona si el paciente está en condiciones de temperatura adecuada.

---

## Enfermedades

Las enfermedades siguen el esquema estándar de D&D pero con el siguiente sistema médico superpuesto:

### Identificar una Enfermedad
- **DC**: Medicina DC 13-20 según la enfermedad.
- Sin identificar: el médico trata síntomas pero no la causa. El paciente puede empeorar.
- Identificada: el médico sabe qué tratamiento aplicar.

### Tratar una Enfermedad Activamente

Cada día que el médico trate al paciente:

1. El médico hace una tirada de **Medicina DC según la enfermedad**.
2. El paciente hace su **TS de Constitución** con ventaja si el médico tuvo éxito.
3. Si el paciente falla aun con ventaja, la enfermedad **no avanza** (en vez de empeorar, que es lo normal sin tratamiento).

### Enfermedades Comunes

#### Fiebre de Río
- **Fuente**: Agua contaminada, mordeduras de ciertos insectos.
- **DC de diagnóstico**: 13.
- **DC de TS del paciente**: Constitución DC 12.
- **Síntomas**: 1 nivel de Agotamiento cada 24h hasta TS exitosa. Delirio en fase avanzada.
- **Tratamiento médico**: DC 13. Con éxito: ventaja en TS. Con ingredientes de herbolario (Diente de León, Menta): DC se reduce a 10.
- **Duración sin tratamiento**: 1d6 días hasta curarse espontáneamente (o muerte si llega a 6 niveles de Agotamiento).

#### Plaga Roja
- **Fuente**: Contacto con cadáveres infectados, mordedura de ratas.
- **DC de diagnóstico**: 16.
- **DC de TS del paciente**: Constitución DC 15.
- **Síntomas**: 1d4 puntos de daño de Constitución cada 48h. El paciente se ve rojo, pustuloso.
- **Tratamiento médico**: DC 17. Requiere Kit Médico Avanzado. Con componentes herbolarios específicos (Espina de Zarzamora Plateada + Hongo de Madera): +3 a la tirada médica.
- **Contagio**: Quien trate al paciente sin guantes o protección hace TS Constitución DC 12.

#### Mal del Hueso Gris
- **Fuente**: Magia necrótica residual, zonas de alta presencia de no muertos.
- **DC de diagnóstico**: 18.
- **DC de TS del paciente**: Constitución DC 16.
- **Síntomas**: Los huesos se vuelven frágiles. -2 a Fuerza y Constitución. Fractura automática con cualquier crítico recibido.
- **Tratamiento médico**: DC 18. Requiere componentes mágicos de origen divino o herbolario raro (Raíz de Corazón del Árbol). Tratamiento médico puro solo detiene la progresión; curar requiere también intervención mágica o herbolaria especializada.

#### Pulmón de Tormenta
- **Fuente**: Exposición a tormentas mágicas, zonas de alta electricidad.
- **DC de diagnóstico**: 15.
- **Síntomas**: Tos constante. -1 a tiradas de Concentración por ruido de tos. 1 nivel de Agotamiento tras cada combate.
- **Tratamiento**: DC 14. Con extractos de Musgo Durmiente (reduce inflamación): DC 12. Recuperación: 3 días de reposo y tratamiento.

---

## Cirugía

La cirugía representa intervenciones invasivas: extraer proyectiles, reparar órganos internos, amputar un miembro gangrenado, o retirar un parásito mágico.

### Condiciones para Operar

1. **El paciente debe estar inconsciente o anestesiado**: Con Musgo Durmiente (ver [[Sistema de Herbolario|herbolario]]) o con magia de sueño.
2. **Entorno adecuado**: Mesa o superficie plana, luz suficiente, instrumentos limpios. Sin entorno: +4 al DC.
3. **Asistente** (recomendado): Otro personaje puede asistir. Si tiene proficiencia en Medicina: +2 a la tirada del cirujano.
4. **Kit Médico Avanzado**: Obligatorio para cirugías de DC 15 o más. Sin él: solo procedimientos simples.

### Procedimientos Quirúrgicos

#### Extracción de Proyectil
- **Descripción**: Retirar una flecha, bala de ballesta, fragmento de piedra, etc.
- **DC**: 13
- **Tiempo**: 30 minutos
- **Insumos**: Kit de Sanador (2 usos)
- **En éxito**: El paciente recupera 1d6 HP y elimina cualquier penalización de movimiento por el proyectil.
- **En fallo**: El daño queda pero el proyectil se extrae. En fallo crítico: 1d6 de daño adicional por complicaciones.

#### Sutura Interna
- **Descripción**: Reparar hemorragia interna, suturar órgano dañado.
- **DC**: 17
- **Tiempo**: 1 hora
- **Insumos**: Kit Médico Avanzado (2 usos)
- **En éxito**: Detiene hemorragia interna (que sin intervención causaría 1d6 daño/hora). El paciente necesita 1 semana de reposo.
- **En fallo**: La hemorragia continúa. Reintentarlo añade +2 al DC por el deterioro del tejido.

#### Amputación Controlada
- **Descripción**: Retirar un miembro gravemente dañado, gangrenado, o maldito que no puede recuperarse.
- **DC**: 15
- **Tiempo**: 1 hora
- **Insumos**: Kit Médico Avanzado (3 usos), vendas de compresión
- **En éxito**: El miembro se retira sin infección. El paciente necesita 2 semanas de recuperación. Sin prótesis, el miembro permanece ausente (efectos mecánicos según el miembro perdido).
- **En fallo**: La herida se infecta. Constitución DC 14 o el paciente gana la condición Envenenado por infección.

#### Extracción de Parásito Mágico
- **Descripción**: Retirar un huevo de criatura mágica, un parásito planar, una espora de hongo mágico.
- **DC**: 19
- **Tiempo**: 2 horas
- **Insumos**: Kit Médico Avanzado (3 usos) + posible componente herbolario específico
- **En éxito**: El parásito se extrae sin dañar al paciente.
- **En fallo**: El procedimiento falla. Si el fallo es por 5 o más, el parásito reacciona (efectos a discreción del DM, posiblemente un nuevo peligro).

---

## Atención Prolongada

Cuando un personaje está gravemente herido, enfermo, o recuperándose de cirugía, puede beneficiarse de atención médica continua.

### Proceso

1. El médico dedica **8 horas al día** a la atención del paciente.
2. Al inicio de cada día, el médico hace **Medicina DC 12**.
3. **En éxito**: El paciente recupera el **doble** de dados de vida durante ese descanso largo.
4. **En éxito por 5+**: El paciente también recupera 1 punto de Constitución si la enfermedad lo había reducido, o acelera su recuperación post-cirugía en 1 día.
5. **En fallo**: Recuperación normal sin bono.

El médico que cuida a otro **no puede** a su vez beneficiarse de atención médica ese día.

---

## Medicamentos

El médico puede preparar medicamentos con insumos de herbolario o comprarlos en tiendas de alquimia. Algunos ejemplos:

| Medicamento | Fuente | Efecto | Costo aproximado |
|---|---|---|---|
| Antiséptico de Zarzamora | Herbolario (Espina de Zarzamora Plateada) | Previene infección post-cirugía | Elaborado o 3 po |
| Sedante de Campo | Herbolario (Musgo Durmiente) | Anestesia para cirugía 1-2h | Elaborado o 5 po |
| Fijador de Fractura | Compra | +2 a tirada de tratamiento de fractura | 10 po |
| Antídoto Genérico | Herbolario o compra | Ventaja en TS contra venenos débiles | Elaborado o 50 po |
| Tónico Vital | Herbolario avanzado | Recupera 2d6 HP, no cuenta como acción mágica | 100+ po o receta rara |

---

## Límites de la Medicina vs. la Magia

La medicina mundana y la magia curativa son complementarias, no equivalentes:

| Situación | Medicina | Magia |
|---|---|---|
| Estabilizar a 0 HP | Sí (con kit) | Sí (hechizo) |
| Curar HP | Indirecto (dados de vida) | Directo |
| Tratar enfermedades | Sí, proceso largo | Sí (Curar Enfermedades) |
| Curar veneno | Sí, requiere identificar el tipo | Sí (Neutralizar Veneno) |
| Reparar pérdida de miembro | Solo amputar si gangrenado | Regenerar (nivel alto) |
| Tratar maldiciones físicas | Solo paliar síntomas | Disipar Magia, Eliminar Maldición |
| Devolver a alguien de la muerte | No | Revivir, Resurrección |

Un médico experto **puede reemplazar parcialmente** el gasto de recursos mágicos en campañas donde los sanadores escasean. Esto es intencional.

---

## Ética Médica y Rol

El sistema de medicina se presta a momentos narrativos profundos:

- **Dilema de recursos**: El kit tiene usos limitados. ¿A quién tratas primero?
- **Información de diagnóstico**: El médico puede descubrir secretos del cuerpo del paciente (cicatrices ocultas, marcas de ritual, señales de abuso antiguo).
- **Reputación médica**: Un médico reconocido puede ser buscado por nobles, ejércitos o facciones. También puede ser objetivo si se descubre que ha tratado al "enemigo".
- **Medicina gris**: Los mismos conocimientos que curan pueden matar. El médico conoce dosis letales, sedantes controlados y puntos vulnerables anatómicos.
