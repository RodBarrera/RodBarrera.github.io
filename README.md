# Portafolio — Rodrigo Barrera

Sitio personal estático (HTML/CSS/JS, sin build). Diseño monocromo editorial.

```
index.html      → estructura y contenido
styles.css      → estilos (sistema blanco y negro)
script.js       → menú móvil, scroll-reveal, nav activo
assets/
  CV_Rodrigo_Barrera.pdf   → tu CV (ya enlazado en los botones "Descargar CV")
  foto.jpg                 → (opcional) tu foto, si quieres añadirla
```

---

## 1. Publicar en GitHub Pages

El sitio se sirve en **https://rodbarrera.github.io** usando un repo de usuario.

1. En GitHub, crea un repositorio **público** con el nombre EXACTO:
   `RodBarrera.github.io`
   (el nombre debe coincidir con tu usuario; las mayúsculas no afectan a la URL final, que será en minúsculas).
2. Sube TODO el contenido de esta carpeta a la **raíz** del repo
   (importante: `index.html` debe quedar en la raíz, no dentro de una subcarpeta).
   - Opción web: en el repo → "Add file" → "Upload files" → arrastra los archivos y la carpeta `assets/`.
   - Opción git:
     ```bash
     git init
     git add .
     git commit -m "Portafolio inicial"
     git branch -M main
     git remote add origin https://github.com/RodBarrera/RodBarrera.github.io.git
     git push -u origin main
     ```
3. En el repo → **Settings → Pages**. Para repos `usuario.github.io` Pages suele activarse solo desde `main` / raíz. Si no, selecciona Branch: `main`, Folder: `/ (root)` y guarda.
4. Espera 1–2 minutos y entra a **https://rodbarrera.github.io**.

> Yo no puedo crear el repo ni publicar por ti (requiere tu cuenta de GitHub). Tú haces esos pasos; los archivos ya están listos.

---

## 2. Qué falta / qué conviene revisar

- **Proyectos (sección 06):** ya integrados con tus repos reales fijados en GitHub
  (Catalejo, devsecops-shift, framework-ciberseguridad-iot-industrial, grc-dashboard).
  Si quieres cambiar cuáles aparecen, añadir demo o ajustar descripciones, dímelo.
  La tarjeta de `grc-dashboard` no tenía descripción en GitHub, así que redacté una
  basada en el nombre — revísala por si quieres precisarla.
- **Foto:** el diseño actual no usa foto (queda más limpio). Si la quieres, súbela como
  `assets/foto.jpg` y te agrego el bloque en el hero.
- **Verificación de certificados:** si tienes URLs de verificación (Credly, CertiProf, etc.),
  dímelas y añado un enlace "Verificar ↗" a cada certificación.

---

## 3. Editar contenido

Todo el texto está en `index.html`, en español y bien comentado por secciones
(`HERO`, `SOBRE MÍ`, `SKILLS`, `FORMACIÓN`, `CERTIFICACIONES`, `EXPERIENCIA`, `PROYECTOS`, `CONTACTO`).
Para cambiar colores o tipografías, edita las variables al inicio de `styles.css` (`:root`).
