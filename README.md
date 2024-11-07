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
•	`Administrador` del sistema: Persona encargada de gestionar y mantener actualizada la base de datos de recetas, asegurando que las opciones disponibles para los usuarios estén actualizadas y sean variadas.
•	`Sistema` externo (opcional): Puede conectarse con bases de datos de recetas externas o con sistemas de comercio electrónico para sugerir ingredientes que faltan en la receta o mejorar las opciones de preparación.
## Historia de Usuario
Las historias de usuario son fundamentales para entender las necesidades de los actores y describen las funcionalidades desde su perspectiva. Algunas historias de usuario relevantes para esta aplicación son:
•	Historia de Usuario 1:
"Como usuario, quiero ingresar los ingredientes que tengo en casa y que la aplicación me muestre recetas que pueda preparar con ellos."
•	Historia de Usuario 2:
"Como administrador, quiero actualizar y gestionar la base de datos de recetas para que los usuarios siempre tengan opciones nuevas y relevantes."
## Criterios de Aceptación
Los criterios de aceptación son condiciones que deben cumplirse para que una historia de usuario se considere completada correctamente. A continuación, se presentan los criterios de aceptación correspondientes a las historias de usuario anteriores:
•	Historia de Usuario 1:
o	El usuario puede agregar y eliminar ingredientes de su lista personal.
o	La aplicación muestra una lista de recetas que requieren únicamente los ingredientes que el usuario tiene disponibles.
o	Si una receta necesita ingredientes adicionales, la aplicación sugiere qué ingredientes faltan y posibles sustitutos.
o	Las recetas sugeridas incluyen instrucciones claras y detalladas para su preparación.
•	Historia de Usuario 2:
o	El administrador puede agregar nuevas recetas a la base de datos.
o	El administrador puede editar y eliminar recetas existentes.
o	La aplicación actualiza la lista de recetas disponibles en tiempo real para los usuarios.
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
## Prototipo en Baja Fidelidad
El prototipo en baja fidelidad es un esquema simple y preliminar que permite visualizar la estructura y el flujo de la aplicación sin enfocarse en los detalles estéticos o interactivos. Su propósito principal es validar la disposición de los elementos y la navegación entre las pantallas.
Características:
•	Dibujo básico o wireframe: Esbozo de las pantallas principales, mostrando dónde estarán ubicados los componentes clave (botones, campos de texto, listas).
•	Enfoque en la funcionalidad: El objetivo es definir qué acciones puede realizar el usuario en cada pantalla y cómo interactúan entre sí.
•	Pantallas clave:
o	Pantalla de inicio: El usuario puede ingresar los nombres de los ingredientes que tiene disponibles.
o	Pantalla de resultados de recetas: Lista de recetas sugeridas basadas en los ingredientes ingresados.
o	Pantalla de detalles de receta: Instrucciones detalladas de una receta seleccionada.
Ejemplo (descripción):
•	Pantalla de inicio: Incluye un campo de texto donde el usuario puede agregar los nombres de los alimentos, un botón para "Generar Recetas" y una lista de ingredientes añadidos.
•	Pantalla de resultados de recetas: Muestra las recetas sugeridas en una lista, cada una con un botón de "Ver más" para acceder a los detalles de la receta.
•	Pantalla de detalles de receta: Muestra los ingredientes necesarios, instrucciones paso a paso, y posibles sugerencias para sustituir ingredientes faltantes.
## Prototipo en Media Fidelidad
El prototipo en media fidelidad es una versión más desarrollada y cercana al diseño final de la aplicación, pero aún sin el nivel completo de detalles o interactividad del prototipo de alta fidelidad. Este tipo de prototipo incluye una estructura visual más definida y algunos elementos interactivos básicos.
Características:
•	Diseño gráfico más detallado: Se implementan colores, tipografía y disposición de los elementos más próximos al diseño final.
•	Interactividad básica: Se pueden navegar entre pantallas para mostrar cómo sería el flujo real del usuario dentro de la app.
•	Herramientas de creación: El prototipo de media fidelidad se puede crear con herramientas como Adobe XD, Figma o InVision.
Pantallas clave:
•	Pantalla de inicio: Incluye una barra de búsqueda estilizada donde el usuario ingresa los ingredientes, botones más definidos (con diseño visual) para añadir o eliminar ingredientes, y un botón más visible para generar las recetas.
•	Pantalla de resultados de recetas: Las recetas aparecen con imágenes representativas y los nombres de los platos sugeridos, organizados en tarjetas o listas. Cada receta tiene un botón que permite al usuario ver más detalles.
•	Pantalla de detalles de receta: Se muestran los ingredientes necesarios, un paso a paso de la preparación y opciones para compartir la receta o guardarla en favoritos.
Ejemplo visual:
El diseño tiene una estructura más cuidada, con iconografía, colores y tipografía que reflejan el estilo de la aplicación. En este prototipo se pretende que el usuario pueda realizar las acciones clave de manera intuitiva, probando la funcionalidad de las interacciones.