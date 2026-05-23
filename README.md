# Legal — Antojo

Documentos legales de la app Antojo. Servidos públicamente desde GitHub Pages
bajo la organización **antojo-app** (sin exponer cuenta personal del developer).

## 📂 Contenido

- [`privacy.md`](privacy.md) — Política de Privacidad
- [`terms.md`](terms.md) — Términos y Condiciones

## 🌐 URLs públicas

- **Privacidad**: https://antojo-app.github.io/legal/privacy
- **Términos**: https://antojo-app.github.io/legal/terms

Estas URLs se usan en:

- **Google Play Console** → "Privacy Policy URL" (obligatorio)
- **App** → pantalla "Mi cuenta" (links a estos docs)
- **Onboarding** (opcional, link "Al continuar aceptás...")

## 🚀 Cómo se publicaron (referencia para mantenimiento)

### Setup inicial (ya hecho)

1. Creada **organización GitHub**: `antojo-app` (plan Free)
2. Creado repo público dentro: `antojo-app/legal`
3. Subidos los .md
4. **Settings → Pages**:
   - Source: Deploy from branch
   - Branch: `main` / folder: `/ (root)`

### Cómo actualizar los documentos

1. Editar el `.md` que necesitas
2. Actualizar la fecha de "Última actualización" arriba
3. Push:

```bash
cd C:\wamp64\refriap\legal
git add .
git commit -m "Update legal docs"
git push
```

GitHub Pages se actualiza automáticamente en 1-2 minutos.

## ⚠️ Importante

Si cambiás de hosting (ej: te comprás dominio `antojo.app`):

1. Actualizar **URLs en la app**: `AccountScreen.tsx` líneas con `PRIVACY_URL` y `TERMS_URL`
2. Actualizar **Privacy Policy URL en Google Play Console**
3. Build + redeploy
