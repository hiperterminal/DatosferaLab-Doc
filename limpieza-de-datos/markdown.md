---
icon: markdown
layout:
  width: default
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
---

# Problemas de los datos

Los problemas con los datos son una cuestión más compleja para tratar en cuanto a que estos pueden venir dados por múltiples factores. Por este motivo, no siempre vamos a poder solucionar los problemas. Pero que no tengan solución no impide su uso, si no se trata de un dato clave o que pueda hacer que el análisis lleve a resultados erróneos, podremos continuar. Es importante por ello que cuando la importación haya sido realizada con éxito revisemos los datos en profundidad:

{% stepper %}
{% step %}
**Identificando ausencias en los datos, anomalías y valores atípicos**


{% endstep %}

{% step %}
**Analizando si se tratan de fallos**


{% endstep %}

{% step %}
**En caso de ser errores, busquemos soluciones.**


{% endstep %}
{% endstepper %}

La presencia de datos anómalos, como un valor numérico muchísimo más elevado o reducido que el resto, no debe verse siempre como un problema a tratar. Que en los datos de las calificaciones de un examen todo el alumnado haya obtenido un 5 salvo una persona que tiene un 10, es algo plausible, pero que esa excepción sea un 15 sí es algo que debe ser revisado pues se sale del valor máximo esperado.

Como ejemplo de estos problemas, imagina que estamos trabajando con los datos que hemos generado de una encuesta. Al importar los datos nos encontramos con personas que han rellenado dos veces la encuesta cuando solo pueden una o que varias personas han dado una misma respuesta a una pregunta, pero usando variantes de la misma palabra (por ejemplo SÍ, sí, SI, SII!). En este caso tendremos que eliminar los duplicados y unificar las distintas variantes de la respuesta en una sola.
