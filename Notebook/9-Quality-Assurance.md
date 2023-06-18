# 9- Quality Assurance (QA):
El Quality Assurance (QA), o aseguramiento de calidad, es un conjunto de actividades y procesos diseñados para garantizar que un producto o servicio cumpla con los estándares de calidad establecidos. El QA se enfoca en prevenir defectos y errores durante el desarrollo, implementación y mantenimiento de un producto, y en asegurar que cumpla con los requisitos y expectativas del cliente. Por decirlo de una forma sencilla es el "departamento de calidad del software". Es el que se asegura de que todo funciona y funciona bajo las necesidades que se plantearon. 

Las actividades de QA involucran la planificación, ejecución y evaluación de pruebas para detectar y corregir cualquier defecto o problema antes de que el producto se entregue a los usuarios finales. El objetivo principal del QA es garantizar que el producto o servicio sea confiable, funcione correctamente y cumpla con los estándares de calidad esperados.

Algunas de las actividades comunes en el QA incluyen:

Planificación de pruebas: Definir los objetivos y alcance de las pruebas, identificar los casos de prueba y establecer los criterios de aceptación.

Ejecución de pruebas: Realizar las pruebas de funcionalidad, rendimiento, seguridad, usabilidad y compatibilidad, entre otras, para identificar cualquier defecto o comportamiento no deseado.

Seguimiento y gestión de defectos: Registrar y rastrear los defectos encontrados durante las pruebas, y colaborar con los equipos de desarrollo para su resolución.

Mejora continua: Identificar oportunidades de mejora en los procesos y procedimientos, y proponer soluciones para evitar la aparición de futuros defectos.

El QA juega un papel fundamental en garantizar la satisfacción del cliente, la confiabilidad del producto y la reputación de la empresa. Al implementar prácticas de QA efectivas, se busca mejorar la calidad del producto o servicio y minimizar los riesgos asociados con su desarrollo y entrega.

El testing consiste en hacer una prueba y el propio software nos dice si ha pasado o no: 

Veamos un ejemplo: suma.test.js 

```JS
test("Prueba de suma", () =>{
    const a =1;
    const b= 2;
    const resultado =a + b;

    expect(resultado).toBe(3)
})

```

## 9.1- Test de cajas:
A continuación vamos a ver tres tipos de técnicas para testear
- Test de la caja negra: Consiste en tratar la app como una caja negra. Es decir, no sé lo que hay dentro. En este caso testeamos la entrada y la salida. Nosotros queremos que para un tipo de entrada haya un tipo de salida. 
- Test de la caja blanca: Consiste en ver lo que está ocurriendo por dentro. En este caso cuando le damos una entrada nos interesa ver los pasos que está haciendo esa entrada. Nos enfocamos en el camino que recorre la app, desde el punto de vista del código. El enfoque principal está en el comportamiento interno. 
- Test de la caja gris: Consiste en juntar los test de la caja negra y la caja blanca. En este caso tenemos una entrada que seguimos por dentro y testeamos además, cuál es la salida de este software. Es como una especie de técnica mixta entre las dos. 

## 9.2- Test funcionales y no funcionales:
- Test funcional: Lo que hace es testear todas las funcionalidades que se supone que nuestra app debe cumpilr. Además, debe testear los requerimientos del cliente pero también los errores.  
- Test no funcional: Se testea todo lo que hay alrededor. Por ejemplo los test de rendimiento o lo tiempos de carga de la app. El Stress test, la escalabilidad.... También debe de testearse la accesibilidad , la parte de UX y UI y test de seguridad.  


## 9.3- Modelos de testing:
- Modelo de testing en cascada o lineal (Waterfall): El modelo de testing en cascada es un enfoque de desarrollo de software en el que las actividades de testing se realizan secuencialmente, siguiendo el flujo de trabajo lineal del modelo en cascada. Este modelo se caracteriza por tener fases claramente definidas y secuenciales, donde cada fase se inicia después de que la fase anterior se haya completado. 
- Modelo de testing repetitivo o iterativo: Suele estar definidos por Sprints de 2 semanas.  El modelo de testing repetitivo o iterativo es un enfoque de desarrollo de software en el que las actividades de testing se realizan de manera iterativa y repetitiva a lo largo de todo el ciclo de vida del proyecto. A diferencia del modelo en cascada, que sigue una secuencia lineal de fases, el modelo iterativo permite la retroalimentación y la mejora continua a medida que se desarrolla y prueba el software.
- Modelo de testing en V: El modelo de testing en V es un enfoque de pruebas que se basa en el modelo de desarrollo en cascada y enfatiza la relación entre las actividades de desarrollo y de pruebas. El modelo toma su nombre de la forma en V que se forma al representar gráficamente las actividades de desarrollo y pruebas a medida que avanza el proceso de desarrollo de software.
- Modelo de testing en espiral:
El modelo de testing en espiral es un enfoque de desarrollo y testing de software que combina elementos del modelo en cascada y el modelo iterativo. Se basa en el concepto de iteraciones controladas y se enfoca en la gestión de riesgos a lo largo del ciclo de vida del proyecto.

El modelo de testing en espiral sigue un enfoque cíclico donde las actividades de desarrollo y testing se realizan en múltiples iteraciones, conocidas como espirales. Cada espiral representa un ciclo completo de desarrollo, que incluye la planificación, el análisis de riesgos, el desarrollo, el testing y la evaluación.