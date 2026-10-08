---
name: cargar-datos
description: Carga clientes o productos de un Excel a Suplai. Usar cuando pidan importar, subir o acomodar un archivo de contactos, precios o catálogo.
---

# Cargar clientes y productos

El Excel lo leés vos. Al conector le mandás lotes ya acomodados, de hasta 100 filas. Si hay más, partí el archivo y hacé un preview por tanda.

No inventes precio, stock ni teléfono. Si el archivo no trae el dato, dejá el campo vacío para que el server lo rechace o avise.

## Columnas

Clientes: `telefono`, `razon_social`, `lista_precios_id`. Opcionales: `nombre`, `codigo`, `dia_de_visita`, `dia_de_entrega`, `email`, `cuit`, `direccion`.

Productos: `product_code`, `nombre`, `precio_unidad`. Opcionales: `stock`, `descripcion`, `unidades_por_bulto`, `unidad_minima_de_venta`, `aliases` (lista de sinónimos del nombre, si se ven en el archivo).

Nombres típicos de columna: teléfono / celular / whatsapp → `telefono`. Razón social / comercio / cliente → `razon_social`. SKU / código → `product_code`. Precio / precio final → `precio_unidad`.

## Lista de precios

Antes de previsualizar productos, llamá `listar_listas_precios` y preguntá cuál lista activa y pública corresponde. Una columna de precio, una lista. Si el Excel trae varias columnas de precio, un preview por lista, no las mezcles en la misma fila.

En clientes, `lista_precios_id` también es obligatorio: usá la misma lista que eligió la persona.

## Cómo cerrar

1. Llamá `previsualizar_carga`.
2. Mostrá una tabla corta: aceptadas, rechazadas y las que ya existen, con el motivo. En productos, mostrá si entra al catálogo, la lista, el precio y el stock.
3. Si la persona dice que sí, llamá `confirmar_carga` con ese `preview_id` y nada más.
4. Si dice que no, no confirmes. Un preview vence a los 30 minutos y no se puede confirmar dos veces.
