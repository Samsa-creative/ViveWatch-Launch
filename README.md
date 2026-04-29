# Propuesta Lanzamiento ViveWatch — Samsa Creative × ViveLibre

Deck HTML single-page, propuesta de lanzamiento del ViveWatch (campaña 2026—2027).

## Ver el deck

**Producción:** https://samsa-creative.github.io/ViveWatch-Launch/

**Local:**
```bash
cd "Documents/Samsa/2. Comercial/2. Pipeline/ViveLibre/deck"
python3 -m http.server 8080
# abrir http://localhost:8080
```

Abrir `index.html` directo en el navegador también funciona, pero algunos enlaces externos pueden estar más restringidos en `file://`.

## Navegación

- `← →` o `Space` — slide anterior / siguiente
- `Home` / `End` — primera / última slide
- `F` — fullscreen
- Touch swipe en mobile
- Click en mitad izquierda / derecha

## Estructura (22 slides)

1. Cover propuesta
2. Carátula servicios Samsa Creative
3. Carátula clientes
4. Índice
5—7. Brief (divisor + reto + lo que entendimos)
8—10. Concepto (divisor + big idea + tono)
11—12. Referencia de campaña
13—16. Referencias por hito (Lanzamiento, Navidad, Padre, Madre)
17—19. Plan (divisor + 3 fases + rodajes)
20—21. Presupuesto (divisor + total y calendario)
22. Cierre

## Stack

Single-page HTML + CSS embebido + vanilla JS. Sin build, sin dependencias. Google Fonts (Montserrat) vía CDN.

## Editar contenido

Todo el contenido está en `index.html` dentro de las secciones `<section class="slide">`. Cada slide está numerada y comentada arriba de su bloque. Los tokens de color y tipografía están en el bloque `:root` al inicio del `<style>`.

## Pendientes para el deck final

- [ ] Reemplazar grilla de clientes (slide 3) con logos finales
- [ ] Definir y reemplazar el total absoluto del presupuesto (slide 21)
- [ ] Cargar embeds reales de YouTube cuando el cliente apruebe las referencias (slides 11—16)
- [ ] Render 3D del ViveWatch post-NDA (a definir dónde insertarlo)

## Como template

Esta estructura queda como base reutilizable para próximas propuestas estratégicas de Samsa Creative.

Para una propuesta nueva:
1. Duplicar la carpeta `deck/`
2. Reemplazar logo cliente, concepto, moodboards, plan y presupuesto
3. Mantener carátulas Servicios + Clientes (constantes), índice, theme Samsa, componentes y mecánica de navegación
4. Crear nuevo repo en `samsa-creative` y deploy a GitHub Pages
