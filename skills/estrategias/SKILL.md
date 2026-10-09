---
name: estrategias
description: Crea una estrategia de envío sobre un grupo y una agenda que ya existen, o asigna una etiqueta a los clientes de un grupo. Usar cuando pidan una estrategia, una cadencia o etiquetar un grupo.
---

# Estrategias y etiquetas

La estrategia usa la plantilla de una agenda que ya existe. No se elige otra salida ni se cambia el horario.

## Antes de armarla

Hace falta `grupo_id` y `agenda_id`. Si la plantilla no está aprobada, si la agenda es de otro grupo, o si la promo no usa la lista del grupo, no hay preview: explicalo.

El modo es puntual, o ciclo cada `14_dias` o `1_mes`. El ancla queda el lunes salvo que nombren otro día.

## Qué decir en el preview

Nombre de la plantilla, si está aprobada, si la agenda está activa, cuántos clientes entran y si está atada a una promo. La estrategia nace activa. El mensaje sale solo si la agenda también lo está. Confirmar no apaga ni prende la agenda.

## Etiquetas

`listar_etiquetas` muestra id y nombre. Para asignar, una etiqueta existente o un nombre nuevo, y un grupo. Se etiquetan los clientes de ese grupo. Una etiqueta por vez, sin jerarquía.
