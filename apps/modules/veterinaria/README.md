# Veterinaria module
🐾 Módulo Veterinaria – Gestión de Consultas, Clientes y Mascotas
Este módulo está diseñado para clínicas veterinarias y consultorios independientes, con funcionalidades adaptadas a su día a día. Es parte integral de la plataforma SaaS multinicho.

✨ Funcionalidades Principales
🐶 Registro completo de mascotas y dueños

📅 Agenda de citas con recordatorios automáticos

🧾 Historial clínico por mascota

💊 Gestión de productos veterinarios y stock

💸 Control de ventas y cobros

📢 Notificaciones por WhatsApp (recordatorio de citas)

🔐 Corte automático de servicio si no hay pago

/veterinaria/
├── frontend/
│   ├── app/
│   │   ├── (main)/       → Pacientes, citas, historial
│   │   └── public/       → Página de venta del sistema
│   └── lib/
│       ├── api/
│       └── features/
│
├── backend/
│   ├── src/
│   │   ├── features/
│   │   │   ├── appointments/
│   │   │   ├── pets/
│   │   │   └── owners/
│   │   └── shared/
│   └── tests/
│
└── features/
    ├── pets/
    ├── owners/
    └── appointments/


🛠️ Tecnologías Utilizadas
Frontend: Next.js + TailwindCSS + Zustand

Backend: NestJS + PostgreSQL + Prisma

Notificaciones: Integración con WhatsApp API

Facturación: Conexión con módulo global de billing

Corte de servicio: Kill-switch gestionado por microservicio

📈 Próximas Mejoras
📷 Ficha clínica con imágenes de procedimientos

💉 Calendario de vacunación con alertas

🧾 Reportes tributarios adaptados a SUNAT

📱 Modo móvil veterinario (consultas a domicilio)

🐾 Sistema para Clínicas Veterinarias
Este módulo forma parte de la plataforma SaaS y está diseñado específicamente para cubrir las necesidades de clínicas veterinarias en Perú y Latinoamérica. Permite a veterinarios gestionar pacientes, historial médico, citas, pagos y comunicación con clientes, todo en una interfaz moderna y fácil de usar.

Funcionalidades principales
Gestión de pacientes (mascotas): Registro con raza, edad, peso, foto, historial clínico y dueño asociado.

Historia clínica: Evoluciones médicas por fecha, tratamiento, diagnóstico y medicamentos administrados.

Agendamiento de citas: Calendario interactivo, con confirmación vía WhatsApp o correo.

Facturación electrónica: Integración con Sunat (opcional) y generación de boletas/facturas simples.

Recordatorios automáticos: Alertas de vacunación y seguimiento post consulta.

Modo offline (opcional): Versión de escritorio con Electron para zonas sin buena conexión.

Tecnologías utilizadas
Frontend: React + Next.js + Tailwind CSS

Backend: NestJS + Prisma

DB: PostgreSQL

Pasarela de pago: Yape/Plin opcional para cobros rápidos

Infraestructura: Docker, Turborepo, CI/CD

Estado actual
✅ En desarrollo inicial
📅 Próximas tareas:

Crear modelos Pet, Owner, Appointment, Visit

Conectar módulo de recordatorios del notification-service

Integrar pagos con Yape