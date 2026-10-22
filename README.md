# Planificador de Horarios de Tecnologías de la Información

Organizador de horarios para la carrera de **Tecnología de la Información** (malla TIN-S 2023) de la
Universidad de Guayaquil.

Eliges materias de la malla, les asignas un paralelo, y se acomodan solas en un calendario semanal
que te avisa cuando dos clases se cruzan.

Es un solo archivo `index.html` sin dependencias ni build. Se abre en cualquier navegador.

---

## Advertencia sobre los datos

> Los **horarios, paralelos, aulas y docentes** son una copia del SIUG del **Ciclo II 2026 – 2027**
> (Consulta de planificación académica → Ver detalle de los horarios, niveles 1 al 10), tomada el
> 21 de octubre de 2026. El SIUG cambia durante el ciclo: se reasignan docentes, se abren y cierran
> paralelos, y se mueven horarios y aulas.
>
> **Verifica siempre contra el horario oficial del SIUG antes de matricularte.**

## Qué trae cargado

| | |
|---|---|
| Materias de la malla | 68 (10 semestres + componente de idiomas) |
| Paralelos con horario | 195, en 61 materias |
| Bloques de clase | 336 |
| Paralelos con docente | 195 de 195 |

De cada materia se guarda código, créditos, modalidad, requisitos y semestre. De cada paralelo,
la jornada (matutino / vespertino / nocturno), el aula, el docente y sus bloques de horario.

### Lo que no tiene horario

Siete materias no tienen paralelos porque no llevan horario fijo: Servicio Comunitario (727),
Prácticas Preprofesionales (827), Trabajo de Titulación (157) y los cuatro niveles de Inglés
(107 – 110). Esas se agregan a mano.

Todos los paralelos traen docente asignado en el SIUG.

## Cómo se usa

1. **Malla** — buscas la materia o filtras por semestre, y haces clic en ella.
2. **Paralelos** — se abre la lista de paralelos disponibles con su horario, aula y docente.
   Filtras por jornada y eliges uno; se llena todo solo. También puedes escribirlo a mano.
3. **Calendario** — la materia aparece como un bloque de lunes a sábado; la rejilla va de tu primera
   clase a la última.
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
| Paralelos, horarios, jornada, aula y docente | SIUG, Ver detalle de los horarios, Ciclo II 2026 – 2027 |

Los datos quedaron transcritos dentro de `index.html`; los PDFs que se usaron antes no se versionan
(están en `.gitignore`).

Los nombres de docentes van en mayúscula inicial. El SIUG trae la mayoría sin tildes y no se les
inventaron, salvo donde una fuente anterior ya traía el nombre acentuado.
