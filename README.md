# App1 — Aplicación Móviles

![Android](https://img.shields.io/badge/Android-API%2034%2B-3DDC84?style=flat&logo=android&logoColor=white)
![Java](https://img.shields.io/badge/Java-11-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-9.2.1-02303A?style=flat&logo=gradle&logoColor=white)
![Material Design](https://img.shields.io/badge/Material%20Design-3-757575?style=flat&logo=material-design&logoColor=white)
![Lottie](https://img.shields.io/badge/Lottie-6.7.1-00DDB3?style=flat)

Aplicación Android desarrollada para la actividad de la materia de Aplicaciones Móviles "A". Implementa un flujo de autenticación con pantalla de introducción, inicio de sesión y registro de usuarios.

---

## Pantallas

| Pantalla | Descripción |
|---|---|
| **Intro** | Splash screen con animación Lottie (robot), logo UTEQ y botón "Entrar" |
| **Login** | Formulario de correo y contraseña con acceso mediante Google, Facebook y GitHub |
| **Registro** | Formulario completo: nombres, apellidos, correo, teléfono, fecha de nacimiento, tipo de documento, número de documento y género |

---

## Tecnologías

- **Lenguaje:** Java
- **SDK mínimo:** API 34 (Android 14)
- **SDK objetivo:** API 36
- **Gradle:** 9.2.1 (AGP)

### Dependencias principales

| Librería | Versión | Uso |
|---|---|---|
| `androidx.appcompat` | 1.7.1 | Compatibilidad con versiones anteriores de Android |
| `com.google.android.material` | 1.13.0 | Componentes Material Design (TextInputLayout, botones) |
| `androidx.constraintlayout` | 2.2.1 | Layout de posicionamiento por restricciones |
| `com.airbnb.android:lottie` | 6.7.1 | Animaciones JSON en la pantalla intro |
| `androidx.activity:activity-ktx` | 1.13.0 | Extensiones de Activity |

---

## Estructura del proyecto

```
App1/
├── app/
│   └── src/
│       └── main/
│           ├── java/com/uteq/software/app1/
│           │   ├── MainActivity.java        # Pantalla de introducción
│           │   └── RegistroUsuario.java     # Pantalla de registro
│           ├── res/
│           │   ├── layout/
│           │   │   ├── activity_act_intro.xml
│           │   │   ├── activity_act_login.xml
│           │   │   └── activity_registro_usuario.xml
│           │   ├── drawable/                # Íconos e imágenes (logos UTEQ/FCC)
│           │   └── raw/
│           │       └── robot.json           # Animación Lottie
│           └── AndroidManifest.xml
├── gradle/
│   └── libs.versions.toml                   # Catálogo de versiones
└── build.gradle
```

---

## Requisitos previos

- Android Studio Meerkat o superior
- JDK 11
- Dispositivo o emulador con Android 14+ (API 34)

---

## Instalación y ejecución

1. Clonar el repositorio:
   ```bash
   git clone https://github.com/ereinosov/App1.git
   ```
2. Abrir el proyecto en Android Studio: **File → Open → seleccionar carpeta `App1`**
3. Sincronizar Gradle: **File → Sync Project with Gradle Files**
4. Ejecutar en emulador o dispositivo: **Run → Run 'app'** (o `Shift + F10`)

---

## Autor

**Eduardo Reinoso Vélez**  
Facultad de Ciencias de la Computación - Software — UTEQ  
© 2026
