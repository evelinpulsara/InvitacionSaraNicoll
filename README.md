# 🎓 Invitación Digital · Mi Grado Sara Nicoll

Proyecto web estático listo para desplegar directamente en **Vercel**.

---

## 📁 Estructura del Proyecto

```text
invitacion-sarita/
├── index.html          # Página principal de la invitación (HTML + CSS + JS)
├── 404.html            # Página de error personalizada con el mismo diseño
├── vercel.json         # Configuración de Vercel (caché, cabeceras de seguridad y URLs)
├── .gitignore          # Archivos que no deben subirse a Git
├── imagenes/           # Fotos del carrusel (foto1.jpg, foto2.jpg, foto3.jpg, foto4.jpg)
└── musica/             # Carpeta para la canción de fondo (ej. cancion.mp3)
```

---

## 🚀 Cómo Desplegar en Vercel

Tienes **2 opciones muy sencillas**:

### Opción 1: Con GitHub (Recomendada)
1. Sube esta carpeta a un nuevo repositorio en [GitHub](https://github.com/).
2. Entra a [vercel.com](https://vercel.com/) e inicia sesión con tu cuenta de GitHub.
3. Haz clic en **"Add New..."** > **"Project"**.
4. Selecciona tu repositorio `invitacion-sarita`.
5. En **Framework Preset**, déjalo en **"Other"**.
6. Haz clic en **"Deploy"**. ¡En menos de un minuto tendrás tu enlace `https://tu-proyecto.vercel.app`!

### Opción 2: Con la terminal (Vercel CLI)
1. Instala Vercel si no lo tienes:
   ```bash
   npm i -g vercel
   ```
2. Desde la carpeta del proyecto, ejecuta:
   ```bash
   vercel
   ```
3. Sigue las instrucciones en pantalla (presiona Enter para los valores por defecto).
4. Para pasar a producción:
   ```bash
   vercel --prod
   ```

---

## ⚙️ Personalización Rápida en `index.html`

Cerca de la línea 610 de [index.html](file:///Users/evelin/Downloads/invitacion-sarita/index.html) encuentras el objeto `CONFIG`:

```javascript
const CONFIG = {
  nombre: "Sarita",
  promocion: "Promoción 2026",
  colegio: "Nombre del Colegio",
  fecha: "2026-12-05T18:00:00-05:00", // Formato ISO
  mama: "Nombre Mamá",
  papa: "Nombre Papá",
  cancion: {
    src: "musica/cancion.mp3",
    titulo: "La canción favorita de Sarita",
    artista: "Artista"
  },
  whatsapp: "573000000000", // Número de WhatsApp para confirmaciones (código de país + número)
  ...
};
```
