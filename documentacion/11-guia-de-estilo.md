# Guía de estilo de diseño

Con el fin de garantizar una interfaz coherente, accesible y visualmente agradable, se ha desarrollado una guía de estilo para la aplicación **MiMascota**, basada en buenas prácticas de diseño UX/UI. Esta guía define los elementos visuales clave que se aplican en todos los componentes de la interfaz.

### 🎨 Paleta de colores

Se utiliza una paleta principal en tonos verdes, asociada a la naturaleza y el bienestar de las mascotas, combinada con grises neutros y blancos para lograr un contraste armónico.

| Rol / Uso              | Color         | Hex       |
|------------------------|---------------|-----------|
| Primario               | Verde         | `#1AD659` |
| Secundario             | Verde claro   | `#3EE074` |
| Terciario              | Verde suave   | `#5FF791` |
| Cuaternario            | Verde pastel  | `#8CFFB3` |
| Fondo claro            | Verde muy suave | `#deffe9` |
| Fondo alterno claro    | Blanco verdoso | `#f0fff4` |
| Texto principal        | Negro         | `#000000` |
| Texto secundario       | Gris oscuro   | `#5c5c5c` |
| Bordes y líneas        | Gris medio    | `#c8c8c8` |
| Fondos neutros         | Gris claro    | `#eaeaea` |
| Elementos oscuros      | Gris oscuro fuerte | `#414141` |
| Sombra                 | Sutil         | `rgba(0, 0, 0, 0.1)` |

> Estos colores están definidos como variables CSS globales en el archivo de estilos, facilitando su uso consistente en todo el proyecto.

---

### 🖋 Tipografía

Se emplean dos fuentes principales, elegidas por su legibilidad y estilo moderno:

- **'Montserrat', sans-serif** – Usada para títulos y encabezados, aporta presencia y jerarquía visual.
- **'Open Sans', sans-serif** – Usada para párrafos, botones y texto general, por su legibilidad y simplicidad.

```css
--font-heading: 'Montserrat', sans-serif;
--font-body: 'Open Sans', sans-serif;
```

---

### Pasar a la siguiente sección: [Plan de Marketing](12-plan-de-marketing.md)