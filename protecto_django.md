# 🚀 Proyecto Django 6.0 - Guía de Instalación

Este documento describe paso a paso cómo configurar el entorno de desarrollo e iniciar un proyecto utilizando **Django 6.0**.

---

## 📌 1. Requisitos Previos

Antes de comenzar, asegúrate de tener instalado:

- **Python 3.10 o superior**
- **pip**: gestor de paquetes de Python

Puedes verificar las versiones instaladas con:

```bash
python --version
pip --version
```

---

## 🧱 2. Entorno Virtual
#modificar cn palabras propias
El entorno virtual, también conocido como `venv`, permite crear un espacio aislado para instalar las librerías del proyecto.

### ¿Para qué sirve?

Sirve para evitar conflictos entre versiones de librerías de diferentes proyectos.

Por ejemplo:

- Un proyecto puede usar Django 5.0.
- Otro proyecto puede usar Django 6.0.

Gracias al entorno virtual, ambos proyectos pueden existir en la misma computadora sin interferir entre sí.

---

## ⚙️ 3. Crear el Entorno Virtual

Desde la carpeta raíz del proyecto, ejecuta:

```bash
python -m venv venv
```

Esto creará una carpeta llamada `venv/`.

---

## ▶️ 4. Activar el Entorno Virtual

### En Windows

```bash
.\venv\Scripts\activate
```

### En Linux o macOS

```bash
source venv/bin/activate
```

Cuando el entorno virtual esté activado, normalmente verás algo como esto al inicio de la terminal:

```bash
(venv)
```

---

## 📦 5. Archivo de Dependencias

Crea un archivo llamado:

```txt
requirements.txt
```

Este archivo debe estar ubicado en la raíz del proyecto.

Su función es guardar todas las librerías necesarias para que el proyecto funcione correctamente.

---
```txt
.
├── README.md
├── manage.py
├── mi_sitio
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── protecto_django.md
└── requirements.txt
```

![image](/captura%20m6_l2%20django.PNG) 

Qué diferencia hay entre un "proyecto" y una "aplicación" en Django?

Qué carpetas se generan dentro de la app principal?

```python
INSTALLED_APPS = [
    "django.contrib.admin",
    "django.contrib.auth",
    "django.contrib.contenttypes",
    "django.contrib.sessions",
    "django.contrib.messages",
    "django.contrib.staticfiles",
    "principal",
]
```