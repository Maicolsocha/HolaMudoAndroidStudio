HolaMudoAndroidStudio

Una aplicación "Hola Mundo" minimalista para Android, escrita en Kotlin y basada en Jetpack Compose.

Capturas de pantalla

(Añade tu propia captura en la carpeta docs/ o elimina esta sección)

Características

Aplicación de una sola pantalla que muestra el saludo «¡Hola Mundo!».

Construida con Jetpack Compose (UI declarativa sin archivos XML).

Compatible desde API 24 (Android 7.0) en adelante.

Uso de componentes Material 3.

Proyecto configurado íntegramente con Gradle Kotlin DSL (build.gradle.kts).

Primeros pasos

Requisitos previos

Herramienta

Versión mínima

Android Studio

Iguana

Android SDK

24

JDK

11

Clonar el repositorio

git clone https://github.com/Maicolsocha/HolaMudoAndroidStudio.git
cd HolaMudoAndroidStudio

Ejecutar la aplicación

Abre Android Studio → File ▸ Open… y selecciona la carpeta raíz del proyecto.

Espera a que Gradle termine de sincronizar las dependencias.

Haz clic en Run ▶️ y elige un emulador o un dispositivo físico.

Desde la línea de comandos:

./gradlew installDebug
adb shell am start -n com.example.primera/.MainActivity

Estructura del proyecto

.
├── app/
│   ├── src/
│   │   └── main/
│   │       ├── java/com/example/primera/MainActivity.kt
│   │       ├── java/com/example/primera/Hola \Mundo.kt
│   │       └── res/…
├── build.gradle.kts
└── settings.gradle.kts

Cómo funciona

MainActivity.kt define el contenido de la ventana con Greeting("Mundo"), una función composable que muestra «¡Hola Mundo!» en pantalla. Toda la interfaz se genera con Jetpack Compose, por lo que no se requieren diseños XML.

Comandos útiles

Tarea

Comando

Generar APK de debug

./gradlew assembleDebug

Ejecutar pruebas unitarias

./gradlew testDebug

Limpiar el proyecto

./gradlew clean

Contribuir

¡Se agradecen los pull requests! Para cambios importantes, abre primero un issue y comenta lo que te gustaría modificar.

Licencia

Este proyecto aún no tiene licencia. Si planeas usarlo o distribuirlo, considera añadir una licencia de código abierto (p. ej., MIT, Apache‑2.0).
