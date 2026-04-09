# Prueba Lectiva

Base SvelteKit con arquitectura `feature-first/domain-first` para integrar la API de Rick and Morty.

## Run

```bash
npm install
npm run dev
```

## Check

```bash
npm run check
npm run build
```

## Deploy

El proyecto queda listo para desplegarse con GitHub Actions en GitHub Pages.

1. En GitHub abre `Settings > Pages`.
2. En `Build and deployment`, selecciona `Source: GitHub Actions`.
3. Haz push a `main` para disparar el workflow `Deploy to GitHub Pages`.

La ruta base se calcula automaticamente en el workflow:

- si el repositorio es `usuario.github.io`, publica en `/`
- si es un repositorio de proyecto, publica en `/<nombre-del-repositorio>`

## Estructura

- `src/lib/core`: cliente HTTP, configuracion y adaptadores.
- `src/lib/entities`: tipos y mapeos de dominio.
- `src/lib/features`: features por caso de uso.
- `src/routes`: composicion de rutas y carga de datos.
