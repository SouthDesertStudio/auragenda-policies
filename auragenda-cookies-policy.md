# Politica de cookies de Auragenda

Ultima actualizacion: 19 de junio de 2026

Esta politica explica de forma sencilla que cookies usa Auragenda y para que sirven. Es una politica operativa de producto pensada para la version v1.0; antes de publicarla en produccion debe revisarse con la informacion legal y societaria definitiva del responsable del tratamiento. Para el tratamiento general de datos personales, consulta la politica de privacidad de Auragenda.

## 1. Que es una cookie

Una cookie es un pequeño archivo de texto que la web guarda en tu navegador. Auragenda usa cookies solo para que el servicio funcione, no para perfilar ni rastrear tu actividad.

## 2. Que cookies usamos

En la version v1.0 Auragenda usa una unica cookie, estrictamente necesaria para el funcionamiento del servicio.

### Cookie de sesion (necesaria)

- **Nombre:** `__Host-teragenda_session` en produccion (`teragenda_session` en entornos de desarrollo sin HTTPS).
- **Para que sirve:** mantener la sesion iniciada de las personas que administran el negocio, para que no tengan que volver a identificarse en cada accion.
- **Que contiene:** un identificador de usuario y su rol, firmados con HMAC. No guarda contrasenas, ni tokens de Google, ni datos en texto que el navegador pueda leer por JavaScript.
- **Caracteristicas de seguridad:** `httpOnly` (no accesible desde JavaScript), `sameSite=lax`, `secure` en produccion (solo viaja por HTTPS), `path=/` y, en produccion, el prefijo `__Host-` que impide que se inyecte desde subdominios.
- **Duracion:** caduca a las 8 horas. Se elimina al cerrar sesion.
- **Es obligatoria:** sin ella no es posible administrar el negocio. No requiere consentimiento porque es imprescindible para prestar el servicio.

## 3. Cookies que NO usamos

En la version v1.0 Auragenda **no** usa:

- Cookies de publicidad o marketing dirigido.
- Cookies que perfilen tu comportamiento entre distintas webs.
- Cookies de redes sociales para perfilar visitantes.

Auragenda **no vende tus datos a terceros** en ningun caso.

## 4. Visibilidad en buscadores y asistentes de IA

Queremos que la web del negocio aparezca en buscadores y asistentes como Google, Bing, Google Business, Gemini, OpenAI ChatGPT y similares. Es importante aclarar como funciona:

- **La indexacion no se hace con cookies.** Aparecer en esos servicios se consigue porque sus rastreadores leen el contenido publico de la web (texto, titulos, metadatos de descripcion, Open Graph, sitemaps y datos estructurados). Esos rastreadores no instalan cookies en tu navegador.
- **Posibles cookies de medicion o visibilidad.** Aunque actualmente puede que no esten activas, en el futuro podriamos usar herramientas de estos proveedores (por ejemplo, herramientas de medicion de visibilidad o de posicionamiento) que si fijen cookies. Si llega a ocurrir, su **unico fin** sera mejorar la indexacion, la visibilidad y la presencia del negocio en esos servicios.
- **Sin venta de datos.** Estas cookies o herramientas, en su caso, nunca implicaran la venta de tus datos a terceros. Solo se usan para que el negocio sea encontrado.

Cuando se activen herramientas de este tipo, actualizaremos esta politica y, si la normativa lo exige, solicitaremos tu consentimiento previo.

## 5. Cookies de terceros

Auragenda no instala cookies de terceros por su cuenta, pero ten en cuenta dos casos:

- **Inicio de sesion con Google:** si un administrador se identifica con Google, el proceso ocurre en los dominios de Google, que pueden fijar sus propias cookies en ese contexto. Esas cookies se rigen por las politicas de Google, no por esta.
- **Imagenes alojadas en hosts externos:** si el negocio usa URLs remotas para sus imagenes, tu navegador las solicita directamente a ese host, que podria fijar sus propias cookies segun su configuracion.

## 6. Como gestionar las cookies y darse de baja

Puedes borrar o bloquear las cookies desde la configuracion de tu navegador, y darte de baja del uso del servicio en cualquier momento. Si bloqueas la cookie de sesion, no podras mantener iniciada la administracion del negocio y tendras que identificarte de nuevo.

Si quieres dejar de usar Auragenda o solicitar la eliminacion de tu cuenta y tus datos, puedes hacerlo en cualquier momento usando los datos de contacto de la seccion siguiente.

## 7. Contacto

Para cualquier consulta sobre esta politica, gestionar tus cookies o darte de baja, puedes contactar a traves de:

- Web: https://southdesertstudio.com
- Email: hola@southdesertstudio.com
- Instagram: @southdesertstudio
- Telefono: +34 604 858 298

## 8. Cambios en esta politica

Podemos actualizar esta politica si en futuras versiones se añaden nuevas cookies o servicios. La fecha de ultima actualizacion indicara la version vigente.
