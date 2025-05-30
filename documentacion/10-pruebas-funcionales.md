## Pruebas funcionales y técnicas

### Pruebas funcionales

Con el objetivo de validar que las funcionalidades implementadas en la aplicación **MiMascota** cumplen con los requisitos establecidos, se realizaron pruebas funcionales manuales centradas en la interacción del usuario final con la interfaz del sistema.

#### Funcionalidades evaluadas:

- Inicio de sesión y registro de usuario.
- Registro de refugio y acceso al dashboard.
- Visualización de mascotas disponibles para adopción.
- Solicitud de adopción por parte del usuario.
- Respuesta a solicitudes por parte del refugio.
- Publicación de mascotas para adopción.
- Edición de perfil de usuario.
- Flujo de navegación entre páginas.

#### Metodología:

Para cada funcionalidad, se definieron escenarios de prueba donde se documentó:

- Acción del usuario.
- Resultado esperado.
- Resultado obtenido.
- Estado final de la prueba.

#### Ejemplo de casos de prueba:

| Caso | Acción del Usuario | Resultado Esperado | Resultado Obtenido | Estado |
|------|---------------------|---------------------|---------------------|--------|
| 1 | Usuario se registra desde `SignUp.jsx` con datos válidos | Usuario es redirigido al inicio de sesión | Redirección exitosa | Aprobado |
| 2 | Usuario inicia sesión con credenciales correctas en `SignIn.jsx` | Acceso al sistema y redirección a `Home.jsx` | Redirección correcta y sesión iniciada | Aprobado |
| 3 | Usuario realiza solicitud de adopción desde `AnimalesAdopcion.jsx` | Solicitud registrada y confirmación en pantalla | Solicitud enviada y alerta de éxito mostrada | Aprobado |
| 4 | Refugio responde solicitud en `DashboardRefugio.jsx` | Solicitud actualizada correctamente | Confirmación visible en `RespuestaSolicitud.jsx` | Aprobado |

---

### Pruebas técnicas (rendimiento y calidad)

Para evaluar la eficiencia técnica del sistema, se realizaron pruebas de rendimiento enfocadas en tiempo de carga, uso de recursos y fluidez de navegación.

#### Herramientas utilizadas:

- **Google Lighthouse** para pruebas de rendimiento del frontend.
- **Chrome DevTools** para análisis de red y recursos.
- Pruebas manuales en diferentes navegadores (Chrome, Firefox) y dispositivos (PC, móvil).

#### Resultados obtenidos:

| Métrica | Resultado |
|---------|-----------|
| Tiempo de carga inicial (Home) | 1.7 s promedio |
| FPS durante navegación | Estable entre 55-60 FPS |
| Puntaje Lighthouse (Performance) | 88/100 |
| Uso de memoria en sesión prolongada | ~120 MB (estable) |
| Errores de consola | 0 errores críticos detectados |

---

### Conclusión

Las pruebas realizadas validan que **MiMascota** funciona correctamente desde el punto de vista funcional, cubriendo los flujos principales esperados por los usuarios y administradores (refugios). A nivel técnico, la aplicación ofrece una experiencia fluida, con buen rendimiento en carga inicial y navegación. Se recomienda implementar pruebas automatizadas (por ejemplo, con Cypress o Vitest) y realizar pruebas de carga si se planea escalar el sistema.



### Pasar a la siguiente sección: [Guia de estilo](11-guia-de-estilo.md)