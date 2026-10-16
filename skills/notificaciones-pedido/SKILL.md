---
name: notificaciones-pedido
description: Muestra o cambia quién recibe avisos de pedidos, asistencia o errores, por WhatsApp o por mail. El destino es un teléfono o un mail libre.
---

Llamá `guia_suplai` con tema `notificaciones-pedido`. No inventes pasos. Para ver mails y teléfonos usá solo `ver_notificaciones`. No uses `ver_notificaciones_pedido`: lee un JSON viejo y puede decir que no hay mails aunque la lista nueva tenga. Para cambiar un destino o la plantilla de WhatsApp, `previsualizar_notificaciones` y después `confirmar`. El id de plantilla sale de `listar_plantillas`. Confirmar no manda el mensaje.

