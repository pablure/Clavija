# Clavija — afinador de guitarra

Afinador web para el móvil. Escucha por el micrófono, detecta la nota con el algoritmo YIN y te dice si tienes que apretar o aflojar la clavija.

## Funciones
- Modo **Guitarra**: detecta sola qué cuerda estás tocando. Toca una cuerda en la fila de abajo para fijarla (útil si está muy desafinada).
- Modo **Cromático**: cualquier nota.
- Afinaciones: Estándar, Drop D, medio tono abajo, un tono abajo, DADGAD, Open G.
- Referencia La4 ajustable (430–450 Hz).
- Botón **▶ Tono** para escuchar la nota de la cuerda.
- Vibra al quedar afinada (Android), mantiene la pantalla encendida y funciona sin conexión tras la primera visita.

## Publicarla en GitHub Pages
1. Crea un repositorio nuevo en GitHub (por ejemplo `clavija`).
2. Sube estos archivos a la raíz: `index.html`, `manifest.json`, `icon.svg`, `sw.js`, `README.md`.
3. En el repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, rama `main`, carpeta `/ (root)` → **Save**.
4. En un minuto estará en `https://TU-USUARIO.github.io/clavija/`.
5. Ábrela en el móvil, pulsa **Activar micrófono** y acepta el permiso.
6. Para tenerla como app: en Safari **Compartir → Añadir a pantalla de inicio**; en Chrome **⋮ → Instalar aplicación**.

El micrófono solo funciona con `https`, por eso GitHub Pages es ideal (abrir el archivo directamente desde el móvil no funcionará).

## Probar en el ordenador
```bash
python3 -m http.server 8000
```
y abre `http://localhost:8000` (localhost sí permite el micrófono).
