---
tipo: estado
actualizado: 2026-11-25
tags:
  - proyecto
  - planificación
---

# Estado y hoja de ruta

| Entregable | Estado | Evidencia |
| --- | --- | --- |
| Presentación Concept Solution | Publicada | [Página en Vercel](https://caja-pulse-360.vercel.app/) |
| Fuentes y aporte del cliente | Publicados | [Origen de los datos](https://caja-pulse-360.vercel.app/#origen-datos) |
| Base del motor | Implementada y verificada con perfiles sintéticos | [Repositorio Python](https://github.com/LuisRz1/caja-pulse-360-modelo) |
| Contexto público de calzado | Consulta y corrida verificadas | [Fuente y observación](../Datos/Registro%20de%20fuentes.md) |
| LLM opcional | Adaptador probado con respuesta controlada | [Escenarios públicos y LLM](../Modelo/Escenarios%20p%C3%BAblicos%20y%20LLM.md) |
| Contexto consolidado y formulario | Original archivado | [AGENTS.md](https://github.com/LuisRz1/caja-pulse-360-modelo/blob/main/AGENTS.md) |

## Siguiente tramo del MVP

- Preparar clientes, evaluaciones, créditos, cronogramas y pagos sintéticos. Punto de partida propuesto de 1.000 perfiles en calzado, comercio, agricultura y transporte.
- Integrar [ICCO](../Modelo/Historial%20de%20pagos%20e%20ICCO.md), [comparables](../Modelo/Perfiles%20comparables%20y%20KNN.md) y trazabilidad de datos faltantes.
- Conectar cartera y ficha individual al motor. Mostrar prioridad y confianza por separado, con razones de revisión explícitas.
- Ejecutar la [validación comparativa](../Validacion/Plan%20de%20validaci%C3%B3n.md) y ampliar fuentes por sector según su pertinencia.

La propuesta técnica usa Python, Pandas, NumPy y scikit-learn, con Streamlit y Plotly para el MVP. CSV es el punto de partida y SQLite es una opción si se requieren consultas o persistencia. La presentación pública es un sitio independiente.

Ver las [decisiones y supuestos](Decisiones%20y%20supuestos.md), las [preguntas para Riesgos](Preguntas%20para%20Riesgos.md) y el [contexto de CAJATHÓN](Entrega%20CAJATH%C3%93N.md).
