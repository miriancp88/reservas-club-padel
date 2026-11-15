# Documentación técnica inicial

Resumen de lo definido en la Fase 2 (requisitos y viabilidad técnica). Se actualizará al terminar cada bloque de trabajo.

## Tecnologías

| Parte | Tecnología | Por qué |
|---|---|---|
| Cliente | HTML, CSS y JavaScript con Bootstrap | Casi todas las pantallas son formularios, tablas y listados, y Bootstrap trae componentes preparados y se adapta a móvil y ordenador. No uso un framework de JavaScript porque no lo necesito. |
| Servidor | PHP | Está pensado para páginas web conectadas a una base de datos. Permite sesiones, roles, contraseñas cifradas y validación de formularios, y es un lenguaje que conozco. |
| Base de datos | MySQL | Datos muy relacionados (jugadores, reservas, pistas, clases), restricción de unicidad para evitar reservas duplicadas, transacciones, licencia libre y buena integración con PHP. |

Valoré también MariaDB y PostgreSQL, pero elijo MySQL para no introducir herramientas ni sintaxis nuevas.

## Comunicación entre cliente y servidor

- Protocolo HTTP: el navegador envía una petición, el servidor la procesa, consulta o guarda en MySQL y responde.
- **Formularios HTTP** para registrarse, iniciar sesión, reservar, modificar, cancelar, apuntarse a clases y gestionar pistas y clases.
- **Peticiones con JavaScript y JSON** (fetch) para consultar la disponibilidad sin recargar la página.

## Roles de usuario

- **Jugador:** consulta huecos, gestiona sus propias reservas y se apunta a clases de su nivel.
- **Coordinadora:** gestiona todo el club: pistas, clases, horarios fijos, niveles y reglas.
- **Profesor:** consulta sus clases y alumnos.

## Requisitos funcionales principales

- Registro e inicio de sesión con correo y contraseña, con permisos según el rol.
- Consulta de pistas libres por fecha y franja, y de clases del nivel del jugador.
- Reserva, modificación y cancelación de pistas dentro del plazo que fije el club, con confirmación.
- Inscripción y baja en clases por nivel con aforo.
- Horarios fijos semanales con posibilidad de cancelar una sesión sin perder la franja.
- Gestión de pistas, clases, niveles y reglas del club por la coordinadora.
- Validaciones: no se reserva una pista ocupada, fuera de horario o por encima del máximo de reservas; no se entra en una clase completa o de otro nivel; los datos de los formularios se validan.
- Datos guardados de forma persistente y validados siempre en el servidor.

## Requisitos no funcionales

- **Usabilidad y compatibilidad:** uso correcto desde móvil y ordenador, y reservar en pocos pasos.
- **Accesibilidad:** contraste suficiente y etiquetas en los campos de los formularios.
- **Rendimiento:** consulta de disponibilidad en menos de 3 segundos con los datos de prueba.
- **Seguridad:** contraseñas cifradas y permisos comprobados en el servidor.
- **Fiabilidad e integridad:** nunca dos reservas activas para la misma pista, fecha y franja, y una clase no supera su aforo.
- **Mantenibilidad:** código organizado por módulos, control de versiones y un README que explique cómo ejecutar la aplicación.
