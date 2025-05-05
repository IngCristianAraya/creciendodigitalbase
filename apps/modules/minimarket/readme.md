🏪 Módulo Minimarket – Sistema de Ventas e Inventario
Este módulo forma parte de la plataforma SaaS multinicho y está diseñado específicamente para pequeños minimarkets, bodegas y tiendas de abarrotes. Su propósito es ofrecer una solución moderna, intuitiva y accesible para llevar el control del negocio.

✨ Funcionalidades Principales
📦 Gestión de productos con stock mínimo

🧾 Registro rápido de ventas con boleta/ticket

📊 Reportes diarios, semanales y mensuales

🧍 Control de usuarios (cajeros, admin)

💸 Integración con pagos vía Yape, Plin

⚠️ Alertas de bajo stock y productos por vencer

🔐 Corte automático si no se paga la membresía (modo killer)


/minimarket/
├── frontend/             → UI con Next.js
│   ├── app/
│   │   ├── (main)/       → Dashboard, productos, ventas
│   │   └── public/       → Landing específica del rubro
│   └── lib/              → Funciones y SDK locales
│
├── backend/              → Lógica de negocio con NestJS
│   ├── src/
│   │   ├── features/
│   │   │   ├── inventory/
│   │   │   └── sales/
│   │   └── shared/
│   └── tests/
│
└── features/             → Arquitectura limpia
    ├── inventory/
    │   ├── domain/
    │   ├── application/
    │   └── infrastructure/
    └── sales/


🛠️ Tecnologías Utilizadas
Frontend: Next.js 14 App Router, TailwindCSS, Zustand

Backend: NestJS, Prisma ORM, PostgreSQL

API SDK: auto-generado y compartido con otros módulos

Pruebas: Vitest + Playwright e2e

Infraestructura: Docker + CI/CD

📈 Próximas Mejoras
🧾 Boleta electrónica SUNAT

📱 Soporte completo en app móvil

🔁 Integración con inventarios multitienda

🧮 Control de deuda de clientes frecuentes


🛒 Sistema para Minimarket
Este módulo está orientado a pequeños y medianos negocios del rubro retail: minimarkets, bodegas organizadas, tiendas de abarrotes con caja. Permite gestionar productos, ventas, inventario, clientes, y realizar operaciones con o sin lector de código de barras.

Funcionalidades principales
Gestión de productos: Categorías, precios, unidades, stock mínimo, alertas y control por lote (opcional).

Ventas con y sin lector de código de barras: Compatible con lectores USB, permite búsqueda por nombre o escaneo rápido.

Punto de venta (POS): Interfaz ágil para vender productos, aplicar descuentos, imprimir tickets.

Inventario en tiempo real: Entrada/salida de stock, historial de movimientos.

Corte de caja diario: Registro de ingresos, egresos, resumen de caja por turno.

Clientes y fiados (créditos): Seguimiento de deudas por cliente, historial de pagos.

Modo offline (opcional): Versión con Electron para venta sin Internet.

Facturación electrónica: Integración con SUNAT para emisión automática (boleta/factura).

Alertas y reportes: Reportes diarios/semanales, exportables a Excel, alertas de stock bajo.

Tecnologías utilizadas
Frontend: React + Next.js App Router + Tailwind CSS

Backend: NestJS + Prisma

Base de datos: PostgreSQL

Desktop (opcional): Electron + React

Pagos: Soporte para Yape, Plin y QR simple

Estado actual
✅ Arquitectura definida
📦 Modelos base: Product, Sale, Client, InventoryMovement, CashRegister
🚧 Próximas tareas:

Agregar impresión de tickets

Integrar lector de códigos

Mejorar vista responsive para tablets