---
tipo: plan
estado: propuesto
tags:
  - validación
  - riesgo-crediticio
---

# Plan de validación

## Qué se verificó

El conjunto inicial de siete pruebas cubre el caso A/B, la abstención por faltantes, la reproducibilidad, la selección de un periodo válido, la validación de escenarios y el comportamiento ante fallas de la fuente o del LLM. Existe además una consulta pública en vivo de BCRPData.

## Qué medir en el prototipo

1. **Definir población, evento y horizonte.** Riesgos debe acordar qué se considera evento, en qué créditos y cuánto tiempo antes sirve una advertencia.
2. **Comparar con la línea base.** Usar reglas crediticias y el mismo conjunto de perfiles, fecha de corte, horizonte y definiciones. Medir aciertos entre alertas, sensibilidad, falsos positivos, anticipación y casos útiles entre los primeros revisados.
3. **Probar datos faltantes.** Ocultar valores conocidos para medir error y cobertura de KNN. Registrar cuántas veces se abstiene el motor y si la calidad cambia por sector, zona y disponibilidad.
4. **Evaluar el aporte de contexto.** Comparar escenarios fijos contra reglas con señales públicas y contra el LLM. Mantener el resto del motor constante. Revisar vigencia, fundamento y estabilidad de los escenarios.
5. **Separar periodos.** Conservar observaciones y parámetros disponibles en la fecha de corte. Evitar revisiones de fuentes publicadas después del corte y mantener la verdad sintética fuera de las entradas.

Una cartera sintética permite comprobar cálculos y el flujo del asesor. Para evaluar el valor en cartera real se requiere información autorizada, un estudio temporal y revisión de resultados por segmento. La reducción de mora o pérdidas queda como hipótesis por verificar.

Relacionado con el [caso A/B](Caso%20A%20y%20B.md), el [origen de los datos](../Datos/Origen%20y%20contrato%20de%20datos.md) y las [preguntas para Riesgos](../Proyecto/Preguntas%20para%20Riesgos.md).
