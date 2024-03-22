

# Introducción a Python

## Semana 12
<!-- .element style="text-align:center" -->

![alt text](./img/logo2.png) <!-- .element style="margin-left: auto; margin-right: auto; display: block" -->

---

# Listas

Se pueden crear de tres formas:
- Literales de listas
- `list()` con un iterable
- List comprehensions
- Métodos de listas: https://www.w3schools.com/python/python_ref_list.asp

---

# Operaciones comunes en secuencias

No hay que sabérselas, pero hay que saber que están.

Valen para listas, cadenas, tuplas:

- `x in s`
- `x not in s`
- `s + t`
- `s * n`
- `s[i]`
- `s[i:j]`
- `s[i:j:k]`
- `len(s)`
- `min(s)`
- `max(s)`
- `s.index(x[, i[, j]])`
- `s.count(x)`
- `enumerate(x)`

Se admiten índices negativos, empiezan desde el final: `[1,2,3][-1] => 3`

Ejercicio: usando índices, obtén el culo de estas cadenas: "culombio", "pedúnculo", "suculosa"

---

# List comprehensions


  - `[expression(item) for item in iterable]`
  - `even_numbers = [num for num in range(1, 10) if num % 2 == 0]`
  - `multiplication = [[i * j for j in range(1, 6)] for i in range(2, 5)]`
  -
PONER EJEMPLOS:
- Simple
- If
- If/else
- doble for

---

# Ejercicios list comprehensions


```python
numeros = [1, 2, 3, 4, 5]
mayores_que_dos = []
for numero in numeros:
    if numero > 2:
        mayores_que_dos.append(i)
```
<details>
<summary>Solución</summary>
<pre class="code-wrapper"><code class="python">
mayores_que_dos = [ i if i > 2 for i in numeros]
</code></pre>
</details>


---


# Duplicar una lista
numeros = [1, 2, 3, 4, 5]
result = []

for i in numeros:
    result.append(i * 2)

[ i*2 for i in numeros]

# Obtener los mayores de dos
numeros = [1, 2, 3, 4, 5]
mayores_que_dos = []
for numero in numeros:
    if numero > 2:
        mayores_que_dos.append(i)

[ i for i in numeros if i > 2]

# Loop
transformed = []
for i in range(5):
    transformed.append(i * 2 if i % 2 == 0 else i)

# List comprehension
transformed = [i * 2 if i % 2 == 0 else i for i in range(5)]



# Loop
matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
flattened = []
for row in matrix:
    for item in row:
        flattened.append(item)

# List comprehension
flattened = [item for row in matrix for item in row]


---

# Ordenamiento pseudoalfabético

> He preparado un programa que ordena los números del 1 al 100 en orden alfabético
> es decir: primero los que empiezan por 1, luego por 2, etc. Los que empiezan
> por el mismo dígito los reordena por el dígito que viene a continuación. Así,
> los números quedarían: 1, 10, 100, 11, 12...

¿En qué números coincide el orden numérico con el alfabético?

---

# ¿Cómo de buena eres realmente?

Había un examen en tu clase y lo has aprobado. ¡Enhorabuena!

Pero eres una persona ambiciosa. Quieres saber si eres mejor que el alumno medio de tu clase.

Recibes las puntuaciones de los exámenes de tus compañeros. Ahora calcula la media y compara tu puntuación.
Devuelve `True` si eres mejor, si no, `False`.

<div></div> <!-- .element style="height: 200px" -->

[Enlace Kata](https://www.codewars.com/kata/5601409514fc93442500010b)



---

# Rangos


---

# Tuplas

https://realpython.com/python-tuple/
fixed and unchangeable series of values
puede contener múltiples tipos
cero index





---


# Diccionarios


