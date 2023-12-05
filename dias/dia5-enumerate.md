# La función enumerate
## Día 5

Un tip valioso para mejorar la programación en Python con las bibliotecas estándar y la sintaxis estándar es utilizar la función ```enumerate()``` en bucles ```for```. Esta función agrega un contador a un iterable y devuelve este contador junto con el valor del iterable. Es especialmente útil cuando necesitas tanto el índice como el valor de los elementos en un iterable, como una lista.

Usar ```enumerate()``` en lugar de manipular manualmente los índices del bucle no solo hace que el código sea más limpio y legible, sino que también reduce el riesgo de errores, como los que pueden ocurrir al actualizar manualmente los índices.

**[➡️ AQUÍ PUEDES VER EL CÓDIGO FUNCIONANDO ⬅️](/notebooks/dia5-enumerate.ipynb)** 


```Python
# Definimos una lista de elementos
frutas = ["manzana", "platano", "cereza", "durazno"]
```

```Python
# Usamos enumerate en un bucle for
for indice, fruta in enumerate(frutas):
    print(f"Índice {indice}: {fruta}")
```

Este bucle for utiliza ```enumerate(frutas)```, que devuelve pares de índice y valor para cada elemento en la lista frutas. Dentro del bucle, indice es el índice actual y fruta es el valor. Esto te permite acceder fácilmente a ambos en cada iteración del bucle.

**De hecho hay un TikTok que lo explica**
[➡️DALE CLIC AQUÍ PARA VERLO⬅️]()

| [⬅️ Día 4 ](/dias/dia4-itertools.md) | Con 💖 por [@brujeriatech](https://www.instagram.com/brujeriatech/) | [Día 5 ➡️](/dias/dia5-enumerate.md)|
|:------------- |:---------------:| -------------:|

