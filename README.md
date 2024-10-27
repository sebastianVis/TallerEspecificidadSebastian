Parte 1: Introducción teórica a la especificidad.

<h2>1. ¿Qué es la especificidad?</h2>
  - El navegador decide que reglas del CSS aplica, dependiendo de su peso, siempre escogiendo la opción con mas relevancia en el HTML (Etiqueta = 1), (Clase = 10), (ID = 100).

  - Los selectores básicos son:
    -Tipo : div{..}
    -Clase : .elemento{..}
    -ID : *id-del-elemento{..}
    -Atributo : a[href=""]{..}
    -Universal : *{}
    
2. Reglas de calculo de especificidad:
  -Selectores de ID (100 puntos).
  -Selectores de clase, atributos y pseudoclases (10 puntos).
  -Selectores de elementos y pseudoelementos (1 punto).
  -! important : Este selector solo lo podemos utilizar cuando necesitamos que algo funcione si o si por encima de todo, no es una buena practica

   Link a las diapositivas https://www.canva.com/design/DAGUlbzGR-Q/O888yApm_0OPPjZzZbRGtA/view?utm_content=DAGUlbzGR-Q&utm_campaign=designshare&utm_medium=link&utm_source=editor


<h2>Parte 2: Ejemplos Prácticos</h2>
1. Ejemplo Basico:
![si](https://github.com/user-attachments/assets/c6243cdf-d1e2-40e6-bec8-770828f4776d)

El resultado esperado es que el texto sea rojo, puesto que el selector ID posee mayor especificidad que los selectores de clase y etiqueta.

2. Demostración de ! important:
   
![image](https://github.com/user-attachments/assets/d086c8b4-9b10-43cb-a09f-9ff7e87378a7)

En este documento podemos ver que no importa que tanta especificidad posean los otros elementos, porque !important tiene prioridad.

<h2>Parte 3: Ejercicios Prácticos</h2>

Ejercicio 1: Calculando la especificidad

Dado el siguiente codigo, los participantes deben calcular la especificidad y determinen que estilos se aplicarán:

![image](https://github.com/user-attachments/assets/a69d8632-5b5a-48d5-b028-4643910d7876)

Pregunta:
  - ¿Qué color tendrá el título h1?
  - Respuesta: El titulo será de color rojo, puesto que el selector ID tiene mayor especificidad.

Ejercicio 2: Resolviendo conflictos de especificidad.

Modifica el siguiente código para que el párrafo tenga color amarillo, sin usar !important

![image](https://github.com/user-attachments/assets/99df0009-55f7-436e-bfe9-8f6c6ca50faf)

Una solución, es agregar un selector con mayor especificidad, como en este caso, ID:

![image](https://github.com/user-attachments/assets/f6dd7679-71e2-43bc-80e2-2c2fe94edf6d)

<h2>Parte 4: Desafío Final</h2>

Dales a los participantes un archivo HTML con múltiples elementos y clases, y pídeles que
agreguen estilos CSS para lograr un diseño específico. Deberán aplicar todo lo aprendido sobre
especificidad para resolver los conflictos y obtener el resultado correcto.
HTML:

![image](https://github.com/user-attachments/assets/e36f0529-fca5-48ac-9ecc-57ce07d919b6)

Desafío CSS:
  -El h1 en el header debe ser de color blanco
  -El texto del p en .content debe ser rojo.
  -El texto del footer debe ser gris.

Pistas:
  -Usar selectores combinados (clases y etiquetas).
  -Resolver conflictos de estilo con la especificidad correcta.


<h2>Parte 5: Revisión y discusión</h2>

La solución de un participante fue la siguiente:

![image](https://github.com/user-attachments/assets/373b4d6a-10f0-45e6-82b6-f3edc48b1f33)

Como podemos observar, el participante hace un buen uso de las selectores, que aunque no son los mas fuertes, no van a presentar un conflicto entre si.

Otro participante dio la siguiente solución:

![image](https://github.com/user-attachments/assets/f0305a78-f953-4118-ad1e-2a02a512313c)

Este participante cumplió con las reglas y de la misma forma, utilizó los selectores de mas alta especificidad disponibles.

Errores comunes que pueden utilizar es no escribir correctamente el selector, ya sea haber escrito una clase con un #, o un ID con un . al principio. Lo mejor que podemos hacer es escribir el selector meticulosamente para que no se presenten conflictos.

Conclusión:

Los Participantes, ahora conocen como se calcula la especificidad, tomando en cuenta los selectores basicos de forma correcta. Así mismo, pudieron evitar conflictos aplicando la especificidad correcta, y entienden como utilizar ! important cuando es necesario.
