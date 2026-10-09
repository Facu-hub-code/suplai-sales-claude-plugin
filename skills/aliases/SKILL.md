---
name: aliases
description: Muestra búsquedas del agente que no encontraron producto y agrega sinónimos a un SKU que ya existe. Usar cuando pregunten qué no está encontrando el agente o pidan un alias.
---

# Sinónimos

## Qué no encuentra

`busquedas_sin_match` lista frases y cuántas veces volvieron vacías, de los últimos 30 días. Si la traza no está activa, decilo. No inventes búsquedas.

## Agregar un sinónimo

Filas de alias y código. Hasta 100. El código tiene que existir. Si el sinónimo ya es de otro producto, esa fila se rechaza: no lo pases de un SKU a otro.

`previsualizar_aliases` y, después de un sí, `confirmar_aliases`. El alta encola la vectorización. No reescribas el prompt del agente: eso se hace en el backoffice.
