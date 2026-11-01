# Política de privacidad de Virtual Memorial Space

**Fecha de entrada en vigor: 1 de noviembre de 2026**

## 1. Introducción

Virtual Memorial Space («la App», «nosotros») es una app para iOS que permite crear espacios conmemorativos privados, realizar rituales de recuerdo y escribir cartas. Esta política de privacidad explica qué información trata la App, dónde se guarda y qué opciones tienes.

La App no requiere cuenta. Tu contenido conmemorativo permanece en tu dispositivo. Nuestro servidor se usa únicamente para las fichas conmemorativas, unas fichas opcionales dentro de la App que sirven para estilos de ofrendas más elaborados.

Al usar la App, confirmas que has leído y comprendido esta política de privacidad.

## 2. Información que no recopilamos

La App no recopila ni solicita:

- Tu nombre, correo electrónico, número de teléfono ni ninguna cuenta de inicio de sesión
- Los nombres, fotos, fechas, descripciones, cartas o mensajes de tus espacios conmemorativos
- Acceso a toda tu fototeca, ni a la cámara, el micrófono, los contactos o la ubicación
- Los datos de tu tarjeta de pago
- Un identificador publicitario (IDFA). La App no te rastrea a través de apps o sitios web de otras empresas y no muestra la solicitud de Transparencia en el rastreo de apps (ATT).
- Datos analíticos ni eventos de uso. La App no incluye ningún SDK de análisis ni publicidad.

## 3. Contenido conmemorativo guardado solo en tu dispositivo

Lo siguiente se guarda en el almacenamiento privado de la App en tu iPhone o iPad:

- Espacios conmemorativos: nombre, tipo (por ejemplo, un ser querido, pareja, amigo o mascota), descripción, fecha de nacimiento, fecha de recuerdo, tema y ajuste de recordatorio
- Las fotos que añades a un espacio conmemorativo
- Registros de rituales: qué vela, flor u ofrenda de papel se usó, el número de fichas gastadas, la hora y el mensaje que añadas
- Las cartas que escribes, incluidos los borradores
- Preferencias: idioma, efectos reducidos, si se muestran las ofrendas de papel tradicionales, si se completó la introducción, una marca de sincronización de compra pendiente y un contador que limita las solicitudes de valoración
- El último saldo de fichas recibido de nuestro servidor, usado solo para mostrarlo sin conexión

Este contenido no se sube a nuestro servidor, no se usa para publicidad y no se utiliza para ninguna función ni entrenamiento de inteligencia artificial (IA). Si tienes activada la copia de seguridad de iCloud, iOS puede incluir estos datos en la copia del dispositivo, que Apple gestiona bajo tu Apple ID. La App no tiene sincronización en la nube propia.

**Fotos.** Eliges las fotos con el selector de fotos del sistema. La App solo recibe las fotos que seleccionas y no accede a toda tu fototeca. Se guarda una copia comprimida de cada foto seleccionada dentro del almacenamiento de la App.

## 4. Fichas conmemorativas y nuestro servidor

Las fichas conmemorativas son compras dentro de la App de tipo consumible. Para que tu saldo se conserve si reinstalas la App, se guarda en nuestro servidor («appapi»), que funciona en Vercel y almacena los datos en Vercel KV (Upstash Redis).

El servidor solo guarda:

- Un ID de usuario generado aleatoriamente, sin relación con tu nombre, tu correo electrónico ni tu Apple ID
- Un resumen (hash) del token de acceso emitido para ese ID de usuario. El token en sí no se guarda en el servidor.
- Tu saldo de fichas
- Registros de compra: ID del producto, ID de transacción de Apple, número de fichas y hora
- Registros de gasto: ID de la ofrenda (por ejemplo, un tipo de vela), número de fichas, la clave de solicitud que evita un doble cargo, saldo resultante y hora
- Un historial de abonos, gastos y reembolsos con sus importes y los ID de transacción o de gasto relacionados

Cada solicitud al servidor incluye también la versión de la App y un identificador del dispositivo (el identifierForVendor de iOS), que se usan para verificar la firma de la solicitud. Como en cualquier servicio web, nuestro proveedor de alojamiento puede tratar tu dirección IP en registros habituales de solicitudes para prestar y proteger el servicio.

El servidor no guarda tu nombre, tu correo electrónico ni nada sobre las personas o mascotas que recuerdas: ningún nombre, foto, carta ni mensaje conmemorativo.

El ID de usuario y el token se guardan en el llavero de iOS de tu dispositivo. Pueden sincronizarse mediante el llavero de iCloud, de modo que tu saldo esté disponible tras reinstalar la App o en otro dispositivo con el mismo Apple ID.

## 5. Compras

- **Apple (App Store)** procesa todos los pagos a través de tu Apple ID. Nunca recibimos los datos de tu tarjeta de pago. Política de privacidad de Apple: https://www.apple.com/legal/privacy/
- **RevenueCat** valida las transacciones. RevenueCat recibe el ID de usuario aleatorio mencionado, información de la transacción (como el ID del producto, el ID de transacción de Apple y la hora de compra) e información técnica básica como la versión de la App, la versión del sistema operativo y el país de la App Store. Nuestro servidor pide a RevenueCat que confirme las compras, y RevenueCat notifica a nuestro servidor las compras y los reembolsos, para que las fichas se abonen una sola vez y se retiren tras un reembolso. Política de privacidad de RevenueCat: https://www.revenuecat.com/privacy

Las fichas conmemorativas no tienen valor monetario real. Los reembolsos los gestiona Apple según sus normas. Las condiciones de uso son el contrato de licencia estándar de Apple: https://www.apple.com/legal/internet-services/itunes/dev/stdeula/

## 6. Notificaciones (opcionales)

Si activas un recordatorio de fecha conmemorativa para un espacio, la App solicita permiso para enviar notificaciones y programa notificaciones locales en tu dispositivo. Los recordatorios no pasan por nuestro servidor. Puedes desactivarlos en la App o en los Ajustes de iOS.

## 7. Cómo usamos la información

Usamos la información anterior únicamente para:

- Mostrar y conservar tus espacios conmemorativos, rituales y cartas en tu dispositivo
- Crear tu monedero de fichas, abonar las fichas compradas una sola vez por transacción, descontar fichas cuando eliges una ofrenda premium y retirar fichas tras un reembolso
- Verificar solicitudes y evitar fraudes o abonos duplicados
- Responder a tus solicitudes de soporte

No vendemos ni alquilamos información personal, no la usamos para publicidad y no creamos perfiles publicitarios.

## 8. Compartir información

Solo compartimos información con los proveedores necesarios para que funcione la App (Apple, RevenueCat y Vercel / Upstash para alojamiento y almacenamiento), o cuando lo exija la ley o un procedimiento legal válido.

## 9. Eliminar tus datos

En los Ajustes de la App:

- **Eliminar todos los datos (Delete All Data)** elimina todo el contenido conmemorativo de este dispositivo: espacios conmemorativos, fotos, registros de rituales, cartas y mensajes.
- **Eliminar datos de fichas (Delete Token Data)** elimina tu monedero en nuestro servidor: el registro del ID de usuario, el hash del token, el saldo, los registros de compra y gasto y el historial. Tu saldo pasa a cero y no se puede recuperar. Para evitar que una misma compra se abone de nuevo, conservamos solo el ID de transacción de Apple (con su ID de producto), sin el ID de usuario. Después, el ID de usuario y el token se eliminan también de tu llavero.

Eliminar la App borra su contenido local del dispositivo, pero **no** elimina tu monedero de nuestro servidor. Para eliminarlo, usa «Eliminar datos de fichas» antes de eliminar la App o contáctanos. Los datos locales eliminados pueden permanecer en copias de seguridad anteriores de iCloud del dispositivo hasta que Apple las sustituya o elimine.

También puedes pedirnos que solicitemos a RevenueCat la eliminación del registro de compra que conserva.

## 10. Seguridad y conservación

Las conexiones con nuestro servidor, Apple y RevenueCat usan HTTPS cifrado. Las solicitudes van firmadas, el servidor solo guarda un hash de tu token y tu identidad se guarda en el llavero de iOS. Ningún método de almacenamiento o transmisión es totalmente seguro.

- El contenido local se conserva hasta que lo eliminas o eliminas la App.
- Los datos del monedero en el servidor se conservan hasta que usas «Eliminar datos de fichas» o nos pides que los eliminemos.
- Los ID de transacción de Apple sin ID de usuario se conservan para evitar abonos duplicados.
- Apple y RevenueCat conservan los registros de compra según sus propias políticas y obligaciones legales.

## 11. Privacidad de los menores

Virtual Memorial Space no está dirigida a menores. No recopilamos a sabiendas información personal de menores de 13 años (o de la edad mínima exigida en tu país). Si crees que un menor nos ha facilitado información personal, contáctanos y la eliminaremos.

## 12. Tratamiento internacional

Nuestros proveedores de alojamiento y almacenamiento y RevenueCat pueden tratar datos en Estados Unidos o en otros países distintos del tuyo. Para dicho tratamiento nos basamos en las garantías de estos proveedores.

## 13. Tus derechos

Según dónde vivas, puedes tener derecho a acceder, rectificar, suprimir o limitar el tratamiento de tu información personal. La mayoría de los datos están en tu dispositivo y bajo tu control. Para los datos de nuestro servidor, usa «Eliminar datos de fichas» o contáctanos. Podemos pedirte información que nos ayude a localizar los registros correspondientes.

## 14. Cambios en esta política

Podemos actualizar esta política de privacidad. La fecha de la parte superior cambiará cuando lo hagamos. Si la App empieza a recopilar nuevos tipos de datos, actualizaremos antes esta política.

## 15. Contacto

Si tienes preguntas sobre esta política de privacidad, contáctanos:

- Correo electrónico: lpjustdoit@163.com

---

## Otros idiomas

- [English](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/en/privacy.md)
- [简体中文](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/zh/privacy.md)
- [繁體中文](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/zh-tw/privacy.md)
- [日本語](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ja/privacy.md)
- [한국어](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ko/privacy.md)
- [Deutsch](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/de/privacy.md)
- [Français](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/fr/privacy.md)
- [Español](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/es/privacy.md)
- [Italiano](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/it/privacy.md)
- [Português (Portugal)](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/pt-PT/privacy.md)
- [Português (Brasil)](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/pt-BR/privacy.md)
- [ไทย](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/th/privacy.md)
- [Tiếng Việt](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/vi/privacy.md)
- [Bahasa Indonesia](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/id/privacy.md)
- [Bahasa Melayu](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ms/privacy.md)
- [العربية](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ar/privacy.md)
