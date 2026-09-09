# Planificador de Horarios de Tecnologías de la Información

Organizador de horarios para la carrera de **Tecnología de la Información** (malla TIN-S 2023) de la
Universidad de Guayaquil.

Eliges materias de la malla, les asignas un paralelo, y se acomodan solas en un calendario semanal
que te avisa cuando dos clases se cruzan.

Es un solo archivo `index.html` sin dependencias ni build. Se abre en cualquier navegador.

---

## Advertencia sobre los datos

> Los **horarios, paralelos y docentes** precargados salen de fuentes filtradas del
> **Ciclo I 2026 – 2027**. Esta información cambia de un ciclo a otro: se reasignan docentes, se
> abren y se cierran paralelos, y se mueven horarios.
>
> **Verifica siempre contra el horario oficial del SIUG antes de matricularte.**

## Qué trae cargado

| | |
|---|---|
| Materias de la malla | 68 (10 semestres + componente de idiomas) |
| Paralelos con horario | 207, en 61 materias |
| Bloques de clase | 366 |
| Paralelos con docente | 200 de 207 |
| Docentes distintos | 59 |

De cada materia se guarda código, créditos, modalidad, requisitos y semestre. De cada paralelo,
la jornada (matutino / vespertino / nocturno), el aula, el docente y sus bloques de horario.

### Lo que no tiene horario

Siete materias no tienen paralelos porque no llevan horario fijo: Servicio Comunitario (727),
Prácticas Preprofesionales (827), Trabajo de Titulación (157) y los cuatro niveles de Inglés
(107 – 110). Esas se agregan a mano.

Otros siete paralelos tienen horario pero quedaron sin docente, porque no aparecen en el horario
de exámenes: `151/NO-10-8`, `156/NO-10-8`, `199/VE-1-17`, `621/NO-6-1`, `726/MA-7-4`,
`926/NO-9-1` y `927/NO-9-7`.

## Cómo se usa

1. **Malla** — buscas la materia o filtras por semestre, y haces clic en ella.
2. **Paralelos** — se abre la lista de paralelos disponibles con su horario, aula y docente.
   Filtras por jornada y eliges uno; se llena todo solo. También puedes escribirlo a mano.
3. **Calendario** — la materia aparece como un bloque de lunes a sábado, entre 07:00 y 22:00.
   Haz clic en un bloque para editarlo.

Si dos clases se superponen, los bloques se marcan en rojo con ⚠, aparece el detalle del cruce
arriba del calendario, y el contador de **Choques** deja de estar en cero.

Cada materia lleva una pastilla abajo que dice si es **PRESENCIAL** o **VIRTUAL** — que es
justamente donde suelen aparecer los cruces, porque los horarios virtuales se arman aparte de los
presenciales.

### Detalles

- **Se guarda solo.** El horario persiste entre sesiones; abierto desde el mismo navegador lo
  recuperás tal como lo dejaste.
- **Tema.** El botón de la barra superior cicla entre Auto (sigue al sistema), Claro y Oscuro.
- **Imprimir** saca solo el calendario y la advertencia, sin la barra lateral.

## De dónde salen los datos

| Dato | Fuente |
|---|---|
| Materias, códigos, créditos, requisitos, modalidad | Malla TIN-S 2023 (SIUG) |
| Paralelos, horarios, jornada, aula | Horarios filtrados del Ciclo I 2026 – 2027 |
| Docentes | Horario de exámenes del primer parcial, Ciclo I 2026 – 2027 |

Los PDFs de origen no se versionan (están en `.gitignore`): son documentos filtrados y los datos ya
quedaron transcritos dentro de `index.html`.

Los nombres de docentes están en mayúscula inicial tal como vienen de la fuente. El horario de
exámenes trae la mayoría sin tildes, y no se les inventaron: donde falta un acento, falta en el
original.
