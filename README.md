# Suplai Sales para Claude

Este plugin conecta Claude con una distribuidora en Suplai Sales. Un gerente comercial consulta pedidos, carga datos, arma plantillas y agendas, incorpora lo que el ERP ya trajo y crea estrategias, siempre sobre su cuenta. Cada escritura muestra un preview y espera un sí.

El plugin no ejecuta código en tu computadora. Solo apunta al servidor remoto de Suplai. Los datos viajan a `https://mcp.suplaisales.com` y al servidor de autorización `https://api.suplaisales.com`. No se envían a otros destinos.

## Requisitos

- Una cuenta de Suplai Sales en una distribuidora activa.
- El mismo email y contraseña del backoffice.

## Instalación

1. En el directorio de Claude, buscá **Suplai Sales** e instalá el plugin.
2. Autenticáte cuando Claude lo pida.
3. Preguntá, por ejemplo: “¿Cuáles fueron los últimos 10 pedidos?”.

También podés conectar solo el servidor MCP en `https://mcp.suplaisales.com/mcp`. Si tenés el plugin y el conector, ves un solo set de herramientas.

## Privacidad

Claude recibe los pedidos que pide la herramienta. Suplai guarda una auditoría de cada llamada. Detalle en la [política de privacidad](https://www.suplaisales.com/privacidad).

## Soporte

Escribí a facundo@suplaisales.com. Guía: https://www.suplaisales.com/claude.
