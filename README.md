# ALPHA AI — Android starter project

**Version:** 0.1.0  
**Package:** `com.alpha.assistant`  
**Minimum Android:** 8.0 (API 26)  
**Target SDK:** 35

## Qué funciona en esta primera base

- Interfaz Android nativa con estética holográfica azul.
- Navegación entre Inicio, Chat, Módulos y Ajustes.
- Chat local básico con respuestas de demostración.
- Entrada de voz usando el servicio de reconocimiento instalado en Android.
- Salida de voz usando Text-to-Speech de Android.
- No necesita cuenta ni clave API para abrir y probar esta versión.

## Qué NO está implementado todavía

Esta versión no debe confundirse con el ALPHA final. Aún no incluye:
- Conexión real a Gemini, ChatGPT u otro proveedor online.
- Modelo LLM local integrado.
- Selector garantizado de voces masculinas/femeninas (depende de voces instaladas en Android).
- Automatización de ajustes del teléfono.
- Editor/compilador de aplicaciones ni sistema real de extensiones.
- Acceso universal a otras aplicaciones o al sistema.

Estas funciones requieren integración, permisos, pruebas y, en algunos casos, servicios externos.

## Compilar en GitHub desde Windows o Android

1. Crea una cuenta en https://github.com
2. Crea un repositorio nuevo llamado `ALPHA`.
3. Sube **todo el contenido de esta carpeta** a la rama `main` (no subas la carpeta contenedora como una sola carpeta).
4. En GitHub abre la pestaña **Actions**.
5. Selecciona **Build ALPHA APK**.
6. Pulsa **Run workflow** si no se inició automáticamente.
7. Espera a que termine el trabajo. Si aparece un error, abre el trabajo y copia el registro completo.
8. En la parte inferior de la ejecución, descarga el artefacto `ALPHA-debug-apk`.
9. Descomprime el artefacto y encontrarás `app-debug.apk`.

## Compilar localmente en Windows

Requiere Android Studio, Android SDK, JDK 17 y Gradle 8.9.
Abre la carpeta del proyecto en Android Studio y permite que Gradle sincronice.
Luego ejecuta la tarea `app > Tasks > build > assembleDebug`.
El APK queda en `app/build/outputs/apk/debug/app-debug.apk`.

## Seguridad

- No se incluyen claves API ni contraseñas.
- No se solicita acceso root.
- La captura de voz solo se solicita al pulsar el botón de micrófono.
- Las órdenes no modifican automáticamente ajustes del sistema.
