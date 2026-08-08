# Módulo 1 — Agente base

Vatia recibe por chat el mensaje desordenado de un cliente que consulta por
energía solar. Identifica el producto, extrae los datos disponibles y decide:
si están completos, registra la consulta en Airtable; si falta alguno, no
registra nada y responde indicando qué dato pedir.

**Arquitectura:** Chat Trigger → AI Agent (Tools Agent, Claude Haiku 4.5,
máx. 8 iteraciones) → herramienta Airtable acoplada lateralmente → log de
observabilidad vía HTTP.

**Archivos:** `checkpoint1_santiago_larrain.json` y capturas de la ejecución.
