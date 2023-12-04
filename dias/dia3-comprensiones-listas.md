# Compresiones de listas
## Día 3

Un tip valioso para programar mejor en Python es hacer uso eficiente de las **comprensiones de lista (list comprehensions)**. Las comprensiones de lista son una forma concisa y legible de crear listas, aprovechando la sintaxis de Python para expresar la creación de listas a partir de otros iterables de una manera más clara y eficiente que usar bucles tradicionales.

Las comprensiones de lista no solo mejoran la legibilidad del código, sino que también son generalmente más rápidas porque están optimizadas internamente en Python. Además, reducen la cantidad de líneas de código necesarias para realizar una tarea, lo que ayuda a mantener tu código limpio y mantenible.


Creamos una lista en la que nos devuelva todos los cuadrados de los números de 0 al 9.
Es decir, 0\*0=0, 1\*1=1, 2*2=4...
```Python
cuadrados_for = []
for i in range(10):
    cuadrados_for.append(i ** 2)
```

Si imprimimos la lista el resultado es: ```[0, 1, 4, 9, 16, 25, 36, 49, 64, 81]```
```Python
print(cuadrados_for)
```

Podemos lograr exactamente el mismo resultado con una sola linea de código
```Python
cuadrados_comprension = [i ** 2 for i in range(10)]
```

Ahora como puedes ver la operación ```i ** 2``` se coloca primero, y la definición del ciclo for ```for i in range(10)``` después. Todo dentro de corchetes ```[]``` para indicarle a Python que el resultado se colocará en una lista

Si imprimimos la nueva lista el resultado es el mismo: ```[0, 1, 4, 9, 16, 25, 36, 49, 64, 81]```
```Python
print(cuadrados_comprension)
```

**De hecho hay un TikTok que lo explica**
[➡️DALE CLIC AQUÍ PARA VERLO⬅️]()

| [⬅️ Día 2 ](/dias/dia2-lista_recursiva.md) | Con 💖 por [@brujeriatech](https://www.instagram.com/brujeriatech/) | [Día 4 ➡️](/dias/dia4-itertools.md)|
|:------------- |:---------------:| -------------:|
