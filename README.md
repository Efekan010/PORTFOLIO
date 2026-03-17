## SCSS (beginner friendly) – wat moet je doen?

Je opdracht zegt eigenlijk:
- Je gaat **SCSS/SASS** gebruiken om je website te stylen.
- Je laat zien dat je SCSS “handige features” gebruikt (zoals nesting, variabelen, `&`, imports, media queries, enz.).
- Bij het inleveren moet je in je portfolio-repo kunnen zien dat je SCSS hebt toegepast.

## Wat zit er in dit project?

Je SCSS staat in:
- `style.scss` (hoofdbestand)
- `scss/_variables.scss`
- `scss/_mixins.scss`
- `scss/_base.scss`
- `scss/_layout.scss`
- `scss/_components.scss`
- `scss/_utilities.scss`
- `scss/_responsive.scss`

## Welke opdrachtpunten vink je hiermee af?

- **Genestelde elementen (nesting)**: bijv. `nav { ul { ... } a { ... } }`
- **Minimaal 3 manieren `&`**:
  - `a { &:hover { ... } }` (pseudo-class)
  - `.buttons { &--compact { ... } }` (modifier)
  - `#menu-toggle { &:checked + .hamburger + .menu { ... } }` (state + selectors)
- **Namespace**: `$space` en `$breakpoints` als maps + `space()` / `bp()` functions
- **Minimaal 5 variabelen**: o.a. `$color-primary`, `$color-bg`, `$font-base`, `$radius-lg`, `$header-padding`
- **3 types variabelen**: colors, numbers, strings/maps
- **Operations**: bijv. `gap: space(md) + 10px;` en `padding: $i * 4px;`
- **@import**: `style.scss` importeert alle partials
- **@media (mobile & tablet)**: in `scss/_responsive.scss`
- **@extend**: `%card` placeholder wordt ge-extend in buttons/products
- **@if/@elseif/@else**: in `@mixin button-variant()`
- **@for/@each/@while**: in `scss/_utilities.scss`

Je gebruikt dus ruim meer dan de minimaal 3 onderdelen.

## Hoe zet je SCSS om naar CSS (makkelijkste manier)

Omdat dit een “plain HTML/CSS” portfolio is (geen Node/Vite), is dit het meest beginner-vriendelijk:

1. Installeer de VS Code extensie **Live Sass Compiler**.
2. Open `style.scss`.
3. Klik onderin op **Watch Sass**.
4. Dan wordt `style.css` automatisch bijgewerkt zodra je `style.scss` opslaat.

Je HTML gebruikt al:
- `<link rel="stylesheet" href="style.css">`

Dus je website blijft werken zodra `style.css` gecompileerd is.
