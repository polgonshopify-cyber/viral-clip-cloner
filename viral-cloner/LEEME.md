# 🎬 Viral Clip Cloner — Guía de instalación

## Qué necesitas
- Cuenta en GitHub (gratis): https://github.com
- Cuenta en Vercel (gratis): https://vercel.com
- API Key de Anthropic: https://console.anthropic.com

---

## Paso 1 — Sube el proyecto a GitHub

1. Ve a https://github.com y crea una cuenta si no tienes
2. Haz clic en **"New repository"** (botón verde arriba a la derecha)
3. Ponle nombre: `viral-clip-cloner`
4. Déjalo en **Public** y haz clic en **"Create repository"**
5. En la siguiente pantalla verás la opción **"uploading an existing file"** — haz clic ahí
6. Arrastra los 4 archivos de esta carpeta:
   - `index.html`
   - `vercel.json`
   - `package.json`
   - la carpeta `api/` con el archivo `generate.js` dentro
7. Haz clic en **"Commit changes"**

---

## Paso 2 — Despliega en Vercel

1. Ve a https://vercel.com y haz clic en **"Sign up"** → elige **"Continue with GitHub"**
2. Una vez dentro, haz clic en **"Add New Project"**
3. Busca tu repositorio `viral-clip-cloner` y haz clic en **"Import"**
4. En la pantalla de configuración, **no toques nada**, solo baja hasta ver **"Environment Variables"**
5. Añade esta variable:
   - **Name:** `ANTHROPIC_API_KEY`
   - **Value:** tu API key de Anthropic (empieza por `sk-ant-...`)
6. Haz clic en **"Deploy"**
7. Espera 1-2 minutos

---

## Paso 3 — Listo

Vercel te dará una URL como:
`https://viral-clip-cloner-tuusuario.vercel.app`

Esa es tu app. Guárdala en favoritos. Funciona desde cualquier dispositivo, para siempre, gratis.

---

## Cómo conseguir la API Key de Anthropic

1. Ve a https://console.anthropic.com
2. Crea una cuenta
3. En el menú lateral haz clic en **"API Keys"**
4. Haz clic en **"Create Key"**
5. Copia la key (empieza por `sk-ant-api03-...`)
6. ⚠️ Guárdala en un lugar seguro — solo se muestra una vez

La API de Anthropic cobra por uso (muy barato, unos céntimos por cada script generado).

---

## ¿Algo no funciona?

- Si el botón no hace nada: comprueba que la API key esté bien escrita en Vercel
- Si sale error de API: ve a console.anthropic.com y comprueba que tienes créditos
- Para actualizar la app: sube los archivos modificados a GitHub y Vercel se actualiza solo
