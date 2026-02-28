# Tablero Educativo Integral — Sitio de presentación

Sitio estático de presentación del **Tablero de Gestión Integral**: propuesta de valor para instituciones educativas (gestión administrativa, académica y docente).

## Contenido

- **index.html** — Página principal (explorador interactivo del tablero). Es la página por defecto del sitio.

## GitHub Pages

El sitio está preparado para publicarse en **GitHub Pages** sin Jekyll.

1. **Publicar este repositorio**
   - Crea el repo en GitHub (vacío, sin README): [pablogventura/tablero-educativo-integral](https://github.com/pablogventura/tablero-educativo-integral).
   - Desde esta carpeta (`tablero-educativo-integral`):
     ```bash
     git add -A && git commit -m "Sitio estático listo para GitHub Pages"
     git push -u origin main
     ```

2. **Activar GitHub Pages**
   - En el repo: **Settings → Pages**.
   - **Source**: “Deploy from a branch”.
   - **Branch**: `main` (o `master`), carpeta **/ (root)**.
   - Guardar.

3. **URL del sitio**
   - `https://pablogventura.github.io/tablero-educativo-integral/`

El archivo `.nojekyll` evita que GitHub trate el sitio como Jekyll y sirve los HTML tal cual.

## Cómo actualizar desde el repo “colegios”

Desde la raíz del proyecto donde está `web/`:

```bash
cp web/index.html tablero-educativo-integral/index.html
cd tablero-educativo-integral && git add -A && git status
```

Luego commit y push al repo `tablero-educativo-integral`.
