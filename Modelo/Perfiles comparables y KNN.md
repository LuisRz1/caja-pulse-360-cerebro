---
aliases:
  - KNN
tipo: metodología
estado: pendiente-de-integración
tags:
  - modelo
  - datos-faltantes
---

# Perfiles comparables y KNN

Los vecinos más cercanos podrían aportar referencias cuando falten variables en una evaluación. Se parte de registros autorizados y fechados. Para escoger comparables pueden usarse sector, zona, antigüedad, destino del crédito, monto, cuota y plazo, según disponibilidad al corte.

## Criterios de implementación

1. Preparar variables numéricas en escalas comparables y tratar las categorías de forma explícita.
2. Exigir una cantidad mínima de vecinos con el campo buscado y una similitud suficiente. Los criterios se ajustan con validaciones que oculten valores conocidos.
3. Guardar origen, fecha y dispersión de los valores de referencia. Comprobar la coherencia entre ventas, costos, gastos y utilidad.
4. Abstenerse si faltan variables de comparación o si los vecinos son insuficientes. En ese caso, mostrar qué campo debe verificarse.

## Ejemplo ilustrativo

Cinco negocios comparables reportan ventas de S/ 7.500 a S/ 10.000, con media de S/ 8.600. La media sería una referencia y el rango describe a los vecinos. La ficha mostraría ambos junto al estado **estimado**.

En el código actual, el cliente ficticio C conserva el umbral calculable y queda sin simulación individual porque le faltan ventas. El [caso A/B](../Validacion/Caso%20A%20y%20B.md) documenta esa abstención. Ver [procedencia de datos](../Datos/Origen%20y%20contrato%20de%20datos.md).
