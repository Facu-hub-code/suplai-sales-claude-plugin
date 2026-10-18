---
name: plantillas-whatsapp
description: Crea o explica plantillas de WhatsApp de Suplai. Usar cuando pidan un mensaje para contactar, promocionar, ver el estado de una plantilla, la salud del número o cómo rindió un envío.
---

Llamá `guia_suplai` con tema `plantillas`. No inventes pasos. El cupo y el rendimiento salen de `metricas_whatsapp`. Las columnas válidas salen de `listar_plantillas`, campo `columnas_variables`. Crear, probar y borrar es `previsualizar_plantilla` con `accion` `alta`, `probar` o `baja`. Probar pide el nombre aprobado y un teléfono: la respuesta trae `clients.metadata.top_products`, los productos y los `dynamic_params`. `confirmar` manda ese único WhatsApp.
