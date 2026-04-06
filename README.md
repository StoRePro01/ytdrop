# YTDrop 🎬

Descargador de YouTube gratis usando la API de [cobalt.tools](https://cobalt.tools).

## ✨ Funciones

- Descarga video + audio (MP4, WebM, MKV)
- Descarga solo audio (MP3, OGG, Opus, WAV)
- Elige calidad: 144p hasta máxima
- Elige bitrate de audio: 64–320 kbps
- Sin backend, sin servidor, sin registro

---

## 🚀 Deploy en Vercel (5 minutos)

### Paso 1 — Sube a GitHub

1. Crea un repositorio nuevo en [github.com](https://github.com/new)
2. Sube los archivos:
   - `index.html`
   - `vercel.json`

```bash
git init
git add .
git commit -m "YTDrop inicial"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/TU_REPO.git
git push -u origin main
```

### Paso 2 — Conecta con Vercel

1. Ve a [vercel.com](https://vercel.com) e inicia sesión con tu cuenta de GitHub
2. Click en **"Add New Project"**
3. Selecciona tu repositorio
4. En la configuración:
   - **Framework Preset**: `Other`
   - **Root Directory**: `/` (raíz)
   - No necesitas variables de entorno
5. Click **Deploy**

En 30 segundos tendrás una URL como `https://tu-proyecto.vercel.app` ✅

---

## ⚠️ Nota sobre CORS

La API de cobalt.tools (`api.cobalt.tools`) puede bloquear peticiones directas desde el navegador por CORS. Si pasa esto:

### Solución A — Hostea tu propia instancia de cobalt

Cobalt es open source. Puedes correr tu propia instancia gratis en Railway:
- Sigue las instrucciones en: https://github.com/imputnet/cobalt/blob/main/docs/run-an-instance.md
- Luego cambia en `index.html`: `const COBALT_API = 'https://TU-INSTANCIA.railway.app';`

### Solución B — Cambia la instancia pública

Algunos owners de instancias cobalt permiten acceso público. Puedes ver instancias disponibles en:
- https://instances.cobalt.best

Cambia `COBALT_API` en el `index.html` por la URL de una instancia que acepte peticiones externas.

---

## 📁 Estructura

```
/
├── index.html     ← Toda la app (frontend puro)
├── vercel.json    ← Configuración de deploy
└── README.md
```

## ⚖️ Legal

Úsalo solo para descargar contenido:
- De tu autoría
- Con licencia Creative Commons
- De dominio público

Respetar los derechos de autor es responsabilidad del usuario.
