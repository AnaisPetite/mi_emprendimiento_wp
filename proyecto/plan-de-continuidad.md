# Plan de continuidad · Etapa 2 de mi sitio

**Emprendimiento:** Nabi Skin
**Sitio de la etapa 1:** https://github.com/AnaisPetite/mi_emprendimiento_wp/blob/main/proyecto/desiciones.md
**Fecha:** 25/11/2026

## 1. Qué quedó fuera de la etapa 1 y por qué (3 pts)
Lista las funcionalidades que quisiste hacer y no pudiste. Para cada una, la razón.

| Funcionalidad | Por qué quedó fuera (tiempo, recursos, costo, conocimientos) | Qué aporta a mi emprendimiento |
|---|---|---|
| Tienda de comercio electrónico completa con WooCommerce | Tiempo y restricciones técnicas del servidor gratuito (bloqueo de pasarelas de pago seguras y correos). | Permite pasar del catálogo informativo actual a un carrito de compras real con transacciones en línea automatizadas. |
| Formulario de contacto funcional con envío de correos salientes | Restricciones del servidor gratuito de InfinityFree que bloquea los puertos de correo (`wp_mail`), lo que obligó a usar Flamingo solo como almacenamiento local. | Habilita notificaciones automáticas inmediatas a la bandeja de entrada del emprendedor sin depender de respaldos manuales. |
| Sistema de reservas y asesorías faciales en línea | Falta de recursos para implementar plugins de agenda avanzados y tiempo de desarrollo en la fase inicial. | Brinda un valor agregado directo para agendar diagnósticos de K-Beauty personalizados y fidelizar clientas. |


## 2. Recursos que necesito (2 pts)

| Funcionalidad | Plugin o herramienta | Gratis o de pago | Costo aproximado | Qué tendría que aprender |
|---|---|---|---|---|
| Catálogo y Carrito | WooCommerce | Gratis | $0 | Configuración de pasarelas de pago y gestión avanzada de stock. |
| Pagos en línea | WebPay / Mercado Pago | De pago (comisión por transacción) | Variable por venta | Integración de API de pagos nacionales en Chile. |
| Reservas | Amelia o Bookly | Freemium / Pago | ~$40 USD licencias | Administración de horarios de atención y sincronización de citas. |

**Servidor:** Hosting profesional de pago (como SiteGround o DonWeb) con al menos 10 GB de espacio SSD, PHP 8.1+, base de datos MySQL optimizada y certificado SSL obligatorio para procesar datos seguros de transacciones y tarjetas de crédito.

## 3. Priorización y cronograma (2 pts)
Ordena lo que harías primero y en cuánto tiempo. Puedes usar una tabla o un diagrama Gantt.

| Prioridad | Qué hago | Cuándo (mes o semana) | Resultado esperado |
|---|---|---|---|
| 1 | Optimización de imágenes y compresión a WebP | Mes 1, Semana 1-2 | Reducir el peso del sitio para compensar la velocidad de carga del servidor gratuito de InfinityFree. |
| 2 | Instalación y configuración de un plugin de caché gratuito (como LiteSpeed o WP Super Cache) | Mes 1, Semana 3-4 | Mejorar los tiempos de respuesta y la estabilidad general de la página web. |
| 3 | Mejora del SEO on-page y optimización de metadescripciones con Yoast SEO | Mes 2 | Aumentar la visibilidad orgánica de la tienda de cosmética coreana en buscadores. |

## 4. Riesgos y mitigación (1 pt)

| Riesgo | Qué haría | Cuándo se activa |
|---|---|---|
| Incompatibilidad o errores al configurar las pasarelas de pago nacionales. | Realizar pruebas en entorno de ensayo (Sandbox) y contar con soporte técnico del proveedor de pago. | Durante la integración de WooCommerce en el Mes 1. |
| Sobrecarga o caídas del sitio web durante fechas comerciales de alta demanda (CyberDay). | Contratar un plan de hosting con recursos escalables y activar sistemas de caché avanzados. | En eventos masivos o campañas de lanzamiento (Mes 2 en adelante). |
