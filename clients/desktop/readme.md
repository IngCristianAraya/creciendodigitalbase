🖥️ Cliente de Escritorio – Plataforma Offline con Electron
Este módulo contiene la estructura base para compilar y distribuir versiones de escritorio de los sistemas SaaS, diseñados especialmente para negocios que requieren operar sin conexión a internet (modo offline).

🎯 ¿Para quién es?
Ideal para negocios como:

Minimarkets y tiendas en mercados sin WiFi estable

Psicólogos con consultorio sin internet

Comercios rurales

Clientes que prefieren pago único por software offline

⚙️ Estructura General
/desktop/
├── main/                     → Código del proceso principal de Electron
│   └── preload.ts           → Comunicación segura entre renderer y Node
│
├── renderer/                → Interfaz de usuario (React + Vite)
│   ├── src/
│   │   ├── pages/
│   │   ├── components/
│   │   └── lib/
│   └── index.html
│
├── public/
│   └── icon.png             → Ícono de la app
│
├── package.json             → Configuración de Electron
└── vite.config.ts           → Configuración de frontend


📦 Características Técnicas
🔧 Electron 28+ con contexto aislado (contextBridge)

⚡ Vite + React para interfaz rápida

🔌 Comunicación local con SQLite (opcional) o IndexedDB

🌐 Sincronización automática con backend al recuperar conexión

🧱 Instaladores .exe y .dmg listos para empaquetar

🧠 Ventajas
🛑 Funciona sin conexión: ideal para lugares remotos o inestables

💰 Se puede vender como licencia única con activación manual

🛠️ Actualizaciones controladas vía USB o patch por email

🔐 Datos locales encriptados

🚀 Flujo de Instalación
El usuario instala el .exe o .dmg

Al primer uso, se registra una licencia local

La app funciona en modo local con almacenamiento persistente

Al detectar internet, se sincroniza con el backend (opcional)

