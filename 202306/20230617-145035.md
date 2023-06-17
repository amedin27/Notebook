# 1. Introducción al ecosistema de la programación
##1.1 ¿Qué es un lenguaje de programación?
Son una serie de reglas gramaticales bien definidas que permiten al programador escribir una serie de instrucciones (algoritmos) y nos permiten controlar un sistema. 

##1.2 Tipos de paradigmas de programación

- **Imperativos**: Son una serie de instrucciones que van definiendo paso a paso lo que va haciendo un sistemas. Por ejemplo, una receta de cocina es imperativo.  
- **Declarativos**: Se centra en cual va a ser el resultado final. Se centra en el qué, en lugar del cómo. Por ejemplo, la foto final del pato o el plato terminado de la receta anterior. 

*Dumb example: Javascript Example*

```JS
const programmerList =["Santiago", "Pedro", "Ana", "Alejandra"];

let names  = []

//Programación imperativa
programmerList.forEach((programmer, position) => {
names[postion] = programmer
})

//Programación declarativa
names = [...programmerList]
```

### Paradigma Imperativo vs Declarativo: 

|                      | Legibilidad | Curva de aprendizaje | Escalabilidad del código  |
| :---:               | :---:             | :---:                             | :---:                                  |
| Imperativo    | 👍               |👍                               |                                         |
| Declarativo   |                     |                                  |           👍                            |

##1.3 División por niveles de los lenguajes de programación
Los lenguajes de programación se pueden clasificar por niveles, dependiendo de  la especificidad que tiene cada uno. Cuanto más bajo sea el nivel, más características específicas vamos a poder tocar a nivel hardware, es decir, dentro del ordenador. Por eso tenemos una división por niveles que es la siguiente: 

1. **Lenguaje máquina** :Es el lenguaje de programación de nivel más bajo que un ordenador puede entender. Es un conjunto de instrucciones binarias (1 y 0), que representan operaciones muy básicas que pueden ser ejecutadas por la unidad de procesamiento central (CPU) de un ordenador. Cada combinación de ceros y unos representa una acción específica que puede hacer, como sumar dos números o guardar información en la memoria.

2. **Lenguaje ensamblador**: Como el lenguaje máquina es casi imposible de entender por lo humanos se necesitó crear una especie de puente o de "traductor". El lenguaje ensamblador es una abstracción de cosas muy específicas que nosotros podemos llegar a entender. Estos dos lenguajes son conocidos como lenguajes de **bajo nivel** porque están relacionados directamente con el comportamiento del hardware y la arquitectura del propio sistema que estemos utilizando, el procesador o la memoria. 

3. **Lenguajes de medio -bajo nivel**: Los más conocidos son C y C++, tienen acceso a la memoria del procesador. Son lenguajes modernos pero pueden relacionarse con con el propio sistema. 

4. **Lenguajes de medio -alto nivel**: Java, Javascript, PHP. 

5. **Lenguajes de alto nivel**: Están basados en lenguajes de medio nivel (frameworks: es decir una serie de funcionalidades extras que se han añadido a los programas que ya conocemos en base a librerías para que programar con estos lenguajes sea, incluso más fácil). 

##1.4 Proceso de conversión
Como hemos visto en el punto anterior, los ordenadores solo entienden 1 y 0, por lo tanto, cuando nosotros programamos con cualquier lenguaje de programación lo que necesitamos es un "traductor", algo que nos ayude a transformar nuestras líneas de código en algo que sea legible por el ordenador. 

Existen dos formas para hacer esta traducción: 

- **Los compiladores**: Son un programita que se ejecuta por detrás y que lo que hace es traducir nuestro lenguaje a código máquina. Si durante esta compilación existiera algún error el código no llega a ejecutarse. Se para. 

- **Los intérpretes**:  A diferencia del compilador se interpreta en tiempo real. Si existiera algún error no se para. Sale el error normalmente por pantalla. 


##1.5 IDEs (Entorno de desarrollo integrado)
###1.5.1 ¿Qué es un IDEs (Entorno de desarrollo integrado)?
Un IDE (Entorno de Desarrollo Integrado, por sus siglas en inglés) es como el bloc de notas básico pero con "esteroides" con muchas más características que este bloc de notas. Un IDE proporciona un conjunto completo de características y funcionalidades para facilitar el desarrollo de software. Un IDE es un programita que combina un editor de texto, un compilador o intérprete (dependiendo del lenguaje que estemos utilizando), y otras herramientas útiles en una interfaz gráfica.

Existen varios IDEs pero el más utilizado hoy en día es el [VSC ( Visual Studio Code)](https://code.visualstudio.com/) o [Atom](https://atom.en.softonic.com/) es otro de los IDEs más utilizados. 

##1.6 Control de versiones
El control de versiones es un sistema que registra y administra los cambios realizados en los archivos de un proyecto a lo largo del tiempo. Su objetivo principal es mantener un historial de las modificaciones, permitiendo rastrear quién hizo qué cambios, cuándo se hicieron y facilitando la colaboración entre múltiples personas en un proyecto de desarrollo de software u otras formas de trabajo colaborativo. 

Si nosotros como programadores, no utilizáramos a la hora de trabajar un sistema de control de versiones sería un auténtico CAOS. Imagina que tenemos un archivo, lo modificamos y ahora nuestro programa deja de funcionar, sin un sistema de control de versiones no podríamos ir a la versión anterior.  

Una de las opciones que podríamos adoptar sería hacer una copia del archivo y renombrarla como versión 1 pero esto es un poco tedioso porque al final tenemos copias de copias... 

Otra de las opciones que podríamos adoptar sería trabajar con Dropbox  o algún sistema similar en la nube como Google Drive. El problema que tenemos con esto, es que estamos trabajando dentro de un equipo de desarrollo, si yo hago un cambio y mi compañero hace un cambio de manera simultánea solo se va a guardar la última versión del documento.

Por eso a principios de los 2000 se creó [Git](https://git-scm.com/). Aunque no fue el primero. 
- **CVS (Concurrent Version System)** : Fue un sistema para ayudar a los equipos que surgió para ayudar a lidiar con estos problemas. 
- **SVN (Subversión)**: Parecido a CVS pero con alguna serie de mejoras. 
- **Git** : Hoy en día es el sistema que se está utilizando por todo el mundo. Existen dos plataformas que utilizan el sistema de [Git](https://git-scm.com/) por detrás ([GitHub](https://github.com/) y [GitLab](https://about.gitlab.com/free-trial/devsecops/?utm_medium=cpc&utm_source=bing&utm_campaign=brand_emea_pr_rsa_br_exact&utm_content=%2Ffree-trial%2Fdevsecops%2F&_bt&_bk=gitlab&_bm=e&_bn=o&_bg=1328211696466798&msclkid=c69504a17ae91ea172c7602cb930c82a%2F)) . GitHub y GitLab son muy parecidos la única diferencia es que GitLab se centra más en repositorios privados y GitHub se centra más en repositorios públicos. 











