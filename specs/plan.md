# Plan de ejecución · Drôle de Monsieur

## Alcance y Referencias

Construir un prototipo visual y navegable utilizando exclusivamente **HTML semántico y Tailwind CSS**, conforme a los siguientes documentos:

- [AGENTS.md](AGENTS.md): restricciones técnicas y pautas de trabajo.
- [design.md](design.md): identidad visual, colores, tipografías y componentes.
- [CONTEXT.md](CONTEXT.md): contenido de las cinco vistas.
- [specs/spec.md](specs/spec.md): especificaciones y criterios de aceptación.

No incorporar frameworks, JavaScript de aplicación, CSS personalizado, backend ni procesamiento real de datos o pagos. Trabajar una vista o componente por vez, conservando los cambios existentes del equipo.

## Fase 1: Estructura Base y Assets

1. Crear las cinco páginas: `index.html`, `catalog.html`, `product.html`, `cart.html` y `checkout.html`.
2. Preparar los recursos de fotografías, logotipo y tipografías, comprobando su disponibilidad y permisos de uso.
3. Configurar Tailwind CSS preferentemente compilado; no utilizar scripts de ejecución en el navegador.
4. Configurar las familias tipográficas y los colores definidos en la guía visual mediante las herramientas de Tailwind.
5. Establecer la estructura semántica de cada página: cabecera, navegación, contenido principal y pie.
6. Maquetar la navbar con logo, búsqueda y acceso a cuenta. Representar las funciones no implementadas como demostrativas.
7. Maquetar el footer con categorías, información legal, marca y contacto.
8. Repetir navbar y footer en las cinco páginas, manteniendo estilos, orden y destinos coherentes.

**Resultado esperado:** cinco páginas base enlazadas, con recursos disponibles y componentes compartidos consistentes.

## Fase 2: Vistas Principales de Navegación

### Página de Inicio: `index.html`

1. Construir un hero fotográfico de campaña con identidad de marca y enlace al catálogo.
2. Añadir los listados horizontales de nuevos lanzamientos y más vendidos.
3. Mantener tarjetas consistentes con imagen, nombre, precio y enlace a la ficha.

### Catálogo: `catalog.html`

1. Situar controles nativos de categoría y talla antes del listado, sin prometer filtrado real.
2. Maquetar 20 productos en cuatro columnas y cinco filas en escritorio.
3. Adaptar la grilla a dos columnas en móvil y mantener proporciones fotográficas uniformes.

### Vista de Producto: `product.html`

1. Distribuir fotografía e información en dos columnas en escritorio y una columna en móvil.
2. Incluir nombre, referencia, talla, precio y selector nativo de cantidad.
3. Representar “Agregar al carrito” como acceso al carrito de ejemplo, sin modificación ni persistencia de datos.
4. Añadir debajo la descripción, los materiales y los usos recomendados.

**Resultado esperado:** navegación completa entre Inicio, Catálogo y Producto, con contenido visual consistente.

## Fase 3: Flujo de Conversión (Carrito y Pago)

### Carrito: `cart.html`

1. Construir una página completa, no un panel lateral.
2. Mostrar tres productos de ejemplo mediante una tabla semántica adaptada a móvil.
3. Incluir miniatura, nombre, precio unitario, cantidad y total por producto.
4. Definir subtotal, impuestos y total estáticos, comprobando su coherencia aritmética.
5. Añadir el enlace “Comprar” hacia el checkout e identificar el carrito como demostrativo.

### Checkout: `checkout.html`

1. Organizar tres secciones accesibles: datos personales, dirección de entrega y pago con tarjeta.
2. Utilizar enlaces internos para avanzar y retroceder, sin scripts ni ocultación dinámica de pasos.
3. Identificar cada paso con encabezados numerados y etiquetas visibles en sus campos.
4. Utilizar únicamente datos ficticios y validación HTML nativa donde proceda.
5. Representar el pago mediante datos de ejemplo no editables, sin solicitar información bancaria real.
6. Evitar cualquier envío o almacenamiento de datos y señalar que no se realiza una compra real.

**Resultado esperado:** recorrido demostrativo desde Producto hasta Checkout, sin transacciones ni procesamiento real.

## Fase 4: Refinamiento Visual y Responsividad

1. Contrastar colores, tipografías, espaciado, bordes y botones con la guía visual.
2. Revisar cada página en móvil, tablet y escritorio, evitando solapamientos y desbordamientos.
3. Comprobar imágenes, encuadres, enlaces y consistencia de navbar, footer y tarjetas.
4. Verificar encabezados, textos alternativos, etiquetas, navegación por teclado y foco visible.
5. Comprobar contraste y estados de selección, error y deshabilitado sin depender únicamente del color.
6. Confirmar que solo se utilizan HTML y Tailwind CSS, y que las interacciones estáticas están identificadas.
7. Revisar los criterios de aceptación de la especificación y registrar las limitaciones del prototipo.

**Resultado esperado:** prototipo visual coherente con la marca, adaptable y accesible, con alcance demostrativo explícito.