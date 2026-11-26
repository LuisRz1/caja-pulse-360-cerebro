---
tipo: metodología
estado: implementado
tags:
  - modelo
  - escenarios
---

# Simulación Monte Carlo

La base en Python genera muestras reproducibles con NumPy. El caso A/B usa un impacto fijo. Los escenarios de estrés usan rangos triangulares con mínimo, valor central y máximo, y aplican las mismas muestras sectoriales a los perfiles comparados.

- El volumen multiplica tanto las ventas como los costos variables.
- El precio de insumos modifica el costo de cada unidad.
- Los demás gastos y las obligaciones se mantienen constantes en el caso actual.
- Los resultados incluyen utilidad central, percentiles 10, 50 y 90, y proporciones bajo el umbral preventivo o bajo la cuota.

La proporción es condicional a la distribución y al alcance elegidos. Su validación como herramienta operativa requiere escenarios independientes, un horizonte definido y comparar contra una línea base de seguimiento.

Para repetir una corrida, archiva perfiles, rangos, semilla, versión de NumPy, tamaño muestral y fuente pública. El [caso A/B](../Validacion/Caso%20A%20y%20B.md) fija las comprobaciones de cálculo. El [plan de validación](../Validacion/Plan%20de%20validaci%C3%B3n.md) recoge las comprobaciones pendientes.
