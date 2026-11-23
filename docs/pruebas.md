# Pruebas

Plan de pruebas de la Fase 4A. Todavía no he ejecutado ninguna prueba: todas figuran como pendientes y rellenaré el resultado obtenido, el estado y la fecha (o el número de incidencia) cuando haga cada una.

| ID | Funcionalidad | Acción o procedimiento | Resultado esperado | Obtenido | Estado | Fecha / incidencia |
|----|---------------|------------------------|--------------------|----------|--------|--------------------|
| P01 | Reserva de pista | Entro como jugador, elijo una pista libre, un día y una franja y pulso «Reservar» | La reserva se guarda, aparece en «Mis reservas» y se muestra confirmación | — | Pendiente | |
| P02 | Control de solapamientos | Con la pista ya reservada en P01, entro como otro jugador e intento reservar la misma pista, día y franja | Se rechaza la segunda reserva y se avisa de que la pista está ocupada | — | Pendiente | |
| P03 | Modificar una reserva | Cambio la franja de una reserva mía a otra libre, dentro del plazo permitido | La reserva pasa a la nueva franja, la antigua queda libre y se muestra confirmación | — | Pendiente | |
| P04 | Cancelación fuera de plazo | Intento cancelar una reserva cuando ya ha pasado el plazo que fija el club | La cancelación se rechaza y se explica el motivo | — | Pendiente | |
| P05 | Aforo de las clases | Apunto jugadores a una clase hasta completar el aforo e intento apuntar a uno más | El último intento se rechaza y se avisa de que la clase está completa | — | Pendiente | |
| P06 | Horarios fijos | Cancelo una sesión concreta de mi franja fija semanal | Ese día queda libre para otros y la franja sigue activa las semanas siguientes | — | Pendiente | |
| P07 | Permisos por rol | Entro como jugador y escribo la dirección de una página del panel de la coordinadora | El servidor bloquea el acceso y me devuelve al inicio | — | Pendiente | |
| P08 | Validación de formularios | Envío el formulario de registro con campos vacíos y con un correo mal escrito | No se guarda nada y se indica qué campos están mal | — | Pendiente | |
| P09 | Registro e inicio de sesión | Creo una cuenta con datos válidos, cierro sesión y vuelvo a entrar | Se crea la cuenta y se puede entrar y salir | — | Pendiente | |
| P10 | Consulta de huecos libres | Consulto una fecha y franja con reservas hechas | Solo aparecen las pistas realmente libres | — | Pendiente | |
| P11 | Consulta de clases del nivel | Entro como jugador de un nivel y miro las clases | Solo aparecen clases de su nivel, con día, hora, profesor y plazas | — | Pendiente | |
| P12 | Reservas fuera de las reglas | Intento reservar fuera de horario y por encima del máximo de reservas | Ambas reservas se rechazan con un mensaje claro | — | Pendiente | |
| P13 | Panel de la coordinadora | Creo, modifico y elimino una pista, una clase y un horario fijo | Los cambios se aplican y se guardan | — | Pendiente | |
| P14 | Consulta del profesor | Entro como profesor y miro mis clases y alumnos | Veo solo mis clases y los alumnos apuntados | — | Pendiente | |
| P15 | Historial del jugador | Miro el historial con reservas pasadas y presentes | Aparecen las mías y no las de otros | — | Pendiente | |
| P16 | Persistencia de los datos | Cierro sesión, reinicio el servidor y vuelvo a entrar | Los datos siguen ahí | — | Pendiente | |

Estados posibles: Pendiente, Superada, Fallida.
