# matoanselmo — personal site

Personal portfolio site for Mateus Anselmo. Minimal, static, bilingual (EN/PT).

Built with [Astro](https://astro.build), deployed via Docker + Nginx.

## Project structure

```
/
├── public/
│   ├── favicon.ico
│   └── favicon.svg
├── src/
│   ├── assets/
│   ├── components/
│   │   └── hero.astro       # reusable hero card component
│   ├── layouts/
│   │   └── Layout.astro     # root layout with global styles + fonts
│   └── pages/
│       ├── index.astro      # English homepage (/)
│       └── pt.astro         # Portuguese homepage (/pt)
├── Dockerfile
├── docker-compose.yml
└── package.json
```

## Commands

| Command           | Action                                      |
| :---------------- | :------------------------------------------ |
| `npm install`     | Install dependencies                        |
| `npm run dev`     | Start dev server at `localhost:4321`        |
| `npm run build`   | Build production site to `./dist/`          |
| `npm run preview` | Preview the build locally before deploying  |

## Docker

Build and run with Docker Compose:

```sh
docker compose up --build
```

Serves the static build on port 80 via Nginx Alpine.
