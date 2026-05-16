# Presupuesto Eléctrico — Instrucciones de deploy

## Archivos del proyecto

```
presupuesto-electricista.html   → renombrar a index.html al subir
manifest.json
sw.js
README.md
```

---

## Opción A — GitHub Pages (gratis, recomendado)

1. Creá una cuenta en https://github.com si no tenés
2. Nuevo repositorio: "presupuesto-electricista" (público)
3. Subí los 3 archivos (index.html, manifest.json, sw.js)
   - Renombrá presupuesto-electricista.html → index.html
4. Settings → Pages → Branch: main → Save
5. En ~2 minutos queda en:
   https://TU_USUARIO.github.io/presupuesto-electricista

---

## Opción B — Vercel (aún más fácil)

1. Entrá a https://vercel.com → "Add New Project"
2. Arrastrá la carpeta con los 3 archivos
3. Deploy → URL instantánea tipo:
   https://presupuesto-electricista.vercel.app

---

## Instalar como app en el celular (Android)

1. Abrí la URL en Chrome
2. Menú (⋮) → "Agregar a pantalla de inicio"
3. Listo — aparece como ícono de app, sin barra del navegador

## Instalar en iPhone (Safari)

1. Abrí la URL en Safari
2. Compartir (□↑) → "Agregar a inicio"

---

## Para que funcione offline

El service worker (sw.js) cachea la app automáticamente en la primera visita.
Después funciona sin internet.

---

## Personalización rápida (VS Code)

En index.html buscás y cambiás:
- Los datos por defecto de forma de pago → línea ~130
- El IVA del 21% si no aplica → línea ~200
- El logo/nombre en el PDF → función generatePDF()

