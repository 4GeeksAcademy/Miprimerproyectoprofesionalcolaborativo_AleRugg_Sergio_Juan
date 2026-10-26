# Especificación técnica y funcional · Drôle de Monsieur

## 1. Resumen y Stack Tecnológico

Desarrollar un prototipo visual y navegable de la tienda online de **Drôle de Monsieur**, con cinco vistas: Inicio, Catálogo, Producto, Carrito y Checkout.

### Documentos de referencia

- [AGENTS.md](../AGENTS.md): restricciones técnicas y pautas de trabajo.
- [design.md](../design.md): identidad visual y sistema de diseño.
- [CONTEXT.md](../CONTEXT.md): estructura y contenido de las vistas.

### Restricciones técnicas

- Utilizar exclusivamente **HTML semántico y Tailwind CSS**.
- Preferir Tailwind compilado; si se usa CDN, servir CSS precompilado, sin ejecución de scripts en el navegador.
- No incorporar React, Vue, Angular, Bootstrap, bibliotecas de componentes, JavaScript de aplicación ni TypeScript.
- No añadir CSS personalizado, backend, APIs, autenticación ni procesamiento de pagos.
- Representar navegación mediante enlaces y selección mediante controles HTML nativos.
- Búsqueda, filtros, carrito y pago serán demostraciones estáticas, sin procesamiento, recálculo ni persistencia entre páginas.

## 2. Identidad Visual y Diseño

- **Estética:** Retro-Luxury, Smart Casual y Aesthetic Streetwear; combinar referencias deportivas retro con elegancia editorial y sastrería relajada.
- **Eslogan:** “Not from Paris Madame”.
- **Neutros:** blanco hueso `#F7F5F0`, beige `#D8C8B4`, crema `#EFE5D2` y negro `#000000`.
- **Tonos principales:** borgoña `#6F263D`, chocolate `#493329` y verdes oliva `#666B45` o bosque `#263F35`.
- **Acentos puntuales:** violeta retro `#79618D`, azul marino `#202B40` y mostaza tenue `#B49A59`.
- **Tipografía:** serif editorial para titulares y eslogan; sans-serif sobria para menús, precios y formularios. Referencias: Libre Baskerville y Archivo.
- **Composición:** grillas limpias, espacio en blanco, bordes finos, botones sobrios y ausencia de sombras recargadas.
- **Fotografía:** producto claramente visible, encuadres consistentes y proporción 3:4 en tarjetas.

Los valores son propuestas de diseño del proyecto, no especificaciones oficiales de la marca.

## 3. Especificaciones por Vista

### Elementos compartidos

- Usar `header`, `nav`, `main` y `footer`, con un único `h1` por página.
- Mantener navbar con logo, búsqueda y acceso a cuenta, respetando orden y destinos.
- Repetir footer con categorías, enlaces legales, información de la marca y contacto.
- Usar enlaces válidos; no presentar funciones no implementadas como operativas.

### Inicio

- Hero fotográfico de campaña con titular y enlace al catálogo.
- Dos listados horizontales: nuevos lanzamientos y más vendidos.
- Tarjetas con fotografía, nombre, precio y enlace a producto.

### Catálogo

- Controles nativos de categoría y talla antes del listado, identificados como demostrativos.
- Mostrar 20 productos de referencia mediante una grilla Tailwind de dos columnas en móvil y cuatro en escritorio.
- Mantener proporciones fotográficas y alineaciones consistentes.

### Producto

- Una columna en móvil y dos en escritorio: fotografía e información.
- Incluir nombre, referencia, talla, precio, cantidad y acceso a un carrito de ejemplo.
- Añadir descripción de materiales y usos recomendados.
- Identificar la acción de compra como demostrativa; no afirmar que modifica datos.

### Carrito

- Página completa con tres productos de ejemplo, no un panel lateral.
- Cada producto muestra miniatura, nombre, precio unitario, cantidad y total.
- Resumen con subtotal, impuestos y total estáticos y coherentes.
- Enlace “Comprar” hacia el checkout de demostración.

### Checkout

- Representar tres pasos mediante páginas enlazadas o secciones accesibles: datos personales, dirección de entrega y pago con tarjeta.
- Indicar el paso actual y permitir volver al anterior.
- Usar etiquetas visibles, tipos de campo adecuados y validación nativa donde proceda.
- Utilizar datos ficticios; no enviar, almacenar ni solicitar información bancaria real.
- Mostrar claramente que el pago es una demostración sin transacciones.

## 4. Criterios de Aceptación

- Las cinco vistas están presentes y enlazadas, sin destinos ficticios.
- La maquetación se adapta a móvil y escritorio sin solapamientos ni desbordamientos; solo los listados previstos permiten desplazamiento horizontal.
- Los estilos se implementan exclusivamente con utilidades de Tailwind.
- Navbar, footer, tarjetas y controles mantienen consistencia visual entre páginas.
- Imágenes sin distorsión, con textos alternativos adecuados y recursos disponibles.
- Formularios con etiquetas, navegación por teclado y foco visible; selección y errores no dependen solo del color.
- Contraste mínimo de 4,5:1 para texto normal y 3:1 para texto grande.
- Carrito con tres ejemplos e importes verificables; checkout con tres pasos y aviso de demostración.
- No existen scripts de aplicación, frameworks adicionales, envío de datos personales ni procesamiento de pagos.
- Se comprueban las vistas en móvil y escritorio, sus enlaces y sus estados accesibles.