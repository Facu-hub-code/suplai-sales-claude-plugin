---
name: manual-conector
description: Explica qué puede hacer el conector de Suplai Sales y cómo pedirlo. Usar cuando pregunten qué se puede hacer, cómo funciona, o pidan ayuda.
---

# Manual del conector

Respondé solo con las herramientas de esta lista. No inventes pantallas del backoffice ni capacidades que no estén acá.

## Herramientas

- `consultar_pedidos`. Pedidos recientes, de un cliente, de un estado, el detalle de uno o un ranking. Ejemplo: “¿Cuáles fueron los últimos 10 pedidos?”. Fechas y formato: skill `consultar-pedidos`.
- `listar_listas_precios`. Listas para elegir un `lista_precios_id` antes de cargar.
- `previsualizar_carga` y `confirmar_carga`. Revisan y guardan clientes o productos. Cómo mapear el Excel: skill `cargar-datos`.
- `listar_plantillas`, `columnas_plantilla`, `salud_whatsapp` y `metricas_plantillas`. Estado de las plantillas, variables permitidas, cupo del número y rendimiento.
- `previsualizar_plantilla` y `confirmar_plantilla`. Crean una plantilla nueva. Queda en revisión. Skill `plantillas-whatsapp`.
- `listar_grupos`, `previsualizar_agenda` y `confirmar_agenda`. Dicen a quién y cuándo llega una plantilla. La agenda nace inactiva. Skill `grupos-agendas`.
- `estado_erp`, `previsualizar_erp` y `confirmar_erp`. Muestran lo que el ERP ya trajo y lo incorporan. No abren una sync nueva. Skill `erp`.
- `listar_etiquetas`, `previsualizar_etiqueta`, `confirmar_etiqueta`, `previsualizar_estrategia` y `confirmar_estrategia`. Etiquetan un grupo o crean una estrategia sobre una agenda existente. Skill `estrategias`.
- `metricas_conversaciones`. Conteos de charlas y hasta cinco ejemplos sin teléfono ni texto. Skill `conversaciones`.
- `busquedas_sin_match`, `previsualizar_aliases` y `confirmar_aliases`. Frases que el agente no encontró y sinónimos de un SKU. Skill `aliases`.

## Todavía no

Conectar credenciales del ERP, empujar pedidos, editar el prompt del agente y borrar datos. Tampoco se edita el texto de una plantilla ya creada: hay que crear otra. No se manda un WhatsApp de prueba desde el chat.

## Cuando una tool escribe

Mostrá el preview en el chat y esperá un sí de la persona. Recién ahí llamá la tool de confirmar que corresponda. Si dice que no, no la llames.
