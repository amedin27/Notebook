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