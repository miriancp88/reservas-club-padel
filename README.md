# Gestión autónoma de reservas en un club de pádel

Aplicación web de reservas para un club de pádel de Elche. Proyecto Intermodular de 2.º de Desarrollo de Aplicaciones Web (DAW), de Mirian Cabrera Parra.

## Descripción

Una aplicación web en la que los jugadores consultan los huecos libres de las pistas y de las clases por niveles y reservan por sí mismos, y la coordinadora del club gestiona pistas, clases, horarios fijos y reglas desde un panel propio.

## Problema que pretende resolver

El club no tiene sistema de reservas y todo se gestiona por WhatsApp con la coordinadora. Por eso el jugador solo conoce el hueco que se le ofrece, todo depende de una sola persona, a quienes tienen horarios cambiantes (por ejemplo, turnos rotativos) les resulta más difícil reservar, y no queda un registro ordenado de las reservas.

## Funcionalidades previstas

- Registro, inicio de sesión y tres tipos de usuario con permisos distintos: jugador, coordinadora y profesor.
- Consulta de huecos libres de las pistas por día y franja horaria.
- Reserva, modificación y cancelación de pistas, con validaciones que impiden reservas incompatibles.
- Clases por nivel con aforo: inscripción y baja.
- Horarios fijos, con posibilidad de cancelar una sesión sin perder la franja.
- Panel de la coordinadora e historial de reservas.
- Consulta de clases y alumnos para el profesor.

Ampliaciones, solo si hay tiempo: lista de espera, avisos por correo y estadísticas de ocupación.

## Tecnologías previstas

HTML, CSS y JavaScript con Bootstrap en la parte que ve el usuario, PHP en el servidor y MySQL como base de datos.

## Estado actual

**Fase 4A: plan de seguimiento y control.** El proyecto sigue en fase de planificación y todavía no hay código de la aplicación. Ya están hechos el análisis de la necesidad, el diseño y estudio de viabilidad, el plan de ejecución y el plan de seguimiento. El estado de las tareas se ve en el [tablero de seguimiento](https://github.com/users/miriancp88/projects/1).

## Documentación

Toda la documentación está en la carpeta [`docs/`](docs/):

- [Plan de ejecución](docs/plan-de-ejecucion.md): tareas, dependencias, horas, cronograma, hitos y procedimiento de trabajo.
- [Cronograma (Gantt)](docs/plan-de-ejecucion.md#cronograma).
- [Registro de riesgos](docs/riesgos.md).
- [Permisos y autorizaciones](docs/permisos.md).
- [Documentación técnica inicial](docs/documentacion-tecnica.md): tecnologías, requisitos y roles.
- [Recursos](docs/recursos.md).
- [Decisiones del proyecto](docs/decisiones.md).
- [Seguimiento semanal](docs/seguimiento.md).
- [Plan de pruebas](docs/pruebas.md) y carpeta de [evidencias](docs/evidencias/).
- [Indicadores de calidad](docs/indicadores.md).
- [Registro de cambios](docs/cambios.md).
- [Evaluación con usuarios](docs/usuarios.md).
- [Matriz de aceptación](docs/requisitos.md).
- Plantilla de incidencias: [.github/ISSUE_TEMPLATE/incidencia.md](.github/ISSUE_TEMPLATE/incidencia.md).

## Estructura del repositorio

```
reservas-club-padel/
├── README.md        Descripción del proyecto
├── .gitignore
├── .github/         Plantilla de incidencias
└── docs/            Documentación (plan y cronograma, riesgos, permisos, documentación técnica, recursos, decisiones, seguimiento, pruebas, indicadores, cambios, usuarios, requisitos y evidencias)
```

El código se añadirá en carpetas nuevas (por ejemplo `src/` y `sql/`) durante el desarrollo y se anotará aquí.
