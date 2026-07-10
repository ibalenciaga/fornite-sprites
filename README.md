# Fortnite Sprites - Astro Estatico

App para llevar el control de los Sprites (espiritus) de Fortnite con Astro, sin backend.

## Que hace

- Muestra una card por Sprite con su nombre e imagen.
- Agrupa los Sprites por tipo (Base, Gold, Gummy, Galaxy, Holofoil).
- Permite marcar/desmarcar cada Sprite pulsando en su card.
- Oscurece la card cuando esta marcado como conseguido.
- Guarda el progreso en localStorage del navegador.
- Permite resetear la coleccion local con un boton.

## Requisitos

- Node.js 18 o superior.

## Desarrollo local

1. Instala dependencias:

    npm install

2. Arranca Astro en desarrollo:

    npm run dev

3. Abre en el navegador:

    [http://localhost:4321](http://localhost:4321)

## Build para subir a hosting estatico

1. Genera la build:

    npm run build

2. Los archivos finales quedan en:

    dist/

3. Sube dist/ a Netlify, Vercel, Cloudflare Pages o GitHub Pages.

## Datos y persistencia

- Catalogo de Sprites: data/sprites.json
- Imagenes: public/images/sprites/
- Progreso de coleccion: localStorage (clave fortnite-sprites-collected-v1)

## Nota importante

Al no tener backend, el progreso no se sincroniza entre dispositivos de forma automatica.
