
# Interning
## Día 1

Para mejorar la eficiencia y la gestión de memoria, Python preasigna ciertos objetos inmutables como pequeñas cadenas de caracteres y números enteros dentro de un rango específico. 
Esto significa que cada vez que creas una variable con el mismo valor pequeño (por ejemplo, un entero entre -5 y 256), Python en realidad no crea un nuevo objeto, sino que referencia al objeto ya existente. 

Este comportamiento es especialmente notable con las cadenas y los enteros, donde múltiples referencias pueden apuntar al mismo objeto en memoria si sus valores son idénticos y están dentro del rango predefinido.

**[➡️ AQUÍ PUEDES VER EL CÓDIGO FUNCIONANDO ⬅️](/notebooks/dia1-interning.ipynb)** 


Enteros
```Python
a = 256
b = 256
```

Cadenas
```Python
s1 = "Hola"
s2 = "Hola"
```

Se comprueba si las variables referencian al mismo objeto en memoria

```Python
internado_enteros = a is b
internado_cadenas = s1 is s2
```

Ambos resultados son True porque se cumple con el interning

```Python
print(internado_enteros, internado_cadenas)
```

**De hecho hay un TikTok que lo explica**
[➡️DALE CLIC AQUÍ PARA VERLO⬅️](https://vm.tiktok.com/ZM68gCCFV/)

| [⬅️ Ir al inicio ](/README.md) | Con 💖 por [@brujeriatech](https://www.instagram.com/brujeriatech/) | [Día 2 ➡️](/dias/dia2-lista_recursiva.md)|
|:------------- |:---------------:| -------------:|
