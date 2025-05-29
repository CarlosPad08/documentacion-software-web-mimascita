
### Pasar a la siguiente sección: [Monetizacion](16-monetizacion.md)

## 15. Optimización de rendimiento y carga

La aplicación "MiMascota" ha sido optimizada para tiempos de carga rápidos y experiencia fluida del usuario. 

### Acciones implementadas:
- Uso del bundler **Vite** que permite recarga rápida en desarrollo y construcción eficiente para producción.
- Implementación del formato **WebP** para imágenes clave, lo que reduce significativamente el tamaño de los recursos gráficos.
- Carga condicional de componentes: por ejemplo, el componente `SignIn` se renderiza solo si el usuario navega a la ruta `/signin`.
- Comandos `vite build` y `vite preview` utilizados para asegurar una versión final optimizada y minificada.

### Mejoras propuestas:
- Revisión de rutas de imágenes para evitar errores y permitir mejor caché del navegador.
- Agregar el atributo `loading="lazy"` en imágenes para mejorar el rendimiento inicial.
- Evaluación del tamaño del bundle mediante herramientas como `rollup-plugin-visualizer`.

---