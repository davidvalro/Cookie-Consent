## 🍪 Modal de Cookie Consent Engañosa

### 📝 Sobre Este Proyecto

Este es un proyecto enfocado al desarrollo *frontend* diseñado para explorar y poner en práctica la **manipulación del DOM** y la **gestión de eventos** utilizando únicamente JavaScript puro. Su objetivo es simular un modal de "**cookie** consent" que intencionalmente incorpora patrones de diseño oscuros (*dark patterns*), sirviendo como un excelente ejercicio de control total sobre la interfaz de usuario.

---

### 🌟 Cómo Funciona (Funcionalidades Clave)

El modal incorpora varios trucos de interacción para demostrar el control total que tenemos sobre la interfaz:

| Característica | ¿Qué Hace? | Archivos Principales |
| :--- | :--- | :--- |
| **Aparece Solo** | El modal se muestra automáticamente 1.5 segundos después de que la página carga, usando un temporizador (`setTimeout`). | `index.js` |
| **El Truco del Botón** | Si intentas hacer *hover* sobre el botón "Decline," este inmediatamente intercambia su lugar con el botón "Accept". | `index.js`, `index.css` |
| **Simulación de Venta** | Tras aceptar el formulario, se inicia una simulación que dura 3 segundos. El modal muestra mensajes progresivos para imitar un proceso de carga y venta de datos en dos etapas. | `index.js` |
| **Cierre Bloqueado** | El botón de cierre (`X`) permanece desactivado al principio y solo se habilita una vez que la simulación de 3 segundos ha finalizado, forzando al usuario a ver todo el proceso. | `index.js`, `index.html` |
| **Mensaje Personalizado**| El mensaje final del modal es dinámico: utiliza el nombre que el usuario introdujo en el formulario (`FormData`) para un toque más personal. | `index.js` |

---

### 💻 Herramientas Utilizadas

* **Lógica:** JavaScript (Vanilla)
* **Estructura:** HTML5
* **Estilos:** CSS3
* **Entorno de Desarrollo:** Vite

---

### ▶️ Instrucciones para Ponerlo en Marcha

Si quieres ver el proyecto en tu máquina:

1.  **Instala las dependencias necesarias**:
    ```bash
    npm install
    ```
2.  **Inicia la aplicación** en el servidor de desarrollo local:
    ```bash
    npm start
    # o si lo prefieres, npm run dev
    ```

---

### 👨‍💻 Nota del Desarrollador

Este ejercicio, realizado originalmente como parte de un curso en línea, fue excelente para afianzar conceptos fundamentales del desarrollo *frontend*. Me permitió trabajar directamente con la **manipulación del estado visual** y gestionar **flujos asíncronos** (simulados con `setTimeout`), algo crucial para cualquier comunicación con el *backend*. Además, se demuestra un manejo limpio de la captura de datos del usuario con los *event listeners* y la API `FormData`.