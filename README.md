# 📋 Asignaciones — Conferencia de Estaca

Aplicación web para gestionar las asignaciones de la Conferencia de Estaca.  
Permite crear el registro de participantes, generar cartas de invitación personalizadas y exportarlas como PDF o imagen.

---

## ✨ Funcionalidades

- **Registro de asignaciones** — Director, Pianista, Mensajes, Testimonios, Capacitaciones, Oraciones, Especiales (Presidente de Misión / Templo)
- **Generación de cartas** — Carta personalizada por asignado con saludo, sesión, himnos y cierre firmado
- **Exportación** — Descarga en PDF (alta resolución) e imagen PNG
- **Control de seguimiento** — Registro de aviso, confirmación y reconfirmación por participante
- **Sesiones** — Adultos, Líderes y General, con horarios configurables
- **Drag & drop** — Reordenamiento de filas en el registro
- **Tipografía LDS** — Fuente McKay para las cartas impresas

---

## 🛠️ Tecnologías

| Recurso | Versión |
|---|---|
| HTML / CSS / JavaScript | Vanilla (sin frameworks) |
| [jsPDF](https://github.com/parallax/jsPDF) | 2.5.1 |
| [html2canvas](https://html2canvas.hertzen.com/) | 1.4.1 |
| Fuente McKay LDS | local |

---

## 🚀 Uso local

1. Clonar o descargar el repositorio.
2. Abrir `index.html` en cualquier navegador moderno.
3. No requiere servidor ni instalación.

> Los datos se guardan en `localStorage` del navegador. Para almacenamiento en la nube se recomienda integrar Firebase Firestore (ver sección de despliegue).

---

## ☁️ Despliegue recomendado

**Firebase Hosting + Firestore** es la opción recomendada para tener hosting y base de datos en la nube dentro de una sola plataforma.

Pasos básicos:
```bash
npm install -g firebase-tools
firebase login
firebase init        # seleccionar Hosting + Firestore
firebase deploy
```

---

## 📁 Estructura

```
/
├── index.html          # Aplicación completa (HTML + CSS + JS)
├── font/
│   └── McKay ldsLat Regular.otf
├── images/
│   └── fondo-estaca.b64.txt
└── README.md
```

---

## © Licencia

Copyright © 2025–2026 David Montecinos. Todos los derechos reservados.  
Consultar el archivo [COPYRIGHT](./COPYRIGHT) para más detalles.
