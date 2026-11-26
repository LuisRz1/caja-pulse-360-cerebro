---
tipo: datos
estado: diseño
tags:
  - datos
  - trazabilidad
---

# Origen y contrato de datos

Las fuentes internas son las previstas en el diseño. Su disponibilidad, autorización y calidad todavía deben comprobarse con la Caja.

| Información | Origen previsto | Aporte del cliente |
| --- | --- | --- |
| Sector, ubicación operativa, antigüedad y destino | Ficha de originación o expediente del negocio | Se declaran al solicitar el crédito y pueden confirmarse si cambian. |
| Cuota, producto, cronograma, vencimientos y saldo | Registro crediticio al corte | La Caja consulta su registro. El asesor puede aclarar discrepancias con el cliente. |
| Factor de capacidad de pago (FCP) | Regla de Riesgos por producto | La entidad valida su uso como umbral preventivo. |
| Fecha, importe y aplicación de cada pago | Registro de cobranzas, cruzado con cronograma | Los pagos ya registrados sirven de evidencia. El asesor puede pedir una aclaración puntual. |
| Ventas, costos, gastos, otras deudas y carga familiar si corresponde | Última evaluación económica disponible y fechada | Se aprovecha lo que el cliente aportó en la evaluación. Si hay una señal, se solicita el dato puntual que ayudaría a verificarla. |
| Valores económicos faltantes | Registros autorizados de comparables y método KNN | Puede requerirse una actualización económica si los comparables son insuficientes. |
| Producción, precios y clima | Series relevantes por periodo y cobertura | Se consultan en fuentes públicas. |

## Datos mínimos y casos parciales

- **Umbral preventivo.** Cuota vigente y FCP validado. Con cuota y estructura económica se puede medir insuficiencia bajo un escenario aunque falte el FCP.
- **Señales de pago.** Cronograma e historial con fechas, importes y aplicación. El [ICCO](../Modelo/Historial%20de%20pagos%20e%20ICCO.md) requiere una cuota programada positiva por periodo.
- **Simulación individual.** Ventas, costos variables, otros gastos y obligaciones antes de la cuota evaluada, fecha de evaluación y cuota. Si falta una variable, [comparables](../Modelo/Perfiles%20comparables%20y%20KNN.md) podrían aportar una estimación trazable.
- **Contexto sectorial.** Actividad y zona, un indicador pertinente y sus metadatos. La información sectorial puede motivar una verificación.

## Contrato propuesto

Cada valor conserva fuente, fecha de observación, fecha de corte del análisis y procedencia. Los tipos de procedencia son observado, estimado, simulado o faltante. Usar `null` para un faltante y cero para un valor efectivamente registrado como cero. Conservar moneda y unidad. En el prototipo, los importes de los perfiles están en soles mensuales.

El [registro de fuentes](Registro%20de%20fuentes.md) reúne los indicadores públicos. El [archivo de perfiles de ejemplo](https://github.com/LuisRz1/caja-pulse-360-modelo/blob/main/perfiles-sinteticos.json) documenta los campos que recibe el simulador actual.
