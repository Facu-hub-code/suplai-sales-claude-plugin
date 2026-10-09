---
name: erp
description: Muestra el estado del ERP y incorpora al catálogo productos, clientes o una lista que el ERP ya trajo. Usar cuando pregunten por la sincronización, lo pendiente del ERP, o pidan dar de alta lo que ya está en el espejo.
---

# ERP

No se abre una sincronización nueva, no se cargan credenciales y no se empujan pedidos.

## Estado

`estado_erp` dice si hay conector, la última sync y cuántos productos, listas y clientes están pendientes. Si no hay ERP, decilo y no prometas una carga.

## Incorporar

`previsualizar_erp` y, después de un sí, `confirmar_erp`. El tipo es productos, clientes o lista.

- Productos: el sí cubre los SKU del preview. Cada uno entra con una descripción corta a partir del nombre del ERP y queda vectorizado. No inventes precio.
- Clientes: solo los de la cola cuyo teléfono se puede normalizar. El resto se explica con el motivo, sin repetir el teléfono.
- Lista: hace falta el `raw_id` y, o una lista de Suplai, o crear una nueva. Las dos cosas juntas no van. Si el vínculo entra y los precios no, decilo: la lista quedó vinculada y el preview sigue vigente.
