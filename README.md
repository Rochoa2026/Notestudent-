# NoteStudent v6 Multidioma — GitHub Pages

## Objetivo
Versión gratuita, sin servidor de pago y sin claves API.

## Flujo
1. Graba la conferencia completa en su idioma original.
2. El audio se conserva por segmentos.
3. Al finalizar, la aplicación pregunta:
   - idioma hablado;
   - idioma deseado para el texto.
4. La transcripción se intenta realizar localmente en el navegador con Whisper Tiny.
5. Si el navegador admite traducción local, intenta traducir al idioma elegido.
6. Guarda el texto completo en la biblioteca local.

## Muy importante
La transcripción local consume bastante memoria y procesamiento.
- En una computadora suele funcionar mejor.
- En teléfonos modestos puede tardar o fallar.
- La primera vez descarga un modelo de IA y necesita Internet.
- Después el navegador puede reutilizar el modelo desde caché.
- El audio original nunca se pierde por un fallo de transcripción; puede descargarse.

## Traducción
La transcripción multidioma puede detectar o usar el idioma seleccionado.
La traducción a otro idioma depende de que el navegador tenga disponible una API de traducción local.
Si no está disponible, NoteStudent conserva el texto transcrito en el idioma original.

## GitHub Pages
Sube todos los archivos a la raíz del repositorio:
- index.html
- manifest.json
- service-worker.js
- icon-192.png
- icon-512.png
- icon-512-maskable.png

Después activa Settings > Pages > Deploy from a branch > main > /(root).

## Recomendación de prueba
Primero prueba con una grabación de 30 a 60 segundos. Luego prueba 5 minutos. Solo después úsala en una conferencia larga.
