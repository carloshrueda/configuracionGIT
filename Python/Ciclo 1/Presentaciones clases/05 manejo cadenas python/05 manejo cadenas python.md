---
theme: gaia
_class: lead
paginate: true
backgroundColor: #fff
backgroundImage: url('https://marp.app/assets/hero-background.svg')
marp: true
---

![bg left:100%](https://raw.githubusercontent.com/carloshrueda/carloshrueda/main/campus-trainer.png)

---

# **CADENAS PYTHON**

Podemos acceder a una caracter específico del string mediante su índice, pero no modificarlo.

---

## **len()**
Función len() permite conocer el largo de un string (número de caracteres). Así podemos recorrer un string de largo cualquiera.

---

## **Recorrer un string**
Para recorrer un string también podemos utilizar el comando for (que es una alternativa a usar whiles).

---

## **Operaciones con string**
Finalmente existen 4 operadores básicos para trabajar con strings.

---

## **Operaciones con string**


---

<style>
body {
margin-top: 50px;
}

h1 {
text-align: center;
font-size: 2em;
font-weight: bold;
}

h2 {
text-align: center;
}

</style>

![bg left:100% "Metodos de cadenas en Python"](https://techkrowd.com/wp-content/uploads/2020/05/cabecerapythonstr1.jpg)

---

<style>
p {
font-size: 1.5em;
}

.language-JavaScript {
font-size: 1.5em;
}

h2 {
    text-align: left;
    font-weight: bold;
    /*text-transform: capitalize;*/
}

p {
    margin-top: 5px;
    font-size: 1.3em;
}

</style>

# **MÉTODOS DE CADENAS**

El tipo de dato ```str``` es una clase incorporada cuyas instancias incluyen variados métodos para analizar, transformar, separar y unir el contenido de las cadenas de caracteres. 

En esta presentación detallamos los que consideramos más relevantes para tener siempre a mano.

---
<style>
.language-python {
    font-size: 1.1em;
    text-align: left;
    font-weight: bold;
    color:white;
}
h2 > strong {
    color:#00b225;
    font-size: 1.5em;
}
</style>

## **upper()**

Devuelve la cadena con todos sus caracteres a mayúscula:

```python
"Hola Mundo".upper()
``` 

```python
'HOLA MUNDO'
```

----

## **lower()**

Devuelve la cadena con todos sus caracteres a minúscula:

```python
"Hola Mundo".lower()
``` 

```python
'hola mundo'
``` 

----

## **capitalize()**

Devuelve la cadena con su primer carácter en mayúscula:

```python
"hola mundo".capitalize()
``` 

```python
'Hola mundo'
``` 

----

## **title()**

Devuelve la cadena con el primer carácter de cada palabra en mayúscula:

```python
"hola mundo".title()
``` 

```python
'Hola Mundo'
``` 

----

## **count()**

Devuelve una cuenta de las veces que aparece una subcadena en la cadena:

```python
"Hola mundo".count('mundo')
``` 

```python
1
``` 

----

## **find()**

Devuelve el índice en el que aparece la subcadena (-1 si no aparece):

```python
"Hola mundo".find('mundo')
``` 

```python
5
``` 
---

## **find()**

Devuelve el índice en el que aparece la subcadena (-1 si no aparece):

```python
"Hola mundo".find('mundoz')
``` 

```python
-1
``` 

----

## **rfind()**

Devuelve el índice en el que aparece la subcadena, empezando por el final:

```python
"Hola mundo mundo mundo".rfind('mundo')
``` 

```python
17
``` 

----

## **isdigit()**

Devuelve True si la cadena es todo números (False en caso contrario):

```python
c = "100"
c.isdigit()
``` 

```python
True
``` 

----

## **isalnum()**

Devuelve True si la cadena es todo números o carácteres alfabéticos:

```python
c = "ABC10034po"
c.isalnum()
``` 

```python
True
``` 

----

## **isalpha()**

Devuelve True si la cadena es todo carácteres alfabéticos:

```python
c = "ABC10034po"
c.isalpha()
``` 

```python
False
``` 
----

## **isalpha()**

Devuelve True si la cadena es todo carácteres alfabéticos:

```python
"Holamundo".isalpha()
``` 

```python
True
``` 

----

## **islower()**

Devuelve True si la cadena es todo minúsculas:

```python
"Hola mundo".islower()
``` 

```python
False
``` 

----

## **isupper()**

Devuelve True si la cadena es todo mayúsculas:

```python
"Hola mundo".isupper()
``` 

```python
False
``` 

----

## **istitle()**

Devuelve True si la primera letra de cada palabra es mayúscula:

```python
"Hola Mundo".istitle()
``` 

```python
True
``` 

----

## **isspace()**

Devuelve True si la cadena es todo espacios:

```python
"  -  ".isspace()
``` 

```python
False
``` 

----

## **startswith()**

Devuelve True si la cadena empieza con una subcadena:

```python
"Hola mundo".startswith("Mola")
``` 

```python
False
``` 

----

## **endswith()**

Devuelve True si la cadena acaba con una subcadena:

```python
"Hola mundo".endswith('mundo')
``` 

```python
True
``` 

----

## **split()**

Separa la cadena en subcadenas a partir de sus espacios y devuelve una lista:

```python
"Hola mundo mundo".split()[0]
``` 

 ```python
'Hola'
``` 

---
## **split()**

Podemos indicar el carácter a partir del que se separa:

```python
"Hola,mundo,mundo,otra,palabra".split(',')
``` 

```python
['Hola', 'mundo', 'mundo', 'otra', 'palabra']
``` 

----

## **join()**

Une todos los caracteres de una cadena utilizando un caracter de unión:

```python
",".join("Hola mundo")
``` 

```python
'H,o,l,a, ,m,u,n,d,o'
``` 

----

## **join()**

Une todos los caracteres de una cadena utilizando un caracter de unión:

```python
" ".join("Hola")
``` 

```python
'H o l a'
``` 

----

## **strip()**

Borra todos los espacios por delante y detrás de una cadena y la devuelve:

```python
"   Hola mundo     ".strip()
``` 

```python
'Hola mundo'
``` 

---

## **strip()**

Podemos indicar el carácter a borrar:

```python
"-----Hola mundo---".strip('-')
``` 

```python
'Hola mundo'
``` 

----

## **replace()**

Reemplaza una subcadena de una cadena por otra y la devuelve:

```python
"Hola mundo".replace('o','0')
``` 

```python
'H0la mund0'
``` 

---

## **replace()**

Podemos indicar un límite de veces a reemplazar:

```python
"Hola mundo mundo mundo mundo mundo".replace(' mundo','',4)
``` 

```python
'Hola mundo'
```

---
<style>
.ejercicios{
    font-size: 1.2em
}
</style>

## **Ejercicio 1**
<p class="ejercicios">Los teléfonos de una empresa tienen el siguiente formato prefijo-número-extension donde el prefijo es el código del país <b>+34</b>, y la extensión tiene dos dígitos (por ejemplo <b>+34-913724710-56</b>). Escribir un programa que pregunte por un número de teléfono con este formato y muestre por pantalla el número de teléfono sin el prefijo y la extensión.
</p>

---

## **Ejercicio 2**

<p class="ejercicios">
Hacer un programa que reciba una palabra e indicar si esta es un <b>palíndrome</b>.<br><br>
Una palabra <b>palíndroma</b> es aquella que se lee igual adelante que atrás.. 
</p>

---

## **Ejercicio 3**

<p class="ejercicios">
Escribir un programa que pregunte al usuario la fecha de su nacimiento en formato dd/mm/aaaa y muestra por pantalla, el día, el mes y el año. Adaptar el programa anterior para que también funcione cuando el día o el mes se introduzcan con un solo carácter.
</p>

---

## **Ejercicio 4**

<p class="ejercicios">
Descargar y resolver el desafio planteado en el documento PDF.
<br><br>
Debe crear un programa que resuelva el desafío, no una función por que el tema no se ha visto.
<br><br>
<span style="text-align: left;">
<a href="https://1drv.ms/b/s!AoVJjWr0lGHbgbsvqYy5kc3i83B6aA?e=KhFGWX">Para ver documento hacer clic aquí.
</span>
</a>
</p>

---

# **MÉTODOS CADENAS**

## **Referencias**

* [Operaciones comunes de cadena de caracteres _(sitio oficial python)_](https://docs.python.org/es/3/library/string.html)

* [30 Métodos de las cadenas](https://recursospython.com/guias-y-manuales/30-metodos-de-las-cadenas/)

---

![bg left:100%](https://raw.githubusercontent.com/carloshrueda/carloshrueda/main/campus-trainer.png)



