
weather app

Este proyecto consiste en una aplicación que  utiliza la API de OpenWeatherMap para mostrar información meteorológica de cualquier ciudad especificada por el usuario. La aplicación permite al usuario buscar el clima de una ciudad y muestra datos como la temperatura, la humedad, la velocidad del viento, y un ícono representativo del clima actual. construida utilizando HTML, CSS y JavaScript.y utilizando de ejemplo el video de greatstack A continuación, se detallan los componentes principales del código y su funcionalidad.


[![wheater-app.png](https://i.postimg.cc/K8b9kSKG/wheater-app.png)](https://postimg.cc/0btGF4dF)

Estructura del Proyecto
Archivos Principales
index.html: Este archivo contiene la estructura básica de la aplicacion.
style.css: Archivo de estilos que define la apariencia de la aplicacion.
script.js: Script que maneja las funciones y acciones de la aplicacion.

HTML:
La estructura HTML define el diseño de la página web.

La sección contiene metadatos y recursos necesarios para la página. Incluye:

meta nombre="viewport" content="ancho=ancho del dispositivo, escala inicial=1.0"
título de la página web
enlaces a la hoja de estilo y fuentes externas
divs que encansulan el contenido y imagenes de la aplicacion entre ellos card,error,weather
a diferencia de mis anteriores proyectos este cuenta con los titulos y parrafos en el idioma ingles

CSS
el estilo CSS define la apariencia de los elementos de la página web.
 proporciona un  estilo  para  el fondo de la aplicacion y su estilo en forma rectangular 
proporciona un estilo para la muestra de las imagenes y textos
 

JAVASCRIPT
el script permite manejar la muestra de los datos meteorologico utilizando la api a continuacion se describen sus  componentes

Configuración de la API:

apiKey: Clave de acceso a la API de OpenWeatherMap.
apiUrl: URL base para hacer solicitudes de datos meteorológicos a la API de OpenWeatherMap en unidades métricas.
Interacción con el usuario:

El usuario ingresa el nombre de la ciudad en un campo de búsqueda (searchBox).
Al hacer clic en el botón de búsqueda (searchBtn), se llama a la función checkweather().
Obtención de datos meteorológicos:

La función checkweather(city) realiza una solicitud HTTP a la API de OpenWeatherMap utilizando la ciudad proporcionada.
Si la respuesta es válida, la información meteorológica se muestra en la interfaz, como:
Nombre de la ciudad: Actualiza el elemento .city con el nombre de la ciudad.
Temperatura: Muestra la temperatura redondeada en grados Celsius.
Humedad: Muestra el porcentaje de humedad.
Velocidad del viento: Muestra la velocidad del viento en km/hr.
Icono del clima: Selecciona la imagen correspondiente al estado del clima actual (e.g., Nubes, Despejado, Lluvia, Llovizna, Neblina).
Si hay un error (por ejemplo, la ciudad no se encuentra), se muestra un mensaje de error.
Persistencia de datos:

La aplicación almacena en Local Storage el nombre de la última ciudad buscada, de modo que, al recargar la página, se vuelva a mostrar el clima de esa ciudad automáticamente.
Eventos del DOM:

Botón de búsqueda: Al hacer clic en el botón, se obtiene el valor del campo de entrada y se llama a checkweather() con dicho valor.
Carga de la página: Al cargar la página, la aplicación verifica si hay una ciudad almacenada en el Local Storage y, de ser así, muestra el clima de esa ciudad
