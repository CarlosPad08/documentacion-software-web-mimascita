---

## 🔐 14. Implementación de Seguridad Básica – *MiMascota*

La seguridad es un componente fundamental de **MiMascota**, especialmente por el manejo de datos personales de usuarios, veterinarias y fundaciones. Para garantizar la integridad y confidencialidad de la información, se han implementado medidas de seguridad esenciales que cumplen con los estándares mínimos recomendados para el software Mimascota.

---

### 🔑 Autenticación de Usuarios

* Implementación de un sistema de **autenticación robusto** mediante **JWT (JSON Web Tokens)**.
* Los tokens son generados al iniciar sesión y permiten la verificación de identidad en cada solicitud protegida, sin exponer credenciales.
* Los endpoints sensibles están protegidos para garantizar el acceso solo a usuarios autenticados.

---

### 🧾 Manejo Seguro de Contraseñas

* Las contraseñas de los usuarios se almacenan utilizando **encriptación segura con hashing (bcrypt)**.
* El sistema no guarda contraseñas en texto plano en ningún momento.
* Se aplican buenas prácticas como verificación de fortaleza de contraseña al momento del registro.

---

### 🛡️ Protección de Datos Personales

* Solo se recolecta la información estrictamente necesaria para el funcionamiento de la aplicación.
* Se han definido políticas básicas de privacidad y control de acceso por roles (usuario común, veterinaria, fundación).

---

### 🔐 Uso de Tokens y Sesiones Seguras

* Los **tokens de sesión (JWT)** incluyen tiempos de expiración para limitar accesos prolongados sin autenticación.
* Se maneja **renovación de tokens** y verificación en el backend para evitar accesos no autorizados.


---

### 🧪 Validaciones y Control de Errores

* Se realizan **validaciones de entrada** para prevenir ataques como inyecciones de código (XSS, SQL Injection).
* El sistema maneja adecuadamente los errores sin exponer detalles del backend al usuario.
* Se emplean middleware y librerías de validación para asegurar que todos los datos recibidos cumplen con formatos esperados.

---



