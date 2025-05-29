
### Pasar a la siguiente sección: [Desarrollo Tecnico](09-desarrollo-tecnico.md)

## 8. Accesibilidad e Inclusión

La aplicación "MiMascota" ha sido desarrollada siguiendo principios de accesibilidad e inclusión para garantizar que cualquier persona, sin importar sus capacidades, pueda interactuar con ella de forma efectiva.

### Implementaciones clave:
- Se usan etiquetas `label` correctamente asociadas a los campos de entrada en formularios, mejorando la navegación con lectores de pantalla.
- El diseño visual presenta un buen contraste de color (texto claro sobre fondo oscuro).
- Todos los campos relevantes son validados con el atributo `required`.
- Se estructura el contenido con encabezados jerárquicos (`<h1>`, `<h3>`) para una navegación más clara.
- Se proveen mensajes de éxito y error en los flujos críticos (inicio de sesión, publicación), con potencial para ser adaptados con `role="alert"` para accesibilidad total.

### Mejoras en progreso:
- Incorporación de atributos `aria` y mejoras en la navegación por teclado en componentes como `ModalAdopcion`.
- Inclusión de control de foco en ventanas emergentes.
- Revisión y adaptación de etiquetas semánticas y soporte para lectores de pantalla en todos los componentes interactivos.

---
