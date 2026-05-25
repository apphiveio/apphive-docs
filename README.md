# Apphive Docs

Documentación oficial de Apphive (https://docs.apphive.io), construida con
[MkDocs Material](https://squidfunk.github.io/mkdocs-material/).

> Migrado desde GitBook. Sitio **bilingüe**: español por defecto en la raíz,
> inglés bajo `/en/`. Selector de idioma nativo de Material en la barra superior.

## Estructura

- `docs/` — contenido en **español** (sitio por defecto, servido en `/`).
- `docs-en/` — contenido en **inglés** (servido en `/en/`).
- `*/gitbook/assets/` — imágenes y GIFs de cada idioma.
- `mkdocs.yml` — config español (raíz) + redirecciones de URLs viejas de GitBook.
- `mkdocs.en.yml` — config inglés (`/en/`).

## Desarrollo local

```bash
python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
mkdocs serve -f mkdocs.yml            # español, http://127.0.0.1:8000
mkdocs serve -f mkdocs.en.yml         # inglés
```

## Sintaxis (ya no es GitBook)

- Avisos: admonitions de Material (`!!! info`) en vez de `{% hint %}`.
- Pestañas: `=== "Título"` en vez de `{% tabs %}`.
- Las páginas de funciones/controles muestran sus sub-secciones
  (Callbacks/Entry vars/Style/Data/Events) como pestañas dentro de la misma página.

## Deploy

Cada push a `master` dispara `.github/workflows/deploy-docs.yml`, que construye
ambos idiomas (es→`_site`, en→`_site/en`) y publica en GitHub Pages.

Primera vez:
1. **Settings → Pages → Source: GitHub Actions**.
2. DNS: `CNAME` de `docs.apphive.io` → `apphiveio.github.io`.
3. **Settings → Pages → Custom domain:** `docs.apphive.io` (+ Enforce HTTPS).
