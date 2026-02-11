# Notas de Cuadernos Python

### Materia: Procesamiento de Datos

#### Nombre: Juan Diego Muñoz Angulo

#### ID de Estudiante: 00020529185

#### Fecha: 10 de febrero de 2026

#### Profesor: John Jairo Corredor

En este archivo se resume de forma sencilla y práctica todo lo aprendido en los cuadernos de ejercicios de Python. Cada sección contiene ejemplos y explicaciones para recordar los conceptos clave.

---

## 01 - Operaciones con Cadenas

Aprendimos qué es una cadena en Python, cómo se define y cómo se manipula. Vimos indexación, slicing, stride, concatenación, secuencias de escape y métodos como upper, replace y find.
Las cadenas nos permiten trabajar con texto, extraer partes, buscar palabras y modificar información.
Por ejemplo, podemos acceder a letras, unir frases, buscar palabras o cambiar mayúsculas.
Esto nos ayuda a trabajar con textos, extraer información, limpiar datos y preparar información para análisis o procesamiento.


```python
cadena = "Python es chimba"  # Creamos una cadena de texto
print(cadena[0])              # Imprime el primer carácter
print(cadena[-1])             # Imprime el último carácter
print(cadena[0:6])            # Imprime los primeros 6 caracteres
print(cadena[::2])            # Imprime un carácter sí y uno no (stride 2)
print(cadena + " y re fácil") # Concatena y muestra otra frase
print(cadena.upper())         # Convierte la cadena a mayúsculas
print(cadena.replace("chimba", "fácil")) # Reemplaza una palabra
print(cadena.find("es"))     # Busca la posición de 'es'
print("Linea1\nLinea2")      # Imprime dos líneas usando salto de línea
print("Columna1\tColumna2")  # Imprime dos columnas usando tabulación
```

---

## 02 - Tuplas

Aprendimos que las tuplas son estructuras de datos inmutables, útiles para almacenar colecciones de elementos que no deben cambiar.
Nos permite guardar datos fijos, como coordenadas o registros, y asegurar que no se modifiquen accidentalmente.


```python
tupla = (10, 20, 30)      # Creamos una tupla con tres números
print(tupla[1])            # Imprime el segundo elemento
print(len(tupla))          # Imprime la cantidad de elementos
x, y, z = tupla            # Desempaqueta la tupla en variables
print(x, y, z)             # Imprime los valores desempaquetados
```

---

## 03 - Listas

Aprendimos a usar listas, que son colecciones de elementos que pueden cambiar. Las listas permiten agregar, eliminar y modificar elementos.
Las listas se usan para manejar datos que cambian, como resultados, registros o cualquier información que pueda crecer o cambiar.
Podemos recorrerlas, modificarlas y ordenarlas.
Esto nos ayuda a manejar datos dinámicos, como resultados, registros o cualquier información que pueda crecer o cambiar.


```python
lista = [10, 20, 30]      # Creamos una lista con tres números
print(lista[1])            # Imprime el segundo elemento
lista.append(40)           # Agrega el número 40 al final
print(lista)               # Imprime la lista actualizada
lista[0] = 5               # Cambia el primer elemento a 5
print(lista)               # Imprime la lista modificada
lista.remove(20)           # Elimina el número 20 de la lista
print(lista)               # Imprime la lista sin el 20
for elemento in lista:     # Recorre cada elemento de la lista
	print(elemento)        # Imprime cada elemento
```

---

## 04 - Conjuntos

Aprendimos que los conjuntos permiten almacenar elementos únicos y realizar operaciones como unión, intersección y diferencia.
Los conjuntos nos ayudan a eliminar duplicados y comparar grupos de datos. Podemos unir conjuntos, encontrar elementos comunes o ver diferencias.
Esto nos ayuda a eliminar duplicados y comparar grupos de datos, útil para análisis y filtrado.


```python
conjunto1 = {1, 2, 3}         # Creamos un conjunto con tres números
conjunto2 = {3, 4, 5}         # Otro conjunto con otros números
print(conjunto1 | conjunto2)  # Unión de ambos conjuntos
print(conjunto1 & conjunto2)  # Intersección (elementos en común)
print(conjunto1 - conjunto2)  # Diferencia (elementos solo en conjunto1)
conjunto1.add(6)              # Agrega el número 6 al conjunto1
print(conjunto1)              # Imprime el conjunto actualizado
```

---

## 05 - Diccionarios

Aprendimos a usar diccionarios para guardar pares clave-valor. Son útiles para organizar datos y acceder rápidamente a información específica.
Los diccionarios nos permiten buscar datos por clave, modificar valores y recorrer información estructurada.
Esto nos permite estructurar datos como registros, configuraciones o cualquier información asociada a una clave.


```python
diccionario = {"nombre": "Juan", "edad": 30}  # Creamos un diccionario
print(diccionario["nombre"])                      # Imprime el valor de la clave 'nombre'
diccionario["edad"] = 31                          # Cambia el valor de 'edad'
print(diccionario)                                 # Imprime el diccionario actualizado
del diccionario["nombre"]                         # Elimina la clave 'nombre'
print(diccionario)                                 # Imprime el diccionario sin 'nombre'
for clave in diccionario:                          # Recorre cada clave
	print(clave, diccionario[clave])               # Imprime clave y valor
```

---

## 06 - Condiciones

Aprendimos a usar condicionales (if, else, elif) para tomar decisiones en el código según valores o situaciones.
Las condiciones nos permiten ejecutar acciones diferentes según los datos o situaciones. Podemos comparar valores y decidir qué hacer.
Esto nos ayuda a controlar el flujo del programa y responder a diferentes escenarios o datos.


```python
x = 7                       # Asigna el valor 7 a x
if x > 10:                  # Si x es mayor a 10
	print("Mayor a 10")     # Imprime si es mayor a 10
elif x == 7:                # Si x es igual a 7
	print("Es 7")           # Imprime si es 7
else:                       # Si no se cumple lo anterior
	print("Otro valor")     # Imprime otro valor
```

---

## 07 - Bucles

Aprendimos a usar bucles (for, while) para repetir acciones o recorrer colecciones de datos.
Los bucles nos permiten automatizar tareas, procesar grandes cantidades de datos y realizar operaciones repetitivas de forma eficiente.
Podemos recorrer listas, repetir instrucciones y controlar cuántas veces se ejecuta algo.
Esto nos permite automatizar tareas, procesar grandes cantidades de datos y realizar operaciones repetitivas de forma eficiente.


```python
for i in range(5):         # Repite 5 veces
	print(i)               # Imprime el valor de i (0 a 4)
lista = ["a", "b", "c"]     # Crea una lista de letras
for elemento in lista:     # Recorre cada elemento de la lista
	print(elemento)        # Imprime cada letra
n = 0                      # Inicializa n en 0
while n < 3:               # Mientras n sea menor que 3
	print(n)               # Imprime el valor de n
	n += 1                 # Suma 1 a n
```

---

## 08 - Funciones

Aprendimos a definir funciones para organizar el código, reutilizar lógica y dividir tareas en bloques independientes.
Las funciones nos ayudan a escribir código más limpio, modular y fácil de mantener. Podemos definir tareas, reutilizarlas y evitar repeticiones.
Esto nos ayuda a escribir código más limpio, modular y fácil de mantener, además de evitar repeticiones.


```python
# La función sumar recibe dos números y retorna su suma
def sumar(a, b):
	return a + b           # Retorna la suma de a y b
print(sumar(3, 5))         # Llama a sumar con 3 y 5, imprime el resultado
# La función saludar no recibe argumentos y solo imprime un saludo
def saludar():
	print("Hola mundo")    # Imprime un saludo
saludar()                  # Llama a la función saludar
```

---

## 09 - Clases y Objetos

Aprendimos qué es una clase, cómo crear objetos, atributos y métodos. Vimos ejemplos con círculos y rectángulos.
Las clases nos permiten modelar problemas complejos, organizar datos y comportamientos, y aprovechar la programación orientada a objetos para proyectos grandes.
Podemos crear nuestros propios tipos de datos, definir cómo se comportan y reutilizar código.
Esto nos permite modelar problemas complejos, organizar datos y comportamientos, y aprovechar la programación orientada a objetos para proyectos grandes.


```python
class Animal:                          # Definimos una clase Animal
	def __init__(self, nombre):        # Método constructor, recibe el nombre
		self.nombre = nombre           # Guarda el nombre en el objeto
	def hablar(self):                  # Método que retorna un saludo
		return "Hola, soy " + self.nombre
perro = Animal("Firulais")            # Creamos un objeto Animal llamado Firulais
print(perro.hablar())                  # Llama al método hablar e imprime el saludo
```
