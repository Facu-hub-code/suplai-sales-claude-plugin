---
name: plantillas-whatsapp
description: Crea o explica plantillas de WhatsApp de Suplai. Usar cuando pidan un mensaje para contactar, promocionar, ver el estado de una plantilla, la salud del número o cómo rindió un envío.
---

# Plantillas de WhatsApp

El cuerpo que la persona acepta es el que se crea. Meta no deja editarlo después: otro texto es otra plantilla, con otro nombre.

## Contactar o promocionar

- Contactar (aviso de visita, saludo) va como utilidad. No pongas precios.
- Promocionar va como marketing. Antes de previsualizar, la promo tiene que existir, estar vigente y ser de una lista concreta. El SKU tiene que estar en el catálogo y con stock. Si falta algo, la tool se niega y le explicás qué falta. No inventes la promo.

## Variables

Pedí `columnas_plantilla`. Solo esas columnas. El orden es `{{1}}`, `{{2}}`, … El texto no puede empezar ni terminar en una variable. Si el Excel del cliente no trae ese dato, la variable sale vacía: decilo.

## Orden

1. Si hace falta, `listar_plantillas`, `salud_whatsapp` o `metricas_plantillas`.
2. `previsualizar_plantilla` con el texto ya escrito.
3. Mostrá el texto, el nombre ya normalizado, la categoría y las variables.
4. Esperá un sí. Recién ahí `confirmar_plantilla`.
5. Decí que quedó en revisión y que no se puede programar activa hasta que Meta la apruebe.

No des de baja plantillas. No subas imágenes ni carruseles. El grupo y el horario son la skill `grupos-agendas`.
