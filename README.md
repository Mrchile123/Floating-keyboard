# ⌨️ Teclado Flotante (Floating Keyboard App)

Una aplicación nativa para Android que crea un botón flotante global. Este botón permanece visible por encima de otras aplicaciones y, al presionarlo, fuerza la aparición del teclado virtual del sistema.

## 🚀 Características
* **Botón Global:** Utiliza el permiso `SYSTEM_ALERT_WINDOW` para flotar sobre cualquier pantalla o aplicación.
* **Activación de Teclado:** Se comunica con el `InputMethodManager` de Android para desplegar el teclado al instante.
* **100% Limpia:** Código nativo en Java, sin rastreo y totalmente libre de anuncios.
* **Compilación en la Nube:** Construida automáticamente mediante GitHub Actions.

## 🛠️ Cómo descargar e instalar el .apk
Ya que este proyecto se compila automáticamente en los servidores de GitHub, no necesitas Android Studio ni Sketchware para obtener la aplicación.

1. Ve a la pestaña **[Actions]** en la parte superior de este repositorio.
2. Haz clic en la ejecución (workflow) más reciente que tenga un ✅ check verde.
3. Desliza hasta la parte inferior de esa página, a la sección de **Artifacts**.
4. Descarga el archivo `.apk` generado.
5. Pásalo a tu teléfono, concédele los permisos de instalación de orígenes desconocidos e instálalo.
6. Al abrir la app por primera vez, te pedirá el permiso de "Mostrar sobre otras aplicaciones". ¡Acéptalo y listo!

## 📂 Estructura del Código
* `app/src/main/java/.../MainActivity.java`: Solicita los permisos necesarios al usuario.
* `app/src/main/java/.../FloatingService.java`: Contiene la lógica del botón y la activación del teclado.
* `.github/workflows/build.yml`: Archivo de configuración que le dice a GitHub cómo compilar la app.
* 
