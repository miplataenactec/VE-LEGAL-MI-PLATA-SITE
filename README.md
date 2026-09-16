# Documentos legales de Mi Plata

Sitio estático que publica la política de privacidad de
[Mi Plata](https://github.com/EdderCastro28/VE-MOBILE-MI-PLATA-APP) en una URL
pública, que es lo que Google Play exige en la ficha de la tienda.

| Ruta | Documento |
|---|---|
| `/` | Política de privacidad (español) |
| `/en/` | Privacy policy (English) |

## Por qué este repositorio existe aparte

Es **público a propósito**: GitHub Pages solo publica gratis desde repositorios
públicos, y una política de privacidad es un documento público por definición.
El repositorio de la aplicación se mantiene privado.

Tampoco se sirve desde el backend: ese corre en el plan gratuito de Render, que
suspende el servicio tras unos minutos sin tráfico y tarda cerca de un minuto en
despertar. Una URL de política que expira durante una revisión de Play es un
riesgo que no hace falta correr. Un sitio estático responde siempre.

`.nojekyll` desactiva el procesado de Jekyll: son archivos HTML servidos tal
cual, sin plantillas ni dependencias.

## Al cambiar la política

La fuente de verdad es
`docs/politica-de-privacidad.md` en el repositorio de la aplicación, y el texto
que la app muestra en Ajustes vive en `lib/l10n/app_es.arb` y `app_en.arb`.

**Los tres tienen que decir lo mismo.** Una divergencia entre lo publicado y lo
que muestra la app es exactamente lo que una revisión señala. Al tocar uno,
actualiza los otros dos y la fecha de «última actualización» en los tres.
