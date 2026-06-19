# Politica de privacidad de Auragenda

Ultima actualizacion: 19 de junio de 2026

Esta politica explica de forma sencilla que datos personales guarda Auragenda, para que los usa y como los protege. Es una politica operativa de producto; antes de publicarla en produccion debe revisarse con la informacion legal y societaria definitiva del responsable del tratamiento.

## 1. Quien es responsable

El responsable de los datos es el negocio que usa Auragenda para gestionar sus reservas. Auragenda actua como herramienta tecnica para crear, administrar y sincronizar esas reservas.

South Desert Studio es el proveedor tecnico de Auragenda. Sus datos de contacto son:

- Web: https://southdesertstudio.com
- Email: hola@southdesertstudio.com
- Instagram: @southdesertstudio
- Telefono: +34 604 858 298

Para ejercer derechos sobre tus datos, debes contactar con el negocio con el que has reservado o con el canal de soporte que se indique en la web de reservas. Tambien puedes escribir a South Desert Studio si necesitas ayuda para identificar el canal correcto o trasladar una solicitud tecnica relacionada con Auragenda.

## 2. Que datos personales guardamos

Auragenda guarda solo los datos necesarios para prestar el servicio de reservas y administracion.

### Datos de clientes

- Nombre o nombre visible de la cuenta.
- Email, cuando el cliente inicia sesion o cuando la reserva lo requiere.
- Telefono de contacto.
- Reserva solicitada o confirmada: servicio, profesional si aplica, fecha, hora, estado y datos operativos asociados.
- Notas que el cliente escriba en la reserva.
- Historial tecnico de recordatorios enviados, omitidos o fallidos.

Las notas de reserva son un campo libre. Recomendamos no incluir informacion sensible que no sea necesaria para gestionar la cita.

### Datos de usuarios administradores

- Email.
- Nombre visible, nombre, apellidos, avatar, idioma y datos de perfil cuando proceden del inicio de sesion con Google.
- Rol de acceso: usuario, administrador o superadministrador.
- Fecha de ultimo acceso.
- Hash de contrasena en cuentas administrativas legacy, cuando existan.

Auragenda no guarda contrasenas en claro. Las contrasenas administrativas se guardan con hash bcrypt.

### Datos de profesionales y negocio

- Nombre y email de profesionales, si el negocio los configura.
- Horarios, ausencias, servicios, imagenes del negocio y configuracion operativa.
- Las imagenes del negocio pueden mostrar personas identificables. La responsabilidad de contar con derechos, autorizacion o consentimiento sobre esas imagenes corresponde al negocio que las aporta.

### Datos de Google Calendar

Si el negocio conecta Google Calendar, Auragenda guarda:

- Email de la cuenta Google conectada.
- Identificador del calendario dedicado del negocio.
- Estado de conexion y sincronizacion.
- Tokens OAuth necesarios para crear, actualizar o cancelar eventos.

Auragenda no debe usar el calendario personal principal como destino compartido. Cada negocio debe usar un calendario dedicado.

### Datos de auditoria y seguridad

Auragenda guarda registros de auditoria para acciones relevantes: login, creacion o modificacion de reservas, cambios de estado, cambios de configuracion, autorizaciones y sincronizacion con Google Calendar.

Estos registros pueden contener identificadores o metadatos necesarios para reconstruir una accion, pero no deben contener contrasenas, cookies de sesion, tokens OAuth ni credenciales.

## 3. Para que usamos los datos

Usamos los datos para:

- Crear y gestionar reservas.
- Mostrar disponibilidad real y evitar dobles reservas.
- Permitir al negocio administrar citas, servicios, horarios y profesionales.
- Enviar recordatorios o comunicaciones relacionadas con la reserva cuando esten configuradas.
- Sincronizar reservas con el calendario dedicado del negocio.
- Mantener seguridad, auditoria, trazabilidad operativa y soporte.
- Exportar, anonimizar o eliminar datos cuando corresponda.

No vendemos datos personales.

## 4. Visibilidad en buscadores, asistentes y fichas de negocio

Auragenda y los negocios que usan Auragenda pueden querer aparecer en buscadores, mapas, asistentes de IA y servicios de descubrimiento como Google, Google Business Profile, Google Maps, Bing, ChatGPT, Gemini u otros servicios similares.

Para ello pueden publicarse y optimizarse paginas o fichas con informacion publica del negocio, por ejemplo nombre comercial, descripcion, servicios, horarios, zona o direccion si aplica, web, telefono, email de contacto, imagenes del negocio y enlaces publicos.

Esa visibilidad no requiere vender datos personales ni entregar datos privados de clientes. Los datos de reservas, cuentas de usuario, notas, telefonos privados de clientes, emails de clientes, tokens, cookies de sesion y registros internos no se publican para indexacion.

Los buscadores y asistentes pueden rastrear paginas publicas mediante bots o agentes automaticos, siguiendo sus propias politicas y los controles tecnicos disponibles, como `robots.txt`, metadatos de indexacion, sitemaps o datos estructurados. La indexacion no se realiza instalando cookies en el navegador del usuario. Si en el futuro se incorporan herramientas de analitica, medicion, publicidad o posicionamiento que usen cookies o tecnologias similares, se informara en la politica de cookies y, cuando proceda, se pedira el consentimiento correspondiente.

## 5. Como se guardan y protegen los datos

Auragenda esta disenada para produccion v1.0 con estas medidas:

- Base de datos PostgreSQL con datos separados por negocio mediante `business_id`.
- Acceso administrativo protegido por sesion firmada, cookie `httpOnly` y `sameSite`.
- Passwords administrativos guardados con bcrypt, no en texto claro.
- Variables sensibles fuera del repositorio, en variables de entorno o archivos `.env` protegidos.
- Rate limiting y cabeceras de seguridad en el servidor.
- Auditoria de operaciones relevantes.
- Tokens OAuth de Google Calendar cifrados en reposo con AES-256-GCM.
- Clave de cifrado `TOKEN_ENCRYPTION_KEY_V1` guardada fuera del codigo y de la base de datos.
- Backups PostgreSQL con permisos restrictivos.

Los tokens OAuth de Google Calendar no se muestran al frontend, no se exportan en texto claro y no deben copiarse a documentacion, prompts, tickets ni herramientas de chat.

## 6. Comunicaciones y terceros

Auragenda puede tratar datos con estos servicios externos:

- South Desert Studio, como proveedor tecnico de Auragenda y soporte operativo de la aplicacion.
- Google Calendar, si el negocio conecta su cuenta para sincronizar reservas.
- Proveedor SMTP o email, si el negocio activa recordatorios por correo.
- Buscadores, mapas, asistentes de IA y servicios de descubrimiento, solo respecto de informacion publica del negocio y paginas publicas indexables.
- Proveedores de hosting, base de datos, backups o infraestructura necesarios para ejecutar la aplicacion.
- Hosts externos de imagenes, si el negocio usa URLs remotas para imagenes. En ese caso, el navegador del visitante puede solicitar la imagen directamente al host externo.

Los emails de recordatorio se envian al email del cliente asociado a la reserva. No se usan emails de profesionales o administradores como destinatarios de recordatorios de cliente.

## 7. Conservacion, exportacion y borrado

Auragenda conserva los datos mientras sean necesarios para gestionar reservas, auditoria y obligaciones operativas del negocio.

Cuando se solicita acceso, exportacion, rectificacion o borrado, el negocio debe poder gestionar la solicitud. En el estado v1.0 previsto:

- Los datos de un negocio pueden exportarse y eliminarse de forma controlada.
- Las reservas de un cliente pueden anonimizarse cuando proceda.
- Los registros de auditoria se conservan para integridad operativa, pero sus metadatos personales pueden anonimizarse.
- Los backups no se modifican fila a fila; se aplicara la politica de retencion de backups vigente.

La eliminacion de un negocio se entiende como borrado fisico controlado de sus datos, manteniendo los registros de auditoria anonimizados cuando sea necesario.

## 8. Datos especialmente sensibles

Auragenda puede ser usada por negocios de salud o bienestar. Una reserva puede revelar que una persona ha solicitado un servicio de ese tipo. Por eso tratamos las reservas, notas y datos asociados con especial cautela.

Auragenda no tiene campos de historial medico, diagnostico o tratamiento clinico. Aun asi, el cliente puede escribir informacion sensible en las notas. Solo debe incluir lo imprescindible para gestionar la reserva.

## 9. Tus derechos

Puedes solicitar, segun la normativa aplicable:

- Acceso a tus datos.
- Rectificacion de datos incorrectos.
- Eliminacion o anonimizacion cuando proceda.
- Limitacion u oposicion al tratamiento.
- Portabilidad de los datos.

La solicitud debe dirigirse al negocio responsable de la reserva o al canal de contacto publicado por el servicio.

## 10. Cambios en esta politica

Podemos actualizar esta politica cuando cambien las funcionalidades, proveedores o medidas de seguridad. La fecha de ultima actualizacion indicara la version vigente.
