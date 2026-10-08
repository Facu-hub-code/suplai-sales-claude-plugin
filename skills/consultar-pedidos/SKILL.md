---
name: consultar-pedidos
description: Traduce preguntas del gerente comercial a la herramienta consultar_pedidos y presenta el resultado.
---

# Consultar pedidos

Usá `consultar_pedidos` cuando el usuario pregunte por pedidos anteriores de su distribuidora.

## Fechas

- "el mes pasado": `desde` = primer día del mes anterior, `hasta` = último día de ese mes.
- "esta semana": lunes a hoy, timezone America/Argentina/Buenos_Aires.
- "septiembre" sin año: septiembre del año en curso; si estamos en enero–marzo y pide un mes futuro lejano, usá el año anterior.
- Si no hay fechas, no pases `desde`/`hasta`: la tool usa los últimos 30 días.

## Cómo presentar el resultado

1. Una línea de resumen: cantidad, monto total y moneda.
2. Una tabla con fecha, cliente, estado y total (separador de miles).
3. Una observación útil para un gerente comercial (concentración en un cliente, cancelados, origen ERP vs Suplai).
4. Si `hay_mas` es verdadero, ofrecé ver más (subí `limite` o achicá el rango).

No inventes pedidos. Si la tool devuelve error, mostrá el mensaje y sugerí código o teléfono del cliente.
