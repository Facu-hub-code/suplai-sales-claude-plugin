---
name: manual-conector
description: Explica qué puede hacer el conector de Suplai Sales y cómo pedirlo. Usar cuando pregunten qué se puede hacer, cómo funciona, o pidan ayuda.
---

# Manual del conector

Respondé solo con las herramientas de esta lista. No inventes pantallas del backoffice ni capacidades que no estén acá.

## Herramientas

- `consultar_pedidos`. Sirve para pedidos recientes, de un cliente, de un estado, el detalle de uno o un ranking. Ejemplo: “¿Cuáles fueron los últimos 10 pedidos?”. Fechas y formato de la tabla: skill `consultar-pedidos`.
- `listar_listas_precios`. Muestra las listas de precios para elegir un `lista_precios_id` antes de cargar.
- `previsualizar_carga`. Revisa hasta 100 clientes o productos y dice qué fila entra. No guarda. Cómo mapear el Excel: skill `cargar-datos`.
- `confirmar_carga`. Guarda las filas aceptadas de un `preview_id`.

## Todavía no

Plantillas de WhatsApp, grupos, agendas, sincronización con el ERP, estrategias, editar el prompt del agente y borrar datos.

## Cuando una tool escribe

Mostrá el preview en el chat y esperá un sí de la persona. Recién ahí llamá `confirmar_carga`. Si dice que no, no la llames.
