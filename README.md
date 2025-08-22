# MAXINC GPS - Traccar Manager Android

Aplicación Android para gestión de dispositivos GPS utilizando Traccar Server.

## 🚀 Características

- **Compatibilidad Android 15**: Target API 35
- **Gestión de dispositivos GPS**: Monitoreo en tiempo real
- **Interfaz web integrada**: Navegación web dentro de la aplicación
- **Soporte para múltiples dispositivos**: Gestión centralizada
- **Notificaciones push**: Alertas en tiempo real
- **Autenticación biométrica**: Seguridad mejorada

## 📱 Requisitos del Sistema

- **Android**: API 23+ (Android 6.0 Marshmallow)
- **Target**: API 35 (Android 15)
- **Compile**: API 36
- **Kotlin**: 2.2.10+
- **Gradle**: 8.14.3+

## 🛠️ Configuración del Proyecto

### Prerrequisitos

- Android Studio Hedgehog | 2023.1.1 o superior
- JDK 17
- Android SDK 36

### Instalación

1. Clona el repositorio:
```bash
git clone https://github.com/tomsilva/traccar-maxinc-2.0.git
cd traccar-maxinc-2.0
```

2. Abre el proyecto en Android Studio

3. Sincroniza el proyecto con Gradle

4. Ejecuta la aplicación en un dispositivo o emulador

## 🏗️ Estructura del Proyecto

```
app/
├── src/
│   ├── main/           # Código principal de la aplicación
│   ├── google/         # Configuración específica para Google Play
│   └── regular/        # Configuración para distribución general
├── build.gradle        # Configuración del módulo
└── proguard-rules.pro  # Reglas de ofuscación

build.gradle            # Configuración del proyecto
gradle.properties       # Propiedades de Gradle
```

## 🔧 Flavors de Build

### Regular
- Sin dependencias de Firebase
- Para distribución general
- Sin Crashlytics

### Google
- Con Firebase Analytics
- Con Firebase Crashlytics
- Con Firebase Messaging
- Para Google Play Store

## 📦 Dependencias Principales

- **AndroidX Core**: 1.16.0
- **Material Design**: 1.12.0
- **Lifecycle**: 2.9.2
- **Biometric**: 1.2.0-alpha05
- **MultiDex**: 2.0.1

## 🚀 Build y Deploy

### Build Debug
```bash
# Flavor regular
./gradlew assembleRegularDebug

# Flavor Google
./gradlew assembleGoogleDebug
```

### Build Release
```bash
# Flavor regular
./gradlew assembleRegularRelease

# Flavor Google
./gradlew assembleGoogleRelease
```

## 🔐 Configuración de Firebase

Para el flavor "google", asegúrate de tener:
- `google-services.json` en la raíz del módulo app
- Configuración de Firebase en el proyecto

## 📄 Licencia

Este proyecto está bajo la licencia especificada en el archivo LICENSE.txt.

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:

1. Fork el proyecto
2. Crea una rama para tu feature
3. Commit tus cambios
4. Push a la rama
5. Abre un Pull Request

## 📞 Soporte

Para soporte técnico o preguntas, contacta al equipo de desarrollo.

---

**Versión**: 1.0.07  
**Build**: 1007  
**Última actualización**: Enero 2025
