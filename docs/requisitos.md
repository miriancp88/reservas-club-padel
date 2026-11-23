# Matriz de aceptación

Relaciona cada requisito con su criterio de aceptación y la prueba que lo comprueba. Estado actual: ninguno aceptado todavía.

| ID | Requisito | Criterio de aceptación | Prueba o comprobación | Evidencia | Estado |
|----|-----------|------------------------|-----------------------|-----------|--------|
| R01 | Registro e inicio de sesión con correo y contraseña | Se puede crear una cuenta, entrar y salir; los datos erróneos se rechazan | P08 y P09 | Capturas y registro de pruebas | Pendiente |
| R02 | Roles con permisos distintos (jugador, coordinadora, profesor) | Cada rol solo accede a lo suyo; las páginas de otro rol quedan bloqueadas en el servidor | P07 | Captura del bloqueo y registro de pruebas | Pendiente |
| R03 | Consultar huecos libres por día y franja | Para una fecha y franja se muestran exactamente las pistas libres | P10 | Captura y comparación con la base de datos | Pendiente |
| R04 | Consultar clases del nivel del jugador con plazas libres | Solo aparecen clases de su nivel, con día, hora, profesor y plazas | P11 | Captura del listado | Pendiente |
| R05 | Reservar, modificar y cancelar pistas dentro del plazo | La reserva se guarda y se confirma; modificar y cancelar funcionan; fuera de plazo se rechaza | P01, P03 y P04 | Capturas y filas de la reserva en la base de datos | Pendiente |
| R06 | Evitar reservas incompatibles | Se rechaza una pista ocupada, fuera de horario o por encima del máximo de reservas, con un mensaje claro | P02 y P12 | Capturas de los mensajes y registro de pruebas | Pendiente |
| R07 | Inscripción y baja en clases con control de aforo y nivel | No se admite una clase completa ni de otro nivel; la baja libera la plaza | P05 | Captura y plazas en la base de datos | Pendiente |
| R08 | Horarios fijos con cancelación de una sesión | Al cancelar una sesión, ese día queda libre y la franja sigue activa | P06 | Capturas antes y después | Pendiente |
| R09 | Panel de la coordinadora: pistas, clases, horarios fijos y reglas | Puede crear, consultar, modificar y eliminar cada elemento y los cambios se aplican | P13 | Capturas del panel y datos en la base de datos | Pendiente |
| R10 | El profesor consulta sus clases y alumnos | Ve solo sus clases y los alumnos apuntados | P14 | Captura del listado | Pendiente |
| R11 | Historial de reservas del jugador | Aparecen todas sus reservas pasadas y presentes, y no las de otros | P15 | Captura del historial | Pendiente |
| R12 | Validación de los datos introducidos | Campos vacíos, correo mal escrito y fechas no válidas se rechazan con un mensaje | P08 | Capturas de los mensajes | Pendiente |
| R13 | Datos guardados de forma persistente | Tras cerrar sesión y reiniciar el servidor, los datos siguen ahí | P16 | Captura antes y después | Pendiente |
| R14 | Uso en móvil y ordenador | Las pantallas principales se ven y se usan a 375 px sin desplazarse hacia los lados | Revisión con las herramientas del navegador | Capturas en móvil | Pendiente |
| R15 | Accesibilidad | Todos los campos con etiqueta y contraste suficiente | Revisión de formularios y del contraste | Captura de la herramienta de contraste | Pendiente |
| R16 | Rendimiento | La consulta de disponibilidad tarda menos de 3 segundos con los datos de prueba | Cronometrar la consulta | Tiempo anotado en el registro | Pendiente |
| R17 | Seguridad de contraseñas | Ninguna contraseña en texto legible | Revisar la tabla de usuarios | Captura de phpMyAdmin | Pendiente |
| R18 | Integridad de los datos | Nunca dos reservas activas para la misma pista, fecha y franja, ni una clase por encima de su aforo | P02, P05 y revisión de la restricción en la base de datos | Captura de la restricción y registro de pruebas | Pendiente |
| R19 | Mantenibilidad | Código en módulos, historial de commits y README que explica cómo ejecutarlo | Revisar el repositorio | Enlace al repositorio | Pendiente |
