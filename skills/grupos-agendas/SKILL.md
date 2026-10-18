---
name: grupos-agendas
description: Arma el grupo y la agenda que envían una plantilla de WhatsApp. Usar cuando pidan a quién escribirle, qué días, o programar un envío.
---

Llamá `guia_suplai` con tema `grupos-y-agendas`. No inventes pasos. La lista es `listar_envios`. Crear, cambiar y borrar una agenda es `previsualizar_agenda` con `accion` `alta`, `editar` o `baja`. El grupo que ya existe se cambia con `previsualizar_grupo`. `confirmar` solo recibe el `preview_id`. `modo=fijo` con la posición `producto` vacía usa `clients.metadata.top_products` de cada comercio. `modo=por_cliente` no lleva `dynamic_params` y exige una estrategia con plantillas aprobadas. Para ver el mensaje en un teléfono, `previsualizar_plantilla` con `accion=probar`.
