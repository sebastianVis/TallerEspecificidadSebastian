Parte 1: Introducción teórica a la especificidad.

1. ¿Qué es la especificidad?
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


Parte 2: Ejemplos Prácticos

![si](https://github.com/user-attachments/assets/c6243cdf-d1e2-40e6-bec8-770828f4776d)
