---
aliases:
  - Escenarios con IA
tipo: metodología
estado: parcialmente-implementado
tags:
  - modelo
  - escenarios
  - llm
---

# Escenarios públicos y LLM

El escenario describe cambios hipotéticos en las variables económicas. En el primer caso se usa la producción nacional de calzado como señal para proponer una prueba de sensibilidad sobre volumen. Una variación anual agregada aporta contexto sectorial. Los rangos mensuales del negocio se documentan como supuestos.

1. **Consultar.** El programa pide la serie oficial configurada, extrae el último periodo mensual válido y registra unidad, cobertura y consulta. El límite de 90 días desde el cierre del periodo es una regla ilustrativa del prototipo.
2. **Proponer.** En modo LLM, el proveedor recibe la observación pública, el horizonte de un mes y las condiciones del ejercicio. La salida contiene rangos mínimo, central y máximo de volumen, justificación e identificador de evidencia.
3. **Validar.** El código comprueba la cita, el orden del rango y que quede entre −15 % y +15 %. El rango y la explicación se guardan como propuesta. La estructura económica individual permanece en el motor local.
4. **Simular.** NumPy aplica los rangos a los perfiles y resume su resistencia. El informe registra el origen de la propuesta, la semilla y la evidencia.

## Modos disponibles

| Modo | Resultado |
| --- | --- |
| `local` | Caso A/B y estrés de insumos con parámetros de demostración. |
| `publico` | Añade el escenario contextual por reglas cuando BCRPData aporta una observación válida. |
| `llm` | Pide al modelo un escenario. Si la respuesta falla, conserva el escenario por reglas cuando hay fuente válida. |

Se verificaron la consulta en vivo a BCRPData y la validación del adaptador con una respuesta de prueba. El paso de inferencia con un modelo real requiere credenciales y configuración de Vercel AI Gateway.

Ver [el registro de fuentes](../Datos/Registro%20de%20fuentes.md), [la simulación](Simulaci%C3%B3n%20Monte%20Carlo.md) y la [plantilla de escenarios](../Plantillas/Plantilla%20de%20escenario.md).
