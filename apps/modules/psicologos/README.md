# Psicologos module
🧠 Módulo Psicólogos y Terapeutas – Gestión de Pacientes, Citas y Seguimiento
Este módulo está diseñado para profesionales de la salud mental como psicólogos clínicos, terapeutas, coach de vida, entre otros. Permite organizar consultas, llevar un historial ordenado de pacientes y automatizar tareas administrativas sin complicaciones.

🧩 Funcionalidades Clave
📅 Agenda de citas con recordatorios automáticos

🧾 Historia clínica por paciente (sesiones, diagnósticos, progreso)

👩‍⚕️ Panel para registrar notas y evaluaciones por sesión

💰 Control de pagos por consulta (efectivo o transferencia)

🛑 Corte automático por impago (modo killer)

📲 Versión web, móvil o de escritorio (sin internet)

/psicologos/
├── frontend/
│   ├── app/
│   │   ├── (main)/        → Pacientes, agenda, progreso
│   │   └── public/        → Página de presentación del profesional
│   └── lib/
│       ├── api/
│       └── features/
│
├── backend/
│   ├── src/
│   │   ├── features/
│   │   │   ├── patients/
│   │   │   ├── appointments/
│   │   │   └── sessions/
│   │   └── shared/
│   └── tests/
│
└── features/
    ├── appointments/
    ├── patients/
    └── sessions/


🧰 Stack Tecnológico
Frontend: Next.js 14 (app router) + Tailwind + Zustand

Backend: NestJS + Prisma + PostgreSQL

Pagos: Yape, Plin o efectivo con seguimiento manual

Facturación: Microservicio global billing-service

Comunicaciones: Recordatorios vía WhatsApp (opcional)

Offline: Versión Electron disponible

🎯 Enfoque Comercial
🎯 Público objetivo: psicólogos particulares, consultorios pequeños, terapias alternativas.

💵 Modalidad: mensual en la nube o licencia única offline.

🧩 Escalable: posibilidad de integrar videollamadas en futuras versiones.

