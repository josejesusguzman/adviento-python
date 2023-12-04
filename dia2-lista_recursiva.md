# Lista recursiva
## Día 2

Una curiosidad poco conocida sobre las listas en Python es su capacidad para contener referencias a sí mismas, lo que se conoce como una **lista recursiva**. Esto significa que una lista puede contener una referencia a sí misma como uno de sus elementos. Esto se debe a que las listas en Python son objetos dinámicos y pueden almacenar cualquier tipo de dato, incluidas referencias a otros objetos, incluso a ellas mismas.

Primero definimos una lista
```Python
lista_recursiva = [1, 2, 3]
```

Después con la función append podemos agregar al final de la lista a la misma lista
```Python
lista_recursiva.append(lista_recursiva)
```

Si la imprimimos, el resultado es una lista con cuatro elementos siendo el cuarto una referencia a la misma lista
Python no vielve a almacenar la lista sino la referencia de memoria de la lista.

```Python
print(lista_recursiva)
```

Si imprimimos el cuarto elemento de la lista nos daremos cuenta que el resultado es el mismo ya que estamos desplegandola desde su referencia de memoria.
```Python
print(lista_recursiva[3])
```

**De hecho hay un TikTok que lo explica**
[➡️DALE CLIC AQUÍ PARA VERLO⬅️]()

| [⬅️ Día 1 ](/dia1-interning.md) | Con 💖 por [@brujeriatech](https://www.instagram.com/brujeriatech/) | [Día 3 ➡️](/dia3-comprensiones-listas.md)|
|:------------- |:---------------:| -------------:|
