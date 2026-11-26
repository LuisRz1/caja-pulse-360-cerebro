---
tipo: decisiones
actualizado: 2026-11-25
tags:
  - proyecto
  - decisiones
---

# Decisiones y supuestos

| Decisión de diseño | Motivo | Qué requiere revisión |
| --- | --- | --- |
| Empezar por créditos vigentes y enfocar el caso en clientes al día | La acción preventiva tiene valor antes del atraso | Población y casos elegibles. |
| Estimar resistencia a escenarios | Permite explicar qué variable consume el margen aun con evaluación parcial | Horizonte, escenarios y alcance de las conclusiones. |
| Usar FCP ilustrativo de 65 % en A/B | Hace replicable el cálculo preventivo | Validez del factor por producto en créditos vigentes. |
| Usar pagos como señal crediticia complementaria | La procedencia de fondos para pagar puede variar | Diferencias entre pago observado, adelanto, regularización y atraso contractual. |
| Consultar fuentes públicas y usar un LLM opcional | Permite generar hipótesis sectoriales trazables y conservar la simulación reproducible | Gasto, estabilidad y ganancia frente a reglas simples. |
| Registrar confianza por separado | El faltante limita lo que se puede afirmar sobre el perfil | Regla operativa para priorizar verificaciones. |
| Preparar datos sintéticos propios | El equipo puede avanzar mientras confirma los insumos de Caja | Representatividad y aceptación de los casos de prueba. |

La recomendación se destina a revisión humana. El diseño reserva aprobación, cambios contractuales y contacto con clientes para la operación autorizada de la Caja.

Para registrar un acuerdo nuevo, usa la [plantilla de decisión](../Plantillas/Plantilla%20de%20decisi%C3%B3n.md). Revisa las [preguntas para Riesgos](Preguntas%20para%20Riesgos.md) antes de cambiar un supuesto.
