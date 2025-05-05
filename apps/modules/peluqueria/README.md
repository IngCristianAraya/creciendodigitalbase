# Peluqueria module
✂️ Módulo Peluquería y Barbería – Gestión de Turnos, Servicios y Clientes
Este módulo está pensado para negocios como peluquerías, barberías, salones de belleza y similares. Automatiza la atención, optimiza los tiempos y mejora la experiencia del cliente.

🧩 Funcionalidades Clave
📅 Agenda de turnos con horarios personalizados

👨‍🦰 Registro de clientes frecuentes y sus servicios

💈 Gestión de servicios (corte, tinte, afeitado, etc.)

💰 Control de ingresos diarios y caja

📢 Recordatorios por WhatsApp (opcional)

🔐 Corte de servicio por impago (modo killer)

/peluqueria/
├── frontend/
│   ├── app/
│   │   ├── (main)/        → Calendario, clientes, ventas
│   │   └── public/        → Página de marketing
│   └── lib/
│       ├── api/
│       └── features/
│
├── backend/
│   ├── src/
│   │   ├── features/
│   │   │   ├── appointments/
│   │   │   ├── clients/
│   │   │   └── services/
│   │   └── shared/
│   └── tests/
│
└── features/
    ├── services/
    ├── appointments/
    └── clients/


🧰 Stack Tecnológico
Frontend: Next.js + TailwindCSS + Zustand

Backend: NestJS + PostgreSQL + Prisma

Facturación: Microservicio global billing-service

Pagos: Integración Yape / Plin / Efectivo

Desconexión: Soporte offline vía Electron opcional

🎯 Enfoque Comercial
👨‍👩‍👧‍👦 Clientes objetivo: negocios familiares, independientes o pequeños salones.

🧾 Modalidad de cobro: mensual (SaaS) o compra única (versión offline).

🧨 Ventaja competitiva: cero complejidad, lista para usar desde el primer día.



💇 Sistema para Peluquería y Barbería
Este módulo está diseñado para peluquerías, barberías y salones de belleza que necesitan organizar sus citas, servicios, personal y ventas. Pensado para pequeños negocios que buscan digitalizar su operación con una interfaz simple y adaptable a tablets o móviles.

Funcionalidades principales
Agenda de citas: Calendario diario/semanal, gestión de reservas por cliente y por colaborador.

Servicios personalizados: Corte, tinte, depilación, tratamientos. Configuración de duración, precio, insumos usados.

Gestión de colaboradores: Registro de barberos/estilistas, asignación de horarios, comisiones por servicio.

Ventas y caja: Registro de servicios vendidos, venta de productos (shampoo, cremas), corte de caja diario.

Control de insumos: Descuento de inventario según servicio, alertas de reposición.

Clientes: Historial de visitas, servicios frecuentes, notas personalizadas.

Promociones y paquetes: Descuentos por combo, membresías semanales o mensuales.

Soporte para pagos QR: Integración con Yape, Plin, pago en efectivo.

Tecnologías utilizadas
Frontend: React + Next.js App Router + Tailwind CSS

Backend: NestJS + Prisma

Base de datos: PostgreSQL

Mobile-first: Diseño optimizado para tablets y móviles

Pagos: QR estático y dinámico

Estado actual
✅ Definición de modelos: Appointment, Service, Stylist, Product, CashMovement, Client
📅 Interfaz de agenda en desarrollo
🚧 Próximas tareas:

Agregar módulo de comisiones

Mejora de interfaz responsive

Enlace directo con WhatsApp para confirmación de citas