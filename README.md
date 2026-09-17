# CLOTHON — Demo interactiva

Prototipo web navegable de la tienda en línea **Clothon** (moda multimarca: zapatos,
chemises, franelas, pantalones, suéteres y accesorios). Es un entregable de diseño:
HTML, CSS y JavaScript en un solo archivo, sin dependencias ni build.

## Cómo verlo

Abre `index.html` directamente en el navegador, o levanta un servidor local:

```bash
npx serve .
```

## Qué incluye

`index.html` es una SPA con enrutado por hash (`#/ruta`) que funciona por completo en el cliente:

- **Inicio**: carrusel editorial, buscador por talla, categorías, recién llegados, arma tu look, más vendidos, gift card y marcas.
- **Catálogo** (`#/c/<categoria>`): filtros por subcategoría, marca, talla, color y precio, más ordenamiento.
- **Producto** (`#/p/<clave>`): galería, swatches de color, tallas, acordeones y reseñas.
- **Marcas** (`#/marcas`, `#/m/<marca>`), **búsqueda en vivo** (`#/buscar`), **favoritos** (`#/favoritos`), **cuenta** (`#/cuenta`).
- **Arma tu look** (`#/look`), **gift card** (`#/gift-card`) y **ayuda / FAQ** (`#/ayuda`).
- **Checkout** (`#/checkout`) con validación y vista de pedido confirmado (`#/done/<n.º>`).
- Carrito lateral, favoritos y búsquedas recientes persistidos en `localStorage`.

`clothon-mockups-desktop.html` conserva la galería estática de las 12 pantallas a 1440 px.

## Estructura

```
index.html                    Demo interactiva (entregable principal)
clothon-mockups-desktop.html  Galería de mockups estáticos
assets/fonts/                 Raleway (Regular/Medium/SemiBold/Bold) + Enigma
```

## Notas

- Sistema visual monocromo, tipografía **Raleway** + logotipo **Enigma**.
- Las imágenes de producto son marcadores de posición (`[ foto ]` / `[ carrusel ]`); no hay fotos reales.
- Los datos de pago son de demostración: no se procesa ninguna transacción.
