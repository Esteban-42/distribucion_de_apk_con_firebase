# Distribución de APK Flutter con Firebase App Distribution

## Repositorio
https://github.com/Esteban-42/distribucion_de_apk_con_firebase

## Descripción
Proyecto Flutter desarrollado como ejercicio académico para generar, distribuir y probar versiones Android mediante Firebase App Distribution.

## Flujo de distribución

1. Desarrollo de la aplicación Flutter.
2. Generación del APK en modo Release.
3. Registro de la aplicación Android en Firebase.
4. Configuración de testers y grupos.
5. Carga del APK en App Distribution.
6. Distribución de la versión a los testers.
7. Instalación y pruebas en un dispositivo Android.
8. Generación y distribución de una actualización.

## Publicación

### Generar APK
```bash
flutter pub get
flutter build apk --release
```

Archivo generado:
`build/app/outputs/flutter-apk/app-release.apk`

### Distribuir mediante Firebase
1. Ingresar a Firebase Console.
2. Abrir App Distribution.
3. Seleccionar la aplicación Android.
4. Cargar el APK generado.
5. Escribir las Release Notes.
6. Seleccionar el grupo QA_Clase.
7. Distribuir la versión.

## Versionado

El versionado se define en `pubspec.yaml` mediante:

`version: versionName+versionCode`

Versiones utilizadas:
- 1.0.0+1: versión inicial.
- 1.0.1+2: actualización incremental.

## Release Notes

Las notas de publicación describen la versión, fecha, cambios realizados y propósito de las pruebas.

## Grupo de pruebas

Grupo: QA_Clase

Tester: dduran@uceva.edu.co

## Tecnologías utilizadas
- Flutter
- Dart
- Android
- Firebase App Distribution
- Git y GitHub