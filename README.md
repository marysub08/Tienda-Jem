# Tienda JEM · Julio Espósito MTB

Tienda online estática (un solo `index.html`) que lee los productos de una planilla de Google Sheets.
Los pedidos llegan por WhatsApp al 261 681-4824.

## Cómo se actualiza
Todo se maneja desde la planilla (productos, precios, promos, avisos y promos DNI).
Los cambios aparecen solos en la tienda en uno o dos minutos. No hace falta volver a subir nada.
La pestaña **Instrucciones** de la planilla explica cada columna.

## Configuración (una sola vez)
En `index.html`, bloque `CONFIG`:
- `SHEET_ID`: el ID de la planilla (lo que está entre `/d/` y `/edit` en el link).
  Mientras esté vacío, la tienda muestra productos de ejemplo ("modo demo").
- `WHATSAPP`: número para los pedidos (formato internacional, sin +).

La planilla tiene que estar compartida como **Cualquier persona con el enlace → Lector**.

## Archivos
- `index.html`: la tienda completa
- `img/logo.png`: logo JEM
- `fotos/`: fotos locales de productos (opcional; también se pueden usar links de Drive)

## Publicación
Repo conectado a Vercel: cada cambio que se sube al repo se publica solo.
