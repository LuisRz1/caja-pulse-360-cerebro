---
aliases:
  - FCP
tipo: metodología
estado: implementado
tags:
  - modelo
  - finanzas
---

# Capacidad de pago y FCP

El factor de capacidad de pago (FCP) expresa un límite de cuota respecto de la utilidad disponible. Su uso preventivo para créditos vigentes y el valor por producto deben confirmarse con Riesgos. El **65 % del caso de demostración es ilustrativo**.

| Indicador | Definición |
| --- | --- |
| Utilidad disponible | Ventas menos costos, gastos y otras obligaciones, antes de restar la cuota evaluada. |
| Umbral preventivo | Cuota ÷ FCP. Se cruza cuando la utilidad simulada cae por debajo del umbral. |
| Umbral de insuficiencia | La cuota. Por debajo de ella, la utilidad simulada resulta insuficiente. |
| Margen cero | La utilidad simulada alcanza exactamente para cubrir la cuota. |
| Ratio cuota sobre utilidad | Cuota ÷ utilidad, definido si la utilidad es positiva. |
| Alza de costos tolerable | (Utilidad inicial − umbral preventivo) ÷ costos variables iniciales, con los demás rubros constantes. Se informa margen cero si ya está en el umbral o por debajo. |

Al armar el perfil, descuenta las demás obligaciones una sola vez. Si falta FCP, se puede conservar la comparación entre utilidad y cuota cuando la estructura económica es utilizable. Si la fecha de evaluación es posterior al corte, el motor se abstiene de calcular el caso individual.

Ver [el caso A/B](../Validacion/Caso%20A%20y%20B.md), [la simulación](Simulaci%C3%B3n%20Monte%20Carlo.md) y [lo que debe confirmar Riesgos](../Proyecto/Preguntas%20para%20Riesgos.md).
