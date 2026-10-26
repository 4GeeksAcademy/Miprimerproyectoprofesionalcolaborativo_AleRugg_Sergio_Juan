# Tareas del prototipo · Drôle de Monsieur

Seguir las cuatro fases acordadas, los requisitos de [CONTEXT.md](CONTEXT.md) y [specs/spec.md](specs/spec.md), las restricciones de [AGENTS.md](AGENTS.md) y la identidad visual de [design.md](design.md).

- [ ] **Configuración Inicial y Base**
  - [ ] Crear los archivos `index.html`, `catalog.html`, `product.html`, `cart.html` y `checkout.html`.
  - [ ] Incorporar estructura semántica, idioma, metadatos responsive y un título principal por página.
  - [ ] Configurar Tailwind CSS preferentemente compilado, sin scripts en el navegador.
  - [ ] Configurar colores y tipografías conforme a la guía visual.
  - [ ] Preparar fotografías, logotipo y recursos tipográficos; comprobar disponibilidad y permisos de uso.
  - [ ] Maquetar la navbar con logo, búsqueda y acceso a cuenta.
  - [ ] Maquetar el footer con categorías, información legal y contacto.
  - [ ] Repetir navbar y footer en todas las páginas, manteniendo estructura, estilos y destinos.
  - [ ] Establecer navegación mediante enlaces válidos, sin frameworks ni lógica de aplicación.

- [ ] **Desarrollo de Vistas Principales**
  - [ ] **Home (`index.html`)**
    - [ ] Maquetar el hero fotográfico de campaña con enlace al catálogo.
    - [ ] Crear el listado horizontal de nuevos lanzamientos.
    - [ ] Crear el listado horizontal de más vendidos.
    - [ ] Mantener tarjetas consistentes con fotografía, nombre, precio y enlace a producto.
  - [ ] **Catálogo (`catalog.html`)**
    - [ ] Colocar filtros nativos de categoría y talla antes del listado.
    - [ ] Identificar los filtros como demostrativos, sin procesamiento real.
    - [ ] Maquetar 20 productos en cuatro columnas y cinco filas en escritorio.
    - [ ] Adaptar la grilla a dos columnas en móvil.
  - [ ] **Vista de Producto (`product.html`)**
    - [ ] Distribuir fotografía e información en dos columnas en escritorio y una en móvil.
    - [ ] Incluir nombre, referencia, talla, precio y selector de cantidad.
    - [ ] Representar “Agregar al carrito” mediante un enlace al carrito de ejemplo, sin prometer cambios persistentes.
    - [ ] Añadir descripción inferior con materiales y usos recomendados.

- [ ] **Desarrollo del Flujo de Compra**
  - [ ] **Carrito (`cart.html`)**
    - [x] Maquetar una página completa, no un panel lateral.
    - [x] Mostrar tres productos de ejemplo con miniatura, nombre, precio unitario, cantidad y total por producto.
    - [x] Incorporar subtotal, impuestos y total general.
    - [x] Comprobar la coherencia aritmética de todos los importes estáticos.
    - [x] Añadir el enlace “Comprar” hacia el checkout de demostración.
  - [ ] **Checkout (`checkout.html`)**
    - [ ] Crear el paso 1: datos personales.
    - [ ] Crear el paso 2: dirección de entrega.
    - [ ] Crear el paso 3: representación del pago con tarjeta.
    - [ ] Organizar los pasos como secciones accesibles con enlaces internos para avanzar y retroceder.
    - [ ] Identificar cada paso mediante encabezados numerados y etiquetas visibles.
    - [ ] Utilizar datos ficticios y representar la tarjeta con información de ejemplo no editable.
    - [ ] Indicar que no se realiza una compra real; evitar envío, almacenamiento o solicitud de datos bancarios reales.

- [ ] **Control de Calidad y Refinamiento**
  - [ ] Verificar el uso exclusivo de HTML y Tailwind CSS, sin CSS personalizado, frameworks ni JavaScript de aplicación.
  - [ ] Confirmar ausencia de backend, APIs, autenticación y pasarelas de pago.
  - [ ] Comprobar fidelidad de colores, tipografías, fotografías, espaciado y componentes con la guía visual.
  - [ ] Revisar todas las vistas en móvil, tablet y escritorio, evitando solapamientos y desbordamientos.
  - [ ] Comprobar enlaces, imágenes y consistencia de navbar, footer y tarjetas.
  - [ ] Verificar textos alternativos, etiquetas, orden de encabezados, navegación por teclado y foco visible.
  - [ ] Comprobar contraste y estados de selección, error y deshabilitado sin depender solo del color.
  - [ ] Confirmar que búsqueda, filtros, carrito y pago se presentan como demostraciones estáticas.
  - [ ] Revisar los criterios de aceptación de la especificación y documentar las limitaciones pendientes.