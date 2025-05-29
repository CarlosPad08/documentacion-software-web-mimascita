
### Pasar a la siguiente sección: [Metricas de Exito](23-metricas-de-exito.md)

## 22. Soporte para notificaciones push

La aplicación "MiMascota" incorpora soporte para notificaciones push basado en la infraestructura existente de componentes de alerta utilizados en otros flujos (por ejemplo, `SuccessAlert` y `ErrorAlert`).

### Implementación técnica:
- Se aprovechan los componentes personalizados de alerta (`PushNotificationAlert`) para mostrar mensajes cuando se reciben notificaciones push en primer plano.
- Las notificaciones se integran con Firebase Cloud Messaging (FCM), lo que permite enviar alertas desde el backend hacia usuarios autenticados o suscritos.
- El `Service Worker` (`firebase-messaging-sw.js`) gestiona los mensajes en segundo plano para mostrar notificaciones persistentes incluso cuando la aplicación está cerrada o inactiva.
- Se utiliza el hook `onMessage` de Firebase para interceptar notificaciones entrantes en primer plano y mostrarlas con la interfaz visual ya familiar para el usuario.
- El diseño de las alertas push sigue la misma línea visual que otras alertas utilizadas en la aplicación, manteniendo coherencia de estilo.

Esta implementación garantiza una experiencia consistente e intuitiva para el usuario, con notificaciones contextuales visibles directamente dentro de la aplicación web.