---
tipo: demostración
estado: verificado-con-datos-sintéticos
tags:
  - validación
  - calzado
---

# Caso A y B

Dos negocios ficticios de calzado están al día. Ambos declaran S/ 12.000 de ventas mensuales y tienen S/ 2.000 en otros gastos y obligaciones. La cuota de ambos es S/ 1.200. Con FCP ilustrativo de 65 %, el umbral preventivo común es S/ 1.846,15.

| Variable | A | B |
| --- | ---: | ---: |
| Costos variables de partida | S/ 7.000 | S/ 8.000 |
| Utilidad de partida | S/ 3.000 | S/ 2.000 |
| Utilidad con costos 10 % mayores | S/ 2.300 | S/ 1.200 |
| Cuota sobre utilidad bajo ese supuesto | 52,17 % | 100 % |
| Alza tolerable antes del umbral preventivo | 16,48 % | 1,92 % |

B queda bajo el umbral preventivo y conserva justo lo necesario para la cuota. Una verificación útil sería preguntar si subieron los insumos y cómo está financiando su compra. A conserva margen bajo el mismo supuesto.

El perfil ficticio C conserva su umbral por cuota y FCP. Como le faltan ventas, el informe registra el dato faltante y deja pendiente la simulación individual.

El caso está en la [demostración interactiva](https://caja-pulse-360.vercel.app/#simulador) y en las [pruebas del motor](https://github.com/LuisRz1/caja-pulse-360-modelo/blob/main/tests/test_modelo.py). Consulta los [umbrales](../Modelo/Capacidad%20de%20pago%20y%20FCP.md) y el [plan de validación](Plan%20de%20validaci%C3%B3n.md).
