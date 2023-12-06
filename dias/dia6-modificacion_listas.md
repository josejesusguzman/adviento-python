# Error común al usar los scopes
## Día 6

Un error común entre los programadores de Python, especialmente los principiantes, es el "error de la variable ```global``` y ```local``` con el mismo nombre". Esto ocurre cuando una variable ```global``` y una variable ```local``` dentro de una función tienen el mismo nombre, lo que puede llevar a comportamientos confusos y errores difíciles de rastrear.

**Python trata las variables definidas dentro de una función como locales**, a menos que se especifique explícitamente lo contrario. Si una variable dentro de una función tiene el mismo nombre que una variable ```global```, la variable ```local``` ocultará a la global dentro del ámbito de la función. Esto puede causar errores si la función intenta modificar la variable global sin declararla como tal.

**[➡️ AQUÍ PUEDES VER EL CÓDIGO FUNCIONANDO ⬅️](/notebooks/dia6-modificacion_listas.ipynb)** 

```Python

# Lista original con algunos números
numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9]

# MÉTODO INCORRECTO: Modificar la lista mientras se itera
for numero in numeros:
    if numero % 2 != 0:
        numeros.remove(numero)

# Lista después de intentar eliminar números impares (MÉTODO INCORRECTO)
resultado_incorrecto = numeros

# Restablecemos la lista a su estado original
numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9]

# MÉTODO CORRECTO: Iterar sobre una copia de la lista
for numero in numeros[:]:  # Usando [:] podemos crear una copia para ser usada con el for
    if numero % 2 != 0:
        numeros.remove(numero)

# Lista después de eliminar números impares (MÉTODO CORRECTO)
resultado_correcto = numeros

print(resultado_incorrecto, resultado_correcto)

```

### Método Incorrecto (Sin usar global):

- En la función ```incrementar_incorrecto()```, intentamos incrementar la variable global contador sin declararla como global
- Esto resulta en un error: ```local variable 'contador' referenced before assignment```. Este error ocurre porque Python asume que contador en la función es una variable local, dado que estamos intentando asignarle un valor. Como aún no está asignada en el ámbito local, se produce un error.


### Método Correcto (Usando global):

- En la función ```incrementar_correcto()```, declaramos contador como una variable global antes de modificarla.
  
- Al hacer esto, le decimos a Python que use la variable global contador en lugar de crear una nueva variable local con el mismo nombre.
- La función incrementa correctamente el valor de la variable global contador, y el ```resultado_correcto``` es 1.


**De hecho hay un TikTok que lo explica**
[➡️DALE CLIC AQUÍ PARA VERLO⬅️]()

| [⬅️ Día 5 ](/dias/dia5-enumerate.md) | Con 💖 por [@brujeriatech](https://www.instagram.com/brujeriatech/) | [Día 7 ➡️]()|
|:------------- |:---------------:| -------------:|

