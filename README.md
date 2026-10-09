# NEXORA — Premium Storefront (Demo)

Sitio independiente desarrollado para presentar al cliente de Nexora. Identidad visual negro / blanco / verde neón (verde solo como acento sobre la X y microinteracciones). Arquitectura SPA estática con enrutado hash compatible con Vercel.

## Funcionalidades

- Home editorial premium, cuatro catálogos y filtros especializados (audiencia, marca y precio).
- Buscador global, detalle de producto, carrito persistente en el navegador y cantidades editables.
- Checkout de demostración con dirección de envío y elección de Bs, USDT o Zinli.
- Opción para generar resumen de pedido y compartirlo por WhatsApp (habilitar número comercial en `app.js`: `WHATSAPP_NUMBER`).
- Cuenta **demostrativa local** sin autenticación real, solo nombre/correo: **no almacena contraseñas**.
- Diseño adaptable a pantallas móviles y de escritorio. Accesibilidad básica y sin dependencias de compilación.

## Publicación

1. Crear repositorio vacío **independiente** en GitHub, por ejemplo `OliverLuggo/nexora-premium`.
2. Subir archivos de esta carpeta a la raíz del repositorio.
3. Vercel > Add New > Project > Import Git Repository > seleccionar `nexora-premium`.
4. Framework: `Other`. Build command: vacío. Output Directory: vacío. Deploy.

## Importante — No es e-commerce conectado

- Los productos, precios, fotografías y disponibilidades son **referenciales**, no son inventario real.
- No hay servidor de cuentas, sesiones verificadas, pasarela de pagos ni integración de empresa de envíos.
- "Realizar pedido de prueba" crea solo una confirmación local no facturable y no cobra dinero.
- La interfaz de pago muestra el método seleccionado, pero **no acepta transferencias reales**.
- Antes de lanzamiento se requiere backend seguro (p.ej. Supabase proyecto nuevo del negocio), autenticación real, inventario, administración, pagos con confirmación y validación legal/comercial.
- No pedir datos de tarjetas ni contraseñas en el prototipo.

## Configuración

`app.js` → `WHATSAPP_NUMBER` colocar el número venezolano con código país, solo dígitos, cuando el cliente lo facilite.

Autor: demo para Nexora, octubre 2026.
