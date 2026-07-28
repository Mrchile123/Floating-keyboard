# ⌨️ Teclado Flotante (Floating Keyboard)

Una aplicación nativa para Android diseñada para invocar el teclado virtual del sistema desde cualquier pantalla mediante un botón flotante superpuesto. 

## 📌 ¿Qué es?
Es una herramienta ligera, de código abierto y libre de anuncios que facilita el acceso rápido al teclado en cualquier momento. Al ejecutarse, la aplicación despliega un botón persistente que se mantiene visible por encima de otras aplicaciones (como navegadores, juegos o redes sociales). 

## ⚙️ ¿Cómo funciona?
El proyecto está construido en Java y utiliza componentes nativos del sistema Android para lograr su objetivo:
* **Servicio en Segundo Plano:** Utiliza un `Service` (`FloatingService`) para mantener el botón activo sin necesidad de tener la interfaz principal de la aplicación abierta.
* **Superposición de Pantalla:** Implementa la clase `WindowManager` y solicita el permiso `SYSTEM_ALERT_WINDOW` para dibujar la vista del botón por encima de la interfaz gráfica del sistema operativo.
* **Invocación del Teclado:** Se comunica directamente con el `InputMethodManager` de Android para forzar el despliegue del panel del teclado virtual al registrar un toque (click) en el botón flotante.
* 
