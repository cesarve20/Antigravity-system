# 🚀 Antigravity System - Panel de Control Espacial

![Estado](https://img.shields.io/badge/Estado-Terminado-success)
![Versión](https://img.shields.io/badge/Versión-1.0.0-blue)
![Tecnologías](https://img.shields.io/badge/Tech-HTML%20%7C%20CSS%20%7C%20JS-yellow)

Una aplicación web interactiva que simula un panel de control para una tripulación espacial. Este proyecto "Mini Full-Stack" gestiona autenticación de usuarios y persistencia de datos utilizando el almacenamiento local del navegador (`localStorage`), sin necesidad de bases de datos externas.

## 🔗 Demo en Vivo
Puedes ver el proyecto funcionando aquí: **[Enlace a tu Vercel aquí]**

## 📋 Características Principales

### 🔐 Autenticación y Seguridad
- **Sistema de Login y Registro:** Alternancia suave entre formularios sin recargar la página.
- **Validación de Datos:** Restricción de contraseñas (mínimo 6 caracteres).
- **UX de Seguridad:** Botón para mostrar/ocultar contraseña (👁️).
- **Gestión de Sesiones:** El sistema recuerda al usuario logueado y protege las rutas privadas.

### 🎛️ Dashboard Interactivo
- **Simulación en Tiempo Real:** Sensores de oxígeno, gravedad y velocidad con actualizaciones dinámicas.
- **Bitácora de Misión (To-Do List):**
  - Crear nuevas tareas.
  - Eliminar tareas completadas.
  - **Persistencia Multi-usuario:** Las tareas se guardan automáticamente y son únicas para cada usuario (las tareas de 'Juan' no las ve 'Maria').

### 🎨 Diseño y UI
- Interfaz moderna con temática espacial (Dark Mode).
- Animaciones CSS (efecto de flotación antigravedad).
- Diseño completamente responsivo (Mobile First).

## 🛠️ Tecnologías Utilizadas

Este proyecto fue construido utilizando **Vanilla JavaScript** (JS Puro) para demostrar una comprensión sólida de los fundamentos del desarrollo web sin frameworks.

- **HTML5:** Estructura semántica.
- **CSS3:** Flexbox, Animaciones (@keyframes), Variables y Diseño Responsivo.
- **JavaScript (ES6+):**
  - Manipulación del DOM.
  - Manejo de Eventos (`EventListeners`).
  - `localStorage` API para la base de datos simulada.
  - `setInterval` y `Math.random` para simulación de datos.

## 📂 Estructura del Proyecto

```text
/proyecto-antigravity
│
├── index.html          # Landing Page (Pública)
├── README.md           # Documentación
│
├── css/
│   └── style.css       # Estilos globales y temas
│
├── js/
│   ├── home.js         # Lógica de la página principal
│   ├── script.js       # Lógica de Autenticación (Login/Register)
│   └── dashboard.js    # Lógica del Panel de Control y Bitácora
│
└── pages/
    ├── auth.html       # Página de Acceso
    └── dashboard.html  # Página Privada (Requiere Login)