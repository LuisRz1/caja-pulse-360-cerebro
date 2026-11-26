---
tipo: evidencia
actualizado: 2026-11-25
tags:
  - datos
  - evidencia
---

# Registro de fuentes

| Fuente | Qué aporta | Estado |
| --- | --- | --- |
| [BCRPData · PN01927AM](https://estadisticas.bcrp.gob.pe/estadisticas/series/mensuales/resultados/PN01927AM) | Variación interanual de la producción manufacturera de calzado, de alcance nacional | Integrada y consultada en vivo para la base de Python. |
| [SENAMHI](https://www.senamhi.gob.pe/site/descarga-datos/) | Datos meteorológicos para explorar escenarios con exposición climática | Fuente candidata. Falta revisar cobertura pertinente al sector y la zona. |
| INEI, MIDAGRI y OSINERGMIN | Precios, producción agropecuaria y combustibles, según serie y cobertura | Fuentes candidatas. Hace falta seleccionar series y verificar oportunidad. |

## Observación reproducible

La consulta del **25 de noviembre de 2026** recuperó **septiembre de 2026**, con un valor de **+11,59 % interanual** en la serie nacional de producción de calzado. Esa observación sirve de contexto para el escenario de volumen. La corrida conserva el valor original, su periodo, unidad, alcance, fecha de consulta y URL de la API.

[Resultado JSON de la consulta](https://github.com/LuisRz1/caja-pulse-360-modelo/blob/main/ejemplo-contexto-publico.json) · [API de BCRPData](https://estadisticas.bcrp.gob.pe/estadisticas/series/ayuda/api)

Antes de incorporar una serie, documenta su variable, unidad, cobertura geográfica y sectorial, periodo disponible, fecha de publicación o consulta y límites de interpretación. Para repetir una evaluación histórica, conserva la versión que se conocía en la fecha de corte.

La nota de [escenarios públicos y LLM](../Modelo/Escenarios%20p%C3%BAblicos%20y%20LLM.md) explica cómo se utiliza la observación. El [plan de validación](../Validacion/Plan%20de%20validaci%C3%B3n.md) describe cómo tratar revisiones y retrasos.
