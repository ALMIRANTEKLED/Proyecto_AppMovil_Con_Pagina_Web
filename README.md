# Proyecto_AppMovil_Con_Pagina_Web

# 🎭 Tu Folklore – Sistema de Alquiler de Trajes Típicos

Este proyecto consiste en una **página web informativa** y una **aplicación móvil Flutter**, ambas conectadas a una base de datos Firebase. El sistema permite **visualizar trajes típicos bolivianos** y realizar **reservas de alquiler en tiempo real**, ya sea desde la web o desde la app móvil.

---

## 📦 Características del Proyecto

- 🌐 Página web desarrollada con **Django**, permite:
  - Ver los trajes disponibles.
  - Reservar un traje seleccionado.
  - Guardar las reservas en **Firebase Firestore**.

- 📱 App móvil desarrollada con **Flutter**:
  - Muestra los trajes con imágenes almacenadas en **Firebase Storage**.
  - Permite seleccionar una danza, ver sus trajes y reservarlos.
  - Toda la información se sincroniza automáticamente con **Firebase**.

---

## 🚀 Requisitos de instalación

### 🖥️ Para la página web (Django)

1. Asegúrate de tener instalado **Python** y **pip**.
2. Crea y activa un entorno virtual:
   ```bash
   python -m venv venv
   venv\Scripts\activate
   ```
3. Instala los paquetes necesarios:
   ```bash
   pip install -r requirements.txt
   pip install firebase-admin
   ```
4. Coloca tu archivo de credenciales Firebase en la raíz de tu app Django (por ejemplo: `firebase_key.json`).

### 📲 Para la app móvil (Flutter)

1. Tener instalado Flutter:  
   - https://docs.flutter.dev/get-started/install
2. Abrir el proyecto en **Visual Studio Code** (o Android Studio).
3. Ejecutar:
   ```bash
   flutter pub get
   flutter run
   ```

---

## 🔧 Conexión con Firebase

Tanto la app como el backend están conectados a:

- **Firebase Firestore**: Para guardar y consultar reservas en tiempo real.
- **Firebase Storage**: Para alojar imágenes de los trajes.

> 💡 Asegúrate de habilitar Firestore y Storage desde la [Firebase Console](https://console.firebase.google.com/) y asignar las reglas correctas para acceso (modo prueba o con autenticación si lo deseas).

---

## 📁 Estructura del Proyecto

```
/Proyecto final/
│
├── app/                    # Proyecto Django
│   ├── alquiler/           # App principal con views y conexión a Firebase
│   ├── static/img/         # Imágenes para la web
│   └── templates/          # index.html y otros
│
├── flutter_app/            # Proyecto Flutter para móvil
│
└── firebase_key.json       # Clave privada de Firebase
```

---
## ✅ ¿Qué hace cada parte?

| Plataforma | Función |
|-----------|---------|
| 🌐 Web     | Mostrar imágenes de trajes, permitir reservas simples |
| 📱 Móvil   | Visualizar, explorar y reservar trajes con experiencia completa |
| ☁️ Firebase | Conecta y sincroniza los datos en tiempo real entre web y app |
---
