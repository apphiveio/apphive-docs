# Apphive Docs

Documentación oficial de Apphive (https://docs.apphive.io), construida con
[MkDocs Material](https://squidfunk.github.io/mkdocs-material/).

> Migrado desde GitBook. Sitio **bilingüe**: español por defecto en la raíz,
> inglés bajo `/en/`. Selector de idioma nativo de Material en la barra superior.

## Estructura

- `docs/` — contenido en **español** (sitio por defecto, servido en `/`).
- `docs-en/` — contenido en **inglés** (servido en `/en/`).
- `*/gitbook/assets/` — imágenes y GIFs de cada idioma.
- `*/SUMMARY.md` — índice heredado de GitBook (excluido del build; útil de referencia).
- `mkdocs.yml` — config español (raíz) + redirecciones de URLs viejas de GitBook.
- `mkdocs.en.yml` — config inglés (`/en/`).

## Desarrollo local

```bash
python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt

# Español (raíz)
mkdocs serve -f mkdocs.yml            # http://127.0.0.1:8000

# Inglés
mkdocs serve -f mkdocs.en.yml
```

Para previsualizar el sitio combinado tal como se publica:

```bash
mkdocs build -f mkdocs.yml    --site-dir _site
mkdocs build -f mkdocs.en.yml --site-dir _site/en
python3 -m http.server -d _site 8000
```

## Sintaxis (ya no es GitBook)

- Avisos: admonitions de Material en vez de `{% hint %}`:
  ```markdown
  !!! info
      Texto del aviso.
  ```
  Tipos: `note`, `info`, `tip`, `success`, `warning`, `danger`.
- Pestañas: `=== "Título"` (en vez de `{% tabs %}`).
- Enlaces entre páginas: enlaces Markdown normales.

## Redirecciones de URLs viejas

`mkdocs.yml` incluye `plugins: redirects` con el mapeo de las URLs viejas de
GitBook → nuevas. Las del espacio español (`/apphive-documentacion/*`) están
mapeadas 1:1. Para agregar más, edita `redirect_maps` en `mkdocs.yml`.

## Deploy

Automático: cada push a `master` dispara `.github/workflows/deploy-docs.yml`,
que construye ambos idiomas y publica en GitHub Pages.

Primera vez:
1. **Settings → Pages → Source: GitHub Actions**.
2. DNS: `CNAME` de `docs.apphive.io` → `apphiveio.github.io`.
3. **Settings → Pages → Custom domain:** `docs.apphive.io` (+ Enforce HTTPS).
