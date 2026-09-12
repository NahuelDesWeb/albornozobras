# Historial de cambios y deploys — AlbornozObras (NRVERTEX)

## 2026-09-11 22:56 ART — Deploy `6aa4b1453de1606e2a416575` (producción)
**Qué cambió:**
- Tracking exacto de oportunidades en los 3 HTML (`index.html`, `privacidad/`, `terminos/`).
- GTM unificado al contenedor nuevo `GTM-NLJH9QCG` (antes: homepage sin GTM, solo `AW-880897335` suelto).
- GA4 `G-67BKKSQPRG` agregado al homepage (antes no medía nada ahí).
- Eliminado `AW-880897335` del homepage (ID de Ads distinto al resto del sitio).
- Cada click en WhatsApp (`generate_lead_whatsapp`) y llamada (`click_call`) envía la sección exacta: hero, nav_menu, float, servicios, nosotros, proyectos, contacto, cta_final, footer, legal, header, soluciones, faq.
- Número único en todo el sitio: `5491172383806`.
- Diseño y contenido intactos (solo se agregaron atributos y scripts de medición).

**Commits GitHub (rama `main`):** `f54cf91` (respaldo inicial) → `001df2f` (tracking) → `5a8f615` (GTM-NLJH9QCG) → `d3201d8` (merge).
**Deploy Netlify:** manual por API (solo se subieron los 3 HTML cambiados), título con fecha/hora, estado `ready` y publicado como deploy de producción.
**Pendiente del lado del cliente:** marcar los 2 eventos como clave en GA4 + crear dimensiones `cta_location` y `cta_text` + prueba en Tiempo real.
