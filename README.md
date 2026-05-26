# Apphive Docs

Documentación oficial de Apphive — **https://docs.apphive.io** — construida con
[MkDocs Material](https://squidfunk.github.io/mkdocs-material/).

> Migrado desde GitBook (mayo 2026). Todo es **Markdown puro** versionado en git.
> Sitio **bilingüe**: español en `/`, inglés en `/en/`.

---

## Índice

- [Estructura del repo](#estructura-del-repo)
- [Preview local](#preview-local)
- [Editar contenido](#editar-contenido)
- [Navegación (menú lateral)](#navegación-menú-lateral)
- [Sintaxis de Markdown](#sintaxis-de-markdown)
- [Imágenes y archivos](#imágenes-y-archivos)
- [Redirecciones de URLs viejas](#redirecciones-de-urls-viejas)
- [Deploy](#deploy)
- [Dominio y HTTPS](#dominio-y-https)
- [Problemas comunes](#problemas-comunes)

---

## Estructura del repo

```
docs/            -> contenido en ESPAÑOL  (se publica en la raíz: /)
docs-en/         -> contenido en INGLÉS   (se publica en: /en/)
  <cualquiera>/gitbook/assets/   -> imágenes y GIFs
mkdocs.yml       -> config del sitio ESPAÑOL (tema + nav + redirects)
mkdocs.en.yml    -> config del sitio INGLÉS
requirements.txt -> dependencias (mkdocs-material, mkdocs-redirects)
.github/workflows/deploy-docs.yml -> CI que construye y publica
```

Cada carpeta usa `README.md` como su página índice (igual que `index.md`).
Ej.: `docs/reference/controles/README.md` es la página de `/reference/controles/`.

---

## Preview local

Necesitas Python 3.

```bash
python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt

mkdocs serve -f mkdocs.yml       # español -> http://127.0.0.1:8000
mkdocs serve -f mkdocs.en.yml    # inglés
```

El navegador se recarga solo al guardar un archivo. Para ver el sitio combinado
tal cual se publica (español + `/en/`):

```bash
mkdocs build -f mkdocs.yml    --site-dir _site
mkdocs build -f mkdocs.en.yml --site-dir _site/en
python3 -m http.server -d _site 8000
```

---

## Editar contenido

**Modificar una página:** edita su archivo `.md`. Listo.

**Agregar una página nueva:**
1. Crea el `.md` dentro de `docs/` (o `docs-en/`), por ejemplo
   `docs/reference/controles/mi-control.md`.
2. Agrégalo al `nav:` en `mkdocs.yml` (ver siguiente sección) para que aparezca
   en el menú. Si no lo agregas al `nav`, MkDocs avisa con un warning.

**Borrar una página:** elimina el `.md` y quita su línea del `nav:`. Si tenía una
URL que pudiera estar enlazada por fuera, considera agregar un redirect (más abajo).

**Mover/renombrar:** mueve el archivo, actualiza su línea en el `nav:` y, si la URL
cambió, agrega un redirect de la URL vieja a la nueva.

---

## Navegación (menú lateral)

El orden y la jerarquía del menú se definen en `nav:` dentro de cada config.
Cada idioma tiene su propio `nav` (en `mkdocs.yml` y `mkdocs.en.yml`).

```yaml
nav:
  - Bienvenido a Apphive: README.md
  - REFERENCE:
      - Controles:
          - reference/controles/README.md      # página índice de la sección
          - Botón: reference/controles/button.md
          - Swiper: reference/controles/swiper.md
```

- `Título: ruta.md` = una entrada que apunta a un archivo.
- `Título:` seguido de una lista anidada = una sección con sub-entradas.
- La primera ruta suelta dentro de una sección (sin título) es su **página índice**.

> Las rutas son relativas a `docs/` (o `docs-en/`), no incluyen `docs/`.

---

## Sintaxis de Markdown

Es Markdown estándar + extensiones de Material. **Ya no es la sintaxis de GitBook.**

**Avisos / cajas de color** (en vez de `{% hint %}`):

```markdown
!!! info
    Texto del aviso (indentado 4 espacios).

!!! warning "Título personalizado"
    Cuidado con esto.
```

Tipos: `note`, `info`, `tip`, `success`, `question`, `warning`, `danger`, `example`.

**Pestañas** (en vez de `{% tabs %}`):

```markdown
=== "Pestaña A"
    Contenido de A (indentado 4 espacios).

=== "Pestaña B"
    Contenido de B.
```

> Convención heredada de GitBook: en las páginas de funciones/controles, las
> sub-secciones (Callbacks, Entry vars, Style, Data, Events) se escriben como
> estas pestañas dentro de la misma página.

**Código:**

````markdown
```js
const x = 1;
```
````

**Enlaces entre páginas:** Markdown normal con ruta relativa al archivo actual:
`[ver botón](button.md)` o `[a la sección](../controles/README.md)`.

---

## Imágenes y archivos

Guarda las imágenes en `docs/gitbook/assets/` (o `docs-en/gitbook/assets/`) y
refiérelas con ruta relativa:

```markdown
![Descripción](../../gitbook/assets/mi-imagen.png)
```

> La carpeta se llama `gitbook/` (sin punto) porque MkDocs ignora las carpetas
> que empiezan con `.`. Cualquier nombre/carpeta nueva funciona igual.

---

## Redirecciones de URLs viejas

Para que las URLs viejas de GitBook no se rompan, `mkdocs.yml` tiene el plugin
`redirects` con un mapa `URL_vieja.md: destino`. Para agregar una:

```yaml
plugins:
  - redirects:
      redirect_maps:
        'ruta/vieja.md': 'ruta/nueva.md'                 # destino interno
        'otra/vieja.md': 'https://docs.apphive.io/en/x/' # destino externo (full URL)
```

- La **clave** es la ruta vieja como si fuera un `.md` (genera un `index.html` que
  redirige). Ej.: la URL vieja `/foo/bar` -> clave `foo/bar.md`.
- El **valor** interno es la ruta del `.md` destino. Para apuntar al sitio inglés
  (`/en/...`) usa la URL completa `https://docs.apphive.io/en/...`.

---

## Deploy

**Automático.** Cada `push` a la rama `master` dispara
`.github/workflows/deploy-docs.yml`, que:

1. Instala dependencias.
2. Construye español a `_site` e inglés a `_site/en`.
3. Publica en GitHub Pages.

No hay que hacer nada manual: editas, `git push`, y en ~1–2 min está en
`https://docs.apphive.io`. Puedes ver el avance en la pestaña **Actions** del repo.

```bash
git add -A && git commit -m "docs: actualizar X" && git push
```

---

## Dominio y HTTPS

Ya configurado (no tocar salvo que cambie la infraestructura):

- DNS: `docs.apphive.io` es un `CNAME` a `apphiveio.github.io`.
- GitHub Pages: custom domain `docs.apphive.io` con **Enforce HTTPS** activo.
- El archivo `docs/CNAME` mantiene el dominio en cada deploy (no lo borres).

---

## Problemas comunes

| Síntoma | Causa / solución |
|---|---|
| Una página no sale en el menú | Falta agregarla al `nav:` del config de su idioma. |
| Warning "not in nav" al construir | Hay un `.md` que no está en `nav:`. Agrégalo o bórralo. |
| Imagen no carga | Revisa la ruta relativa y que el archivo esté en `gitbook/assets/`. |
| El selector de idioma no salta bien | Los links del selector son **relativos** a propósito (`mkdocs.yml`/`mkdocs.en.yml`, sección `extra.alternate`). No los pongas con `/` inicial. |
| Cambié algo y no se ve en producción | Revisa que el Action de **Actions** haya quedado en verde; el deploy tarda ~1–2 min + caché de CDN. |
| Quiero quitar el footer "Made with Material" | Ya está oculto con `extra.generator: false`. |
```
