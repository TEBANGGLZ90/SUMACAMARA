# Suma con Cámara

App Android simple: apuntas la cámara a una fila de números y la app muestra la suma.

- Kotlin + CameraX + ML Kit (OCR en el dispositivo, sin internet)
- minSdk 26, targetSdk 36 (funciona en Android 17)
- Detecta los números de la fila horizontal con más cifras en la imagen
- Botón **Congelar** para fijar el resultado y **Reanudar** para seguir leyendo
- Acepta enteros y decimales (`3.5` o `3,5`) y miles (`1,200`). No lee negativos.

## Obtener el APK

**Opción A: GitHub (sin instalar nada)**
1. Crea un repositorio y sube esta carpeta.
2. Pestaña *Actions* → *Build APK* → *Run workflow*.
3. Al terminar, descarga el artefacto `SumaCamara-APK` (contiene `app-debug.apk`).

**Opción B: Android Studio**
1. *File → Open* y elige esta carpeta; espera la sincronización de Gradle.
2. *Build → Build Bundle(s) / APK(s) → Build APK(s)*.
3. El archivo queda en `app/build/outputs/apk/debug/app-debug.apk`.

## Instalar

Pasa el APK al celular y ábrelo; Android pedirá permitir instalar apps de origen desconocido.
