# Apphive Docs

Documentación oficial de Apphive (https://docs.apphive.io), construida con
[MkDocs Material](https://squidfunk.github.io/mkdocs-material/).

> Migrado desde GitBook. El contenido vive en Markdown puro dentro de `docs/`.

## Desarrollo local

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
mkdocs serve            # http://127.0.0.1:8000
```

## Estructura

- `docs/` — todo el contenido en Markdown (cada carpeta usa `README.md` como índice).
- `docs/gitbook/assets/` — imágenes y GIFs.
- `docs/SUMMARY.md` — índice heredado de GitBook (no se usa en el build, excluido).
- `mkdocs.yml` — config + navegación (`nav:`).

### Sintaxis (ya no es GitBook)

- Avisos: usa admonitions de Material en vez de `{% hint %}`:
  ```markdown
  !!! info
      Texto del aviso.
  ```
  Tipos: `note`, `info`, `tip`, `success`, `warning`, `danger`.
- Enlaces entre páginas: enlaces Markdown normales (`[texto](ruta.md)`).

## Deploy

Automático: cada push a `master` dispara `.github/workflows/deploy-docs.yml`,
que construye el sitio y lo publica en GitHub Pages.

Para que funcione la primera vez:
1. **Settings → Pages → Build and deployment → Source: GitHub Actions**.
2. DNS: `CNAME` de `docs.apphive.io` → `apphiveio.github.io`.
3. **Settings → Pages → Custom domain:** `docs.apphive.io` (+ Enforce HTTPS).
