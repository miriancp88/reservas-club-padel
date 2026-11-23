# Indicadores de calidad

Salen de los requisitos de la Fase 2. Todavía no hay ninguna medición: la columna «Valor medido» se rellena al hacer cada comprobación.

| Indicador | Qué controla | Cómo se comprobará | Resultado aceptable | Cuándo | Valor medido |
|-----------|--------------|--------------------|---------------------|--------|--------------|
| Funcionalidades esenciales comprobadas | Cumplimiento de los requisitos funcionales | Cuento cuántas de las 9 funcionalidades esenciales del alcance tienen su prueba superada en el registro | 9 de 9 superadas antes de publicar | Cada domingo y antes de publicar (T14) | |
| Reservas solapadas | Que no se reserve una pista ocupada | Registro dos reservas para la misma pista, fecha y franja | La segunda se rechaza y un mensaje explica el conflicto | Al terminar las reservas y en T13 | |
| Reservas fuera de las reglas | Horario del club, máximo de reservas y plazo de cancelación | Intento reservar fuera del horario, superar el máximo por jugador y cancelar fuera de plazo | Las tres operaciones se rechazan con un mensaje claro | Al terminar las reglas del club y en T13 | |
| Aforo y nivel de las clases | Que no se apunte más gente de la permitida ni de otro nivel | Lleno una clase e intento apuntar a un jugador más, y a otro de un nivel distinto | Ambos intentos se rechazan y se avisa del motivo | Al terminar las inscripciones a clases | |
| Validación de formularios | Que no entren datos incorrectos | Envío cada formulario vacío, con una fecha no válida y con un correo mal escrito | No se guarda nada y se indica qué campo falla | Al terminar cada formulario | |
| Control de acceso por rol | Que cada usuario solo haga lo suyo | Con la sesión de jugador pido una página de la coordinadora; con la del profesor intento modificar una reserva | El servidor rechaza la petición, no solo se esconde el botón | Al terminar el inicio de sesión y en T13 | |
| Contraseñas protegidas | Seguridad de los datos de acceso | Reviso la tabla de usuarios en phpMyAdmin | Ninguna contraseña aparece en texto legible | Al terminar el registro | |
| Integridad de los datos | Datos coherentes tras operar | Cancelo una reserva y una baja de clase y reviso la base de datos | El hueco o la plaza queda libre, no quedan registros a medias y la base de datos impide dos reservas iguales | Al terminar cancelaciones y en T13 | |
| Adaptación a móvil | Uso correcto en pantalla pequeña | Abro las pantallas principales a 375 px de ancho | Todo se ve y se usa sin desplazarse hacia los lados | Al terminar cada pantalla y antes de publicar | |
| Accesibilidad básica | Contraste y etiquetas | Compruebo que cada campo tenga su etiqueta y mido el contraste de los textos con una herramienta del navegador | Todos los campos con etiqueta y contraste suficiente en los textos principales | Al terminar la interfaz y antes de publicar | |
| Rendimiento de la disponibilidad | Rapidez de la consulta de huecos libres | Cronometro la consulta de un día con los datos de prueba | Menos de 3 segundos | En T13 | |
| Hitos y errores críticos | Cumplimiento del cronograma y estabilidad | Comparo el tablero con el cronograma y cuento las incidencias graves abiertas | Cada hito en su semana (o dentro del margen de febrero) y 0 incidencias graves abiertas al publicar | Cada domingo y antes de publicar (T14) | |
