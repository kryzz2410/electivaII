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

## CI/CD

El proyecto despliega automaticamente a GitHub Pages con GitHub Actions en cada push a `main`.

- Workflow: `.github/workflows/deploy.yml`
- Base path: se configura con `BASE_PATH` para publicar correctamente en repositorios tipo `usuario/repositorio`
- Salida estatica: `build/`

## Estructura

- `src/lib/core`: cliente HTTP, configuracion y adaptadores.
- `src/lib/entities`: tipos y mapeos de dominio.
- `src/lib/features`: features por caso de uso.
- `src/routes`: composicion de rutas y carga de datos.
