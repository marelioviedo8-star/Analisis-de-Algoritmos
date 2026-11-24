# Fundamentos matemáticos y conceptuales

Guía inicial de la unidad.

## Complejidad, corrección y casos de entrada

Para analizar un algoritmo se define el tamaño de entrada n, se fija una operación básica y se cuenta cuántas veces se ejecuta. El espacio auxiliar es la memoria adicional a la entrada.

- O(g(n)) expresa una cota superior asintótica.
- Ω(g(n)) expresa una cota inferior asintótica.
- Θ(g(n)) expresa una cota ajustada.

En una búsqueda lineal, encontrar el objetivo al principio requiere una comparación. Si no aparece o aparece por primera vez al final, se hacen n comparaciones. El invariante es que el objetivo no aparece en las posiciones ya revisadas.

## Sumatorias y recurrencias

- Revisar todos los pares distintos cuesta 0 + 1 + … + (n − 1) = n(n − 1)/2 operaciones, es decir, Θ(n²).
- La búsqueda binaria requiere datos ordenados. En el peor caso, T(n) = T(⌊n/2⌋) + Θ(1) con T(0) = Θ(1). Hay Θ(log n) niveles para n ≥ 2.

## Ejercicio

Cuenta las comparaciones para encontrar el valor 7 en [1, 3, 5, 7, 9] usando ambas búsquedas. La búsqueda lineal hace cuatro comparaciones con elementos y la binaria hace dos si revisa primero el punto medio y luego el punto medio inferior del intervalo restante.
