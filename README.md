# world-news

Proyecto [Astro](https://astro.build) con **Vue 3**, **TypeScript** y **Tailwind CSS v4**.

## Stack

- **Astro 7** — sitio estático con islas hidratadas
- **Vue 3** — componentes interactivos (`<script setup lang="ts">`)
- **TypeScript** — estricto (`astro/tsconfigs/strict`)
- **Tailwind CSS v4** — vía plugin `@tailwindcss/vite`, estilos en `src/styles/global.css`

## Comandos

```bash
npm install      # instalar dependencias
npm run dev      # servidor de desarrollo
npm run build    # build de producción (salida en dist/)
npm run preview  # previsualizar el build
```

## Estructura

```
src/
├── components/
│   └── Counter.vue      # isla Vue de ejemplo (client:load)
├── layouts/
│   └── Layout.astro     # layout base, importa global.css
├── pages/
│   └── index.astro      # página principal
└── styles/
    └── global.css       # @import "tailwindcss"
```

## Notas

- Los componentes `.vue` se usan desde Astro con directivas de hidratación (`client:load`, `client:visible`, etc.).
- El resto del contenido se renderiza como HTML estático.
