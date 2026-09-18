# liq.minecore.ec — form liquidación digital v1

Single-file form (`index.html`). No build step.

## Deploy (GitHub Pages)

1. Crear repo vacío sugerido: `estebanfch-cell/liq` (público o Pages desde private según org).
2. Copiar:
   - `index.html` → raíz del repo
   - `CNAME` → raíz (contenido: `liq.minecore.ec`)
3. Settings → Pages → Deploy from branch `main` / `/ (root)`.
4. DNS en minecore.ec: CNAME `liq` → `estebanfch-cell.github.io` (o el host Pages que use el org).
5. URLs cliente: `https://liq.minecore.ec/?t=TOKEN` (también acepta `?token=`).

API: misma URL de producción que `formularioclientes` (AdminAPI). Tras deploy de **AdminAPI_v108**, `liqGet` / `liqSubmit` quedan públicos.

## Prueba local

Abrir `index.html` no alcanza (CORS/file). Usar Pages o un static server + token real sembrado.
