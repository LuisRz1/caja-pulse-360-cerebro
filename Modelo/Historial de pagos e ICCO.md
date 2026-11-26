---
aliases:
  - ICCO
tipo: metodología
estado: pendiente-de-integración
tags:
  - modelo
  - pagos
---

# Historial de pagos e ICCO

El índice de cobertura de cuota observada (ICCO) divide el monto pagado en un periodo entre la cuota programada para ese periodo. La cobertura acumulada divide las sumas de pagos y cuotas. Las fechas, los pagos fraccionados y la aplicación de regularizaciones o adelantos ayudan a interpretar esos indicadores.

| Mes | Cuota | Pago | ICCO |
| --- | ---: | ---: | ---: |
| Enero | S/ 1.000 | S/ 700 | 0,70 |
| Febrero | S/ 1.000 | S/ 1.300 | 1,30 |
| Marzo | S/ 1.000 | S/ 1.000 | 1,00 |
| Abril | S/ 1.000 | S/ 1.300 | 1,30 |
| Mayo | S/ 1.000 | S/ 700 | 0,70 |

La secuencia ficticia tiene **100 % de cobertura acumulada**, **26,83 % de volatilidad poblacional** y **40 % de periodos con pagos inferiores a la cuota programada**. Determinar el atraso contractual exige saber cuándo se pagó y a qué concepto se aplicó. Para periodos cuya cuota programada sea cero o desconocida, el ICCO queda sin calcular.

El historial complementa la verificación. Un ratio que convierta directamente estos pagos en ventas o utilidad mezclaría fuentes de pago distintas, como capital de trabajo o endeudamiento. Multiplicar `cuota / FCP` por `ICCO` equivale a `pago / FCP` y mantiene esa dependencia.

Para implementarlo, partir del [contrato de datos](../Datos/Origen%20y%20contrato%20de%20datos.md) y comparar su aporte en el [plan de validación](../Validacion/Plan%20de%20validaci%C3%B3n.md).
