# Aplicación de Gestión de Ingredientes y Generación de Recetas (AGIGR)
INTRODUCCION
Las personas a menudo se encuentran con alimentos en casa, como verduras, frutas y condimentos, pero no saben qué platos preparar con ellos. Esto puede generar falta de inspiración culinaria y llevar al desperdicio de alimentos. Existe una necesidad de una herramienta que ayude a aprovechar al máximo los ingredientes disponibles y facilite la planificación de comidas.
Problema identificado:
Los usuarios no saben qué platos pueden preparar con los ingredientes que ya tienen, lo que dificulta la planificación de comidas y puede resultar en desperdicio de alimentos.
## Solución
Se propone desarrollar una aplicación que permita a los usuarios ingresar los nombres de los ingredientes que tienen en casa (como verduras, frutas y condimentos). La aplicación generará automáticamente una lista de recetas que se pueden hacer con esos ingredientes, sugiriendo combinaciones de alimentos y, en caso de ser necesario, mostrando qué ingredientes adicionales podrían mejorar las recetas.
Solución propuesta:
Una aplicación que recibe los ingredientes que el usuario tiene disponibles y sugiere recetas basadas en ellos, optimizando el uso de los alimentos, evitando desperdicios y facilitando la planificación de comidas.
## Actores
En esta aplicación, los actores principales son:

•	`Usuario` (Cocinero): Es la persona que introduce los ingredientes disponibles en la aplicación y recibe sugerencias de recetas. Además, puede ver instrucciones detalladas de preparación.

•	`Sistema` externo (opcional): Puede conectarse con bases de datos de recetas externas o con sistemas de comercio electrónico para sugerir ingredientes que faltan en la receta o mejorar las opciones de preparación.

## Diagrama de Casos de Uso
El diagrama de casos de uso ilustra las interacciones entre los actores y el sistema. Para esta aplicación, los casos de uso incluyen:
•	Usuario (Cocinero):
o	Ingresar los ingredientes disponibles -> "Sugerir recetas".
o	Seleccionar una receta -> "Ver instrucciones detalladas".
•	Administrador del sistema:
o	Gestionar las recetas -> "Agregar, editar o eliminar recetas en la base de datos".
Descripción gráfica (diagrama):
•	Un actor "Usuario" conectado a los casos de uso "Ingresar ingredientes" y "Ver recetas".
•	Un actor "Administrador" conectado al caso de uso "Gestionar recetas".
## Patrón de Arquitectura
Se ha optado por el patrón `MVC` (Modelo-Vista-Controlador) debido a su idoneidad para aplicaciones web y móviles que dependen de la interacción entre el usuario y una base de datos dinámica.
•	Modelo: Encargado de gestionar la lógica de datos, incluyendo la lista de ingredientes del usuario y la base de datos de recetas.

•	Vista: Es la interfaz gráfica que permite a los usuarios interactuar con la aplicación, ingresando sus ingredientes y viendo las recetas sugeridas.

•	Controlador: Se encarga de recibir las acciones del usuario (como ingresar ingredientes), procesarlas, consultar el modelo (base de datos de recetas) y actualizar la vista con los resultados correspondientes.
## Prototipo de la app
 