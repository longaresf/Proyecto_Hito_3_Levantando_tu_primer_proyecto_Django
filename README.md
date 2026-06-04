# Django Core Routing & Views Architecture

Este repositorio contiene un proyecto desarrollado en **Python** con el framework **Django**, enfocado en la implementación y configuración de la capa de enrutamiento (*Routing*) y el procesamiento de vistas (*Views*). El objetivo principal de este desarrollo es estructurar el flujo de peticiones y respuestas HTTP del servidor, garantizando un puente limpio entre las URLs del cliente y la lógica de negocio del backend.

## 🚀 Características y Capacidades Técnicas

* **Arquitectura de Enrutamiento Modular:** Configuración y desacoplamiento de rutas utilizando el archivo principal `urls.py` e integrando de forma limpia las rutas internas de las aplicaciones mediante `include()`.
* **Control de Vistas (Views):** Implementación de lógica de servidor de Vistas Basadas en Clases - CBVs para procesar las solicitudes de los usuarios.
* **Renderizado de Contenido Dinámico:** Conexión de la capa de control con el sistema de plantillas de Django (*Django Templates*) para despachar interfaces web estructuradas.
* **Manejo de Respuestas HTTP:** Control de flujos web estándar, incluyendo códigos de estado, redirecciones y renderizado condicional.

## 🛠️ Stack Tecnológico

* **Lenguaje de Programación:** Python 3.x
* **Framework Backend:** Django 4.x / 5.x
* **Arquitectura:** MVT (Model-View-Template)
* **Entorno de Pruebas:** Django Dev Server

## ⚙️ Resolución del Flujo Web y Buenas Prácticas

El desarrollo se centró en resolver el ciclo de vida de una petición HTTP en una arquitectura monolítica:

1. **Resolución de URLs:** Se diseñaron expresiones y patrones de rutas legibles y amigables para el usuario (SEO-friendly), evitando configuraciones redundantes en el servidor central.
2. **Desacoplamiento de Lógica:** Aplicación del principio de responsabilidad única, separando estrictamente la declaración de rutas de la lógica que procesa los datos dentro de las vistas.
3. **Manejo de Contexto:** Inyección dinámica de variables y datos desde el backend hacia el frontend, permitiendo que la interfaz responda al estado actual de la aplicación.

## 🔧 Instrucciones de Configuración y Ejecución

Sigue estos pasos para clonar y ejecutar el servidor de pruebas de manera local:

1. **Clonar el repositorio:**
   ```bash
   git clone [https://github.com/longaresf/django-routing-views.git](https://github.com/longaresf/django-routing-views.git)
   ```
2. Ingresar al directorio del proyecto:
   Bash
   cd django-routing-views

3. Inicializar y activar el entorno virtual:
   Bash
   python -m venv venv
   source venv/bin/activate  # En Windows usa: venv\Scripts\activate

4. Instalar requerimientos del sistema:
   Bash
   pip install -r requirements.txt

5. Ejecutar el servidor local:
   Bash
   python manage.py runserver

   Accede a las rutas configuradas (http://127.0.0.1:8000) para verificar el procesamiento dinámico de las vistas.

✒️ Créditos y Contexto

    Francisco Longares - Desarrollador Backend Python - longaresf

    Este proyecto representa la resolución del hito práctico de enrutamiento y lógica de vistas dentro del programa de especialización Full Stack Python de Desafío Latam.
