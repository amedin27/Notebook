# 12- Modelo Vista Controlador

El modelo Vista-Controlador (MVC, por sus siglas en inglés: Model-View-Controller) es un patrón de diseño de software más utilizado para el desarrollo de aplicaciones introducido en los años 70. Proporciona una forma de organizar y estructurar el código de una manera que facilite la separación de responsabilidades y la modularidad.

El modelo MVC se compone de tres componentes principales:

- Modelo (Model):Acceder y manipular los datos. Representa los datos y la lógica de negocio de la aplicación. El modelo se encarga de almacenar y manipular los datos, así como de realizar operaciones relacionadas con la lógica de negocio, como validaciones y cálculos.

- Vista (View):Mostrar los datos del modelo y proporcionar la interactividad al usuario. Es la interfaz de usuario o la representación visual de los datos. La vista es responsable de mostrar la información al usuario y de interactuar con él. Puede ser una página web, una ventana de aplicación o cualquier otro medio de presentación de datos.

- Controlador (Controller): Coordinar al modelo y a la vista. Actúa como intermediario entre el modelo y la vista. Recibe las acciones del usuario desde la vista y las procesa, actualizando el modelo y la vista según sea necesario. El controlador gestiona la lógica de la aplicación y coordina la interacción entre el modelo y la vista.

El flujo de trabajo típico en el modelo MVC es el siguiente:

1. El usuario interactúa con la vista, por ejemplo, realizando una acción como hacer clic en un botón.
2. La vista notifica al controlador sobre la acción realizada.
3. El controlador recibe la acción y realiza las operaciones necesarias en el modelo.
4. El modelo actualiza sus datos y notifica a la vista sobre los cambios realizados.
5. La vista actualiza su representación visual para reflejar los cambios en los datos del modelo.
6. El ciclo se repite según las acciones del usuario.
7. El modelo MVC proporciona una estructura clara y separada para desarrollar aplicaciones, lo que facilita la reutilización del código, la modularidad y el mantenimiento del software. Además, promueve la escalabilidad y la flexibilidad, ya que cada componente puede ser modificado o reemplazado sin afectar directamente a los demás.

## 12.1. Paradigmas derivados del MVC
Algunos patrones de diseño derivados del MVC son: 
- HMVC:El patrón HMVC (Hierarchical Model-View-Controller) es una variante del patrón MVC (Model-View-Controller) que se utiliza en el desarrollo de aplicaciones web. El objetivo del HMVC es proporcionar una estructura modular y jerárquica para el desarrollo de aplicaciones web complejas.
- MVA: El patrón MVA (Model-View-Adapter) es un patrón de diseño de software que se utiliza para separar y organizar los componentes de una aplicación en tres partes distintas: el modelo, la vista y el adaptador.
- MVP:El patrón MVP (Model-View-Presenter) es un patrón de diseño de software que se utiliza para separar la lógica de presentación de la lógica de negocio en aplicaciones de interfaz de usuario. Es una variante del patrón MVC (Model-View-Controller) y se centra en la interacción entre la vista y el presentador.
- MV VM:El patrón MVVM (Model-View-ViewModel) es un patrón de diseño de software que se utiliza comúnmente en el desarrollo de aplicaciones de interfaz de usuario. Es una variante del patrón MVC (Model-View-Controller) y está diseñado para separar la lógica de presentación de la lógica de negocio y los datos.