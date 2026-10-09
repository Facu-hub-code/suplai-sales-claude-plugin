---
name: grupos-agendas
description: Arma el grupo y la agenda que envían una plantilla de WhatsApp. Usar cuando pidan a quién escribirle, qué días, o programar un envío.
---

# Grupos y agendas

La plantilla no elige la audiencia. El grupo dice quién entra. La agenda junta las dos cosas con un horario. El WhatsApp lo manda el sender, no este chat.

## Filtros

Hace falta al menos un eje. Etiquetas, lista de precios y días de visita se combinan: el comercio tiene que cumplir todos los que indiques. Dentro de las etiquetas alcanza una. Dentro de los días, alcanza uno. Una zona o un grupo especial (`open_cart`, `recent_orders`, `churn_risk`) no se mezclan con esos ejes. Un grupo vacío no es “todos los clientes”.

Si nombran un grupo que ya existe y los filtros coinciden, reusalo. Si el nombre existe con otros filtros, no lo pises: ofrecé usarlo tal cual o poner otro nombre.

## Promo y variables

Si la plantilla promociona, el grupo filtra por la lista de esa promo. Pasá `promocion_id`. Si no lo pasás, el preview dice que la agenda no está atada a una promoción: no pidas el sí de una promo en ese caso.

`dynamic_params` solo para la variable `producto` (el mismo texto para todos). El nombre y la razón social salen de cada comercio.

## Orden

1. `listar_plantillas` y, si hace falta, `listar_grupos`.
2. `previsualizar_agenda`.
3. Mostrá el conteo, los comercios de la muestra, el horario, si la plantilla está aprobada y el cupo de hoy. No repitas teléfonos.
4. Si el grupo es más grande que el cupo de hoy, avisalo. No lo partas en varios envíos.
5. Esperá un sí. `confirmar_agenda` la deja inactiva.
6. `activar=true` solo si la persona pidió dejarla prendida y la plantilla ya está aprobada. Si sigue en revisión, queda inactiva y se lo decís.

No armes la estrategia, no pauses un envío que ya salió y no mandes un WhatsApp de prueba.
