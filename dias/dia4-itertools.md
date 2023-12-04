# Itertools
## Día 4

**itertools** proporciona una serie de herramientas para la manipulación eficiente de iterables, que pueden hacer tu código más limpio, más rápido y más Pythonic.

Vamos a ver un ejemplo práctico utilizando **itertools**. Supongamos que quieres generar todas las combinaciones posibles de tres elementos a partir de una lista. Podrías hacer esto manualmente con bucles anidados, pero es más eficiente y legible utilizar **itertools**.combinations.

Primero tenemos que importar la biblioteca
```Python
import itertools
```

Declaramos una lista de elementos
```Python
elementos = ['a', 'b', 'c', 'd']
```

Generamos todas las combinaciones posibles de tres elementos.

```itertools.combinations()``` nos solicita 2 argumentos; un ```iterable``` que es la lista u objeto del cual generaremos las combinaciones y un valor ```r``` que es la longitud de elementos de las subsecuencias generadas.

En este ejemplo la función nos generará 4 tuplas con ```r=3``` elementos en cada una de ellas. 
```Python
combinaciones = list(itertools.combinations(elementos, 3))
```
El resultado es: ```[('a', 'b', 'c'), ('a', 'b', 'd'), ('a', 'c', 'd'), ('b', 'c', 'd')]```
```Python
print(combinaciones)
```

**De hecho hay un TikTok que lo explica**
[➡️DALE CLIC AQUÍ PARA VERLO⬅️]()

| [⬅️ Día 3 ](/dias/dia3-comprensiones-listas.md) | Con 💖 por [@brujeriatech](https://www.instagram.com/brujeriatech/) | [Día 5 ➡️]()|
|:------------- |:---------------:| -------------:|
