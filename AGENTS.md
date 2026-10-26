# Guía del copiloto

## Restricción técnica obligatoria

- Desde el inicio de cualquier tarea, utilizar exclusivamente HTML semántico y Tailwind CSS para construir el prototipo.
- No incorporar React, Vue, Angular, Next.js, Bootstrap, bibliotecas de componentes ni otros frameworks.
- No añadir JavaScript de aplicación, TypeScript, manejadores de eventos inline ni scripts para simular funcionalidades.
- Aplicar los estilos con utilidades de Tailwind; no introducir otro sistema de estilos ni hojas de CSS personalizado.
- Preferir Tailwind servido como CSS compilado. Las herramientas de compilación de Tailwind no autorizan otras dependencias de interfaz ni lógica de aplicación.
- No crear un backend, integrar APIs, autenticación o pasarelas de pago. No ampliar el alcance sin autorización explícita.

## Documentación obligatoria

Antes de maquetar o modificar una vista, consultar los apartados relevantes de ambos documentos:

- [CONTEXT.md](CONTEXT.md): fuente de referencia para el contexto del equipo, el cliente, las cinco vistas y sus contenidos.
- [design.md](design.md): fuente de referencia para la identidad de Drôle de Monsieur, colores, tipografía, fotografía, espaciado y estados visuales.

Respetar las mayúsculas de los nombres: el documento existente es `CONTEXT.md`, no `context.md`.
No modificar estos documentos sin autorización ni duplicar sus especificaciones completas en otros archivos.
Si un requisito no puede resolverse con HTML y Tailwind CSS, explicar la limitación y proponer una representación estática; no añadir tecnologías prohibidas.

## Alcance del prototipo

- Construir páginas HTML enlazadas para representar la navegación entre las vistas.
- Utilizar controles nativos de HTML para selección, entrada de datos y validación básica.
- Representar filtros, búsqueda, cuenta y cambios del carrito mediante estados de ejemplo, sin afirmar que existe procesamiento real.
- Mostrar cantidades y totales estáticos coherentes; no prometer recálculo ni persistencia de datos entre páginas.
- Representar los pasos del checkout con páginas enlazadas o secciones HTML accesibles, sin scripts.
- No solicitar datos bancarios reales ni enviar, almacenar o registrar datos personales o de tarjeta. Identificar el pago como demostración.

## Pautas de maquetación por componente

| Componente o vista | Pauta obligatoria |
|---|---|
| Navbar | Mantener logo, búsqueda y acceso a cuenta con el mismo orden, estilo y destinos en todas las páginas. |
| Footer | Conservar categorías, enlaces legales y contacto en todas las vistas. |
| Inicio | Incluir un hero de campaña con fotografía y las secciones horizontales de nuevos lanzamientos y más vendidos. |
| Tarjeta de producto | Mantener proporción fotográfica, alineaciones, nombre, precio y enlace a la ficha consistentes. |
| Catálogo | Situar los filtros de categoría y talla antes de la grilla; mostrar la referencia de 20 productos y 4 columnas en escritorio. |
| Ficha de producto | Distribuir imagen e información en dos columnas en escritorio; incluir nombre, referencia, talla, precio, cantidad, acción de compra y descripción de materiales y usos. |
| Carrito | Usar una página completa, no un panel lateral; incluir tres productos de ejemplo y todos los importes definidos en el contexto. |
| Checkout | Mantener el orden de datos personales, dirección de entrega y pago con tarjeta; indicar el paso actual y permitir volver al anterior. |
| Botones y formularios | Seguir las variantes de diseño; diferenciar foco, selección, error y deshabilitado sin depender solo del color. |

## Identidad visual y adaptación

- Aplicar la dirección Retro-Luxury, Smart Casual y Aesthetic Streetwear descrita en el diseño.
- Respetar las familias tipográficas, la jerarquía, los colores y el uso del eslogan “Not from Paris Madame” definidos en la guía visual.
- Usar fotografías de producto y editoriales relevantes, sin distorsión y con encuadres consistentes.
- Mantener grillas limpias, espacio en blanco, bordes finos y botones sobrios; evitar sombras recargadas y decoración ajena a la marca.
- Diseñar primero para móvil con las variantes responsive de Tailwind: catálogo de dos columnas en móvil y cuatro en escritorio; ficha de producto en una columna en móvil.
- Evitar desbordamientos y solapamientos. Limitar el desplazamiento horizontal a los listados que lo requieran.

## Accesibilidad y navegación

- Usar regiones semánticas, un título principal por página y encabezados ordenados.
- Proporcionar texto alternativo adecuado en imágenes y etiquetas visibles asociadas a los campos.
- Usar enlaces para navegar y botones para acciones; no dejar destinos ficticios ni presentar acciones inexistentes como reales.
- Garantizar navegación por teclado, foco visible, controles de tamaño suficiente y contraste según la guía visual.
- Respetar la preferencia de movimiento reducido si se añaden transiciones.

## Forma de trabajo y verificación

- Explicar brevemente el cambio antes de editar y trabajar en una vista o componente por vez.
- Conservar los cambios del equipo; evitar refactorizaciones, dependencias y archivos innecesarios.
- Mantener navbar, footer y componentes repetidos coherentes entre los archivos HTML, sin introducir un framework para reutilizarlos.
- Comprobar la vista modificada en móvil y escritorio, sus enlaces, imágenes y estados accesibles.
- Verificar que no se añadieron tecnologías prohibidas y que los datos de ejemplo son coherentes.
- No crear pruebas automatizadas sin solicitud explícita ni ejecutar suites completas para cambios de maquetación.
- Informar qué se verificó y qué interacciones son únicamente demostrativas.