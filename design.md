# Sistema de diseño · Drôle de Monsieur

## 1. Visión General e Identidad

**Frase icónica:** “Not from Paris Madame”.

La dirección visual combina **Retro-Luxury**, **Smart Casual** y **Aesthetic Streetwear**: confort deportivo retro, sastrería relajada y una presentación minimalista pero refinada.

La experiencia debe transmitir:
- **Elegancia relajada:** sofisticación sin rigidez.
- **Nostalgia contemporánea:** referencias vintage con una ejecución limpia.
- **Protagonismo del producto:** fotografía, materiales y siluetas por encima de la decoración.

> Esta guía es una propuesta inspirada en la marca, no un manual oficial. Los colores y las tipografías son recomendaciones de implementación.

## 2. Paleta de Colores

### Fondos y Neutros

| Color | HEX propuesto | Uso recomendado |
|---|---|---|
| Blanco hueso / Off-white | `#F7F5F0` | Fondo principal |
| Beige cálido | `#D8C8B4` | Bloques secundarios |
| Crema | `#EFE5D2` | Fondos editoriales y destacados |
| Negro puro | `#000000` | Texto principal y botones de compra |

### Tonos Primarios y Tierra

| Color | HEX propuesto | Uso recomendado |
|---|---|---|
| Borgoña / Burgundy | `#6F263D` | Acentos de marca y campañas |
| Marrón chocolate | `#493329` | Detalles gráficos y contenido editorial |
| Verde oliva | `#666B45` | Etiquetas y elementos secundarios |
| Verde bosque | `#263F35` | Campañas y contrastes puntuales |

### Acentos

| Color | HEX propuesto | Uso recomendado |
|---|---|---|
| Violeta retro | `#79618D` | Colecciones y destacados puntuales |
| Azul marino | `#202B40` | Alternativa cromática al negro |
| Dorado / Mostaza tenue | `#B49A59` | Pequeños detalles gráficos |

### Reglas de Aplicación

- Priorizar fondos neutros y texto oscuro.
- Utilizar un solo acento dominante por sección.
- Reservar los colores suaves para superficies, no para textos pequeños sobre fondos claros.
- Usar gris claro `#DEDAD3` para divisores y bordes.
- Comprobar un contraste mínimo de **4,5:1 en texto normal** y **3:1 en texto grande**.
- No comunicar errores, disponibilidad o selección únicamente mediante color.

## 3. Tipografía

| Función | Dirección | Referencias sugeridas |
|---|---|---|
| Encabezados y titulares | Serif clásica, elegante y editorial | Libre Baskerville o una serif editorial equivalente |
| Cuerpo, precios, menús y formularios | Sans-serif sobria y legible | Archivo o Helvetica Neue |
| Eslogan y acentos | Serif en versalitas o mayúsculas espaciadas | Misma familia editorial |

### Jerarquía Orientativa

| Elemento | Escritorio | Móvil |
|---|---|---|
| Titular principal | 48 px | 32 px |
| Título de sección | 32 px | 26 px |
| Nombre de producto | 18 px | 18 px |
| Texto y formularios | 16 px | 16 px |
| Metadatos y etiquetas | 14 px | 14 px |

### Reglas Tipográficas

- Limitar el sistema a dos familias tipográficas.
- Mantener un interlineado aproximado de `1.2` en titulares y `1.5` en textos.
- Reservar el interletreado amplio, entre `0.08em` y `0.12em`, para eslóganes y etiquetas breves.
- Evitar mayúsculas sostenidas en párrafos.
- Utilizar versalitas reales cuando la fuente las incluya.

## 4. Componentes Visuales y Estilo UI/Layout

### Estructura y Espaciado

- Grillas limpias con alineaciones consistentes.
- Espacio en blanco generoso, sin dificultar la exploración del catálogo.
- Escala de espaciado: **4, 8, 12, 16, 24, 32, 48 y 64 px**.
- Contenido centrado con un ancho máximo orientativo de **1440 px**.
- Márgenes laterales de **16 px en móvil** y **32–48 px en escritorio**.
- Bordes finos de **1 px**; evitar sombras decorativas.

### Fotografía

- Producto sobre fondos neutros con iluminación uniforme y colores fieles.
- Modelos con poses relajadas, naturales y elegantes.
- Encuadres inspirados en editoriales de moda vintage.
- Alternar imágenes completas con detalles de tejidos, acabados y estampados.
- Mantener una proporción **3:4** en imágenes del catálogo.
- Evitar filtros que oculten el color o la textura real de la prenda.

### Botones e Interacción

| Variante | Apariencia | Uso |
|---|---|---|
| Primario | Fondo negro y texto blanco | Agregar al carrito, comprar y continuar |
| Secundario | Fondo transparente y borde oscuro | Acciones alternativas |
| Enlace | Texto con subrayado al interactuar | Navegación y acciones auxiliares |

- Bordes rectos o radio máximo de **4 px**.
- Altura mínima recomendada de **44 px** en controles.
- Hover discreto mediante cambios de fondo, borde o subrayado.
- Transiciones breves de **150–200 ms**, respetando la preferencia de movimiento reducido.
- Foco de teclado visible y estados de selección, carga y deshabilitado claramente diferenciados.

### Componentes del Comercio Electrónico

| Componente | Criterio visual |
|---|---|
| Navbar | Logo, búsqueda y cuenta claramente accesibles; misma estructura en todas las vistas |
| Tarjeta de producto | Imagen protagonista, nombre y precio; sin marco ni sombra innecesarios |
| Filtros | Categoría y talla con selección visible y opción de limpiar |
| Selector de talla | Opciones compactas con estados disponible, seleccionado y agotado |
| Formularios | Etiquetas persistentes, bordes finos y errores junto al campo |
| Footer | Categorías, información legal y contacto organizados con jerarquía discreta |

## 5. Aplicación a las Vistas

- **Inicio:** hero fotográfico de campaña y listados horizontales de nuevos lanzamientos y más vendidos.
- **Catálogo:** filtros antes de la grilla; referencia de **4 columnas y 20 productos** en escritorio, adaptada a 2 columnas en móvil.
- **Producto:** fotografía e información en dos columnas; disposición vertical en móvil. Precio, talla, cantidad y compra deben ser fáciles de localizar.
- **Carrito:** página completa con miniaturas, precio unitario, cantidades, totales por producto y resumen de subtotal, impuestos y total. Incluir tres productos de ejemplo para mostrar el comportamiento visual.
- **Checkout:** tres pasos identificables: datos personales, dirección de entrega y pago con tarjeta. Mantener consistencia visual y conservar la información al retroceder.

La navbar y el footer se reutilizan en todas las vistas para mantener una experiencia coherente.