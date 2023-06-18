# 3- Paradigmas de la programación
Existen tres tipos de "formas de programar": 

## 3.1- Programación esctructurada
Es una programación en la que nosotros le damos al programa una serie de instruciones para que vaya ejecutando poco a poco de forma estructurada. 
Este enfoque ha sido ampliamente adoptado en numerosos lenguajes de programación, como C, Pascal y Python. Además, sentó las bases para el desarrollo de otros paradigmas de programación, como la programación orientada a objetos.

Ejemplo de programación estructurada en Phyton:

```python
def calcular_suma(n):
    suma = 0
    for i in range(1, n+1):
        suma += i
    return suma

def main():
    num = int(input("Ingrese un número: "))
    resultado = calcular_suma(num)
    print("La suma de los primeros", num, "números es:", resultado)

main()

```

## 3.2- Programación orientada a objetos
La programación orientada a objetos al contrario de ser por secuencias lo más importante son los "Objetos". 

La programación orientada a objetos (POO) es un paradigma de programación que se basa en la organización del código en torno a objetos, los cuales son entidades que representan elementos del mundo real y tienen propiedades (atributos) y comportamientos (métodos). La POO se centra en el concepto de encapsulación, abstracción, herencia y polimorfismo.

En la programación orientada a objetos, se crean clases, que son plantillas o moldes para crear objetos. Una clase define las características y comportamientos comunes que tendrán los objetos que se creen a partir de ella. Los objetos son instancias específicas de una clase, que pueden interactuar entre sí a través de métodos y propiedades.

Aquí tienes un ejemplo en Markdown que muestra una clase Persona en Python:

```python
class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad

    def saludar(self):
        print("Hola, mi nombre es", self.nombre)

    def cumpleaños(self):
        self.edad += 1
        print("¡Feliz cumpleaños! Ahora tengo", self.edad, "años.")

# Crear objetos de la clase Persona
persona1 000000000000= Persona("Juan", 25)
persona2 = Persona("María", 30)

# Acceder a los atributos y métodos de los objetos
print(persona1.nombre)  # Salida: Juan
persona2.saludar()  # Salida: Hola, mi nombre es María
persona1.cumpleaños()  # Salida: ¡Feliz cumpleaños! Ahora tengo 26 años.
```

Lo especial de este tipo de programación es que los objetos se vayan relacionando entre sí. 

### 3.2.1- ¿Qué son los objetos?
Lo más importante de los objetos es que tienen dos tipos de propiedades: 
- Por un lado los datos (**atributos**): 
  Los atributos en la programación orientada a objetos son variables asociadas a una clase o a una instancia de esa clase. Representan las características o propiedades de un objeto. Cada objeto tiene su propio conjunto de valores para sus atributos.

Aquí tienes un ejemplo en Markdown que muestra una clase Persona con atributos en Python:
```python
class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad

    def presentarse(self):
        print("Hola, soy", self.nombre, "y tengo", self.edad, "años.")

# Crear objetos de la clase Persona
persona1 = Persona("Juan", 25)
persona2 = Persona("María", 30)

# Acceder a los atributos de los objetos
print(persona1.nombre)  # Salida: Juan
print(persona2.edad)  # Salida: 30

# Llamar al método que utiliza los atributos
persona1.presentarse()  # Salida: Hola, soy Juan y tengo 25 años.

```

En este ejemplo, la clase `Persona` define dos atributos (`nombre` y `edad`) y dos métodos (`saludar()` y `cumpleaños()`). Los objetos `persona1` y `persona2` son instancias de la clase `Persona` y tienen sus propios valores de atributos.


- Por otro lado tenemos las funciones o la funcionalidad (**métodos**):Los métodos en la programación orientada a objetos son funciones asociadas a una clase o a una instancia de esa clase. Representan los comportamientos o acciones que un objeto puede realizar. Los métodos pueden acceder y manipular los atributos de un objeto, así como realizar otras operaciones relevantes para ese objeto.

Aquí tienes un ejemplo en Markdown que muestra una clase Persona con métodos en Python:

```python
class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad

    def presentarse(self):
        print("Hola, soy", self.nombre, "y tengo", self.edad, "años.")

    def cumplir_anio(self):
        self.edad += 1
        print("¡Feliz cumpleaños! Ahora tengo", self.edad, "años.")

# Crear objetos de la clase Persona
persona1 = Persona("Juan", 25)
persona2 = Persona("María", 30)

# Llamar a los métodos de los objetos
persona1.presentarse()  # Salida: Hola, soy Juan y tengo 25 años.
persona2.cumplir_anio()  # Salida: ¡Feliz cumpleaños! Ahora tengo 31 años.
```

En este ejemplo, la clase `Persona` tiene dos métodos: `presentarse()` y `cumplir_anio()`. El método `presentarse()` muestra un mensaje con el nombre y la edad de la persona. El método `cumplir_anio()` incrementa la edad de la persona en uno y muestra un mensaje de feliz cumpleaños.

Los métodos son llamados utilizando la notación de punto (`.`) después del nombre del objeto, seguido del nombre del método y los paréntesis. Por ejemplo, `persona1.presentarse()` llama al método `presentarse()` en el objeto `persona1`.


- Las clases: En programación orientada a objetos, una clase es un concepto que define la estructura y el comportamiento de un tipo de objeto. Se puede considerar como una plantilla o un molde para crear objetos.

Las clases encapsulan atributos y métodos. Los atributos son variables que representan las características o propiedades del objeto, mientras que los métodos son funciones que definen el comportamiento y las acciones que el objeto puede realizar.

Las clases definen los atributos y métodos que serán comunes a todos los objetos creados a partir de ellas. Cada objeto individual creado a partir de una clase se conoce como una instancia de esa clase. Cada instancia tiene sus propios valores de atributos y puede llamar a los métodos definidos en la clase.

Cuando se crea un objeto (una instancia de una clase), este objeto tiene acceso a los atributos y métodos definidos en la clase. Los objetos pueden acceder y manipular sus propios atributos, y pueden llamar a los métodos definidos en la clase para realizar ciertas acciones.

## 3.3- Programación funcional
Se basa en la utilización de lo que se conoce como "funciones puras". 
Una función pura es una función en programación que produce el mismo resultado para los mismos valores de entrada y no tiene efectos secundarios observables fuera de la función. Es decir, su resultado depende únicamente de sus argumentos y no modifica ni depende de ningún estado externo.

```JS
function sumna (num1, num2){
    total = num1 + num2;
    return total
}

console.log(suma(3,8)) //11
console.log(suma(3,8)) //11

```

Otra de las características de la programación funcional son las funciones sin estado. Es decir que no tengan variables internas. Para ello se utiliza algo que se llama recursividad. Es decir que una función se llame a si misma. 

Aquí tienes un ejemplo de recursividad en Javascript:

```javascript
/**
 * Función para calcular el factorial de un número de forma recursiva.
 * @param {number} n - El número para calcular su factorial.
 * @returns {number} - El factorial del número.
 */
function factorial(n) {
  if (n === 0 || n === 1) {
    return 1;
  } else {
    return n * factorial(n - 1);
  }
}

// Calcular el factorial de 5
const resultado = factorial(5);
console.log(resultado);  // Salida: 120
```
En este ejemplo, se define la función `factorial()` que calcula el factorial de un número utilizando recursividad. Si el número es 0 o 1, la función devuelve 1. De lo contrario, multiplica el número por el factorial del número anterior.

Luego, se llama a la función `factorial(5)` para calcular el factorial de 5 y se guarda el resultado en la variable `resultado`. Finalmente, se imprime el resultado en la consola.

El ejemplo que hemos puesto arriba calcula el factorial pero no de forma recursiva. Vamos a ver un ejemplo ahora de forma recursiva. 

```javascript
/**
 * Función recursiva para calcular el factorial de un número.
 * @param {number} n - El número para calcular su factorial.
 * @returns {number} - El factorial del número.
 */
function factorial(n) {
  if (n === 0 || n === 1) {
    return 1;
  } else {
    return n * factorial(n - 1);
  }
}

// Calcular el factorial de 5
const resultado = factorial(5);
console.log(resultado);  // Salida: 120
```

En este ejemplo, la función `factorial()` se define de manera recursiva. Si el número `n` es 0 o 1, la función devuelve 1. En caso contrario, se llama a la función `factorial()` nuevamente con el argumento `n - 1` y se multiplica por `n`. Esta llamada recursiva continúa hasta que se alcanza el caso base, donde el resultado final se calcula multiplicando todos los números desde `n` hasta 1.

Luego, se llama a la función `factorial(5)` para calcular el factorial de 5 y se guarda el resultado en la variable `resultado`. Finalmente, se imprime el resultado en la consola.

