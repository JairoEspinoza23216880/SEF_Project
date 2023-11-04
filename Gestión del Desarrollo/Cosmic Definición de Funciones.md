# Definición de Funciones (RF)

### Requerimientos MUST HAVE

#### *Itinerario de IA*

**Entrada :**
	El Usuario ingresa el formulario de preferencias, tiempos y presupuesto que le servirán a la IA para generar el itinerario

**Escritura :**
	El sistema guarda los datos del formulario del usuario dentro de la Database

**Lectura :**
	El sistema revisa la información guardada para que la IA pueda procesarla

**Escritura :**
	El sistema almacena el itinerario resultante de forma temporal, en espera de que el usuario confirme el guardado o no

**Salida :**
	El sistema devuelve al usuario el itinerario temporal para que pueda visualizarlo


#### *Visitar Páginas de Sitios de Interés*

**Entrada :**
	El usuario solicita el ingreso a la sección de páginas de sitios.

**Lectura :**
	El sistema revisa las preferencias guardadas del usuario para usarlas al buscar sitios.

**Lectura :**
	El sistema accede a la información guardada de todos los lugares que se han registrado en la aplicación con base a las preferencias del usuario.

**Salida :**
	El sistema devuelve al usuario los resultados de su búsqueda.

**Entrada :**
	El usuario solicita ingresar a un sitio en específico.

**Lectura :**
	El sistema accede a la información de ese sitio específico.

**Salida :**
	El sistema devuelve al usuario la información del sitio específico.


#### *Creación de Páginas de Sitios*

**Entrada :**
	El usuario solicita la creación de una página.

**Lectura :**
	El sistema revisa si el usuario está registrado como usuario en la Database.

**Entrada :**
	El usuario ingresa todos los datos del sitio que desea agregar.

**Escritura :**
	El sistema introduce los datos del sitio del usuario dentro de la Database.

**Salida :**
	El sistema devuelve al usuario su página creada.



### Requerimientos SHOULD HAVE

#### *Verificación de Empresas/propietario*

**Entrada :**
	El propietario/empresario inicia el proceso de verificación de su negocio al hacer.

**Lectura :**
	El propietario/empresario proporciona sus datos personales, como nombre, dirección, número de identificación. 

**Entrada :**
	El usuario adjunta documentos que verifique su propiedad para si poder ser verificado.

**Salida :**
	La aplicación redirige al empresario/propietario para completar el proceso de verificación.

**Escritura :**
	Los datos verificados y aprobados se almacenan en un medio de almacenamiento.


#### *Procesamiento de palabras*

**Entrada :**
	Los usuarios ingresan palabras clave que describen sus preferencias de viaje, como destino, actividad, duración, presupuesto.

**Lectura :**
	La aplicación procesa las palabras clave proporcionadas por el usuario y las utiliza como datos de entrada para la generación automática de itinerarios por IA.

**Salida :**
	El resultado de la generación automática del itinerario se muestra al usuario como un plan de viaje sugerido y con la posibilidad de ser cambiado.

**Escritura :**
	La información sobre el itinerario generado se almacena en un medio de almacenamiento persistente, como una base de datos, para su posterior referencia.


#### *Acceso a la herramienta Google Maps*

**Entrada :**
	Los datos de entrada pueden incluir la ubicación actual del usuario, el destino seleccionado y cualquier punto de partida adicional si el usuario lo especifica e incluir su medio de transporte, como puede ser un coche o que tal vez esté utilizando el transporte público por ejemplo.

**Salida :**
	La salida será la información generada por Google Maps que es referente a que genere una ruta en base a su punto de partida hasta su ubicación e incluir el mapa con la ruta trazada.

**Lectura :**
	El usuario especifica la ubicación actual o lo detecta el GPS, el destino y otros detalles como lo puede ser su movilidad o vehículo que esté utilizando.

**Escritura :**
	Los datos que se presentaran será la información de la ruta y el tiempo estimado de viaje que se obtiene de Google Maps. Estos datos se muestran al usuario en la interfaz de usuario.


#### *Registro de Usuario*

**Entrada :**
El usuario accede a la aplicación.

**Entrada :**
En la pantalla aparecerá que proporcione los datos para completar el registro, además también aparecerá una opción que diga “continuar sin registro” en dado caso de que quiera omitir esto.

**Lectura :**
Si el usuario elige registrarse deberá proporcionar los datos personales que se le soliciten como nombre, correo electrónico, etc.

**Lectura :**
En caso de que el usuario continúe sin registro solo se le permitirá el acceso a generar itinerarios y no podrá acceder a las demás funciones.

**Salida :**
Se le solicitara al usuario que genere una contraseña para acceder a la cuenta y terminar el registro.

**Salida :**
Se le solicita que elija un método para en caso de que olvide su contraseña pueda recuperar la cuenta.

**Escritura :**
Se almacenarán los datos proporcionados por el cliente, su nombre de usuario y contraseña en la base de datos de la aplicación.


#### *Calificación de Sitios*

**Entrada :**
En el menú de opciones, el usuario seleccionara el apartado de calificación de sitios 

**Entrada :**
El usuario podrá buscar o elegir un sitio de su interés.

**Entrada :**
Al seleccionarlo aparecerá información del lugar, así como comentarios de otros usuarios y su calificación.

**Lectura :**
Ahí mismo aparecerá un apartado donde el usuario podrá comentar su opinión sobre el sitio y calificarlo con estrellas en una escala del 1 al 5 (Puede mejorar, regular, bueno, muy bueno, excelente).

**Lectura :**
Si el usuario es dueño de algún sitio de interés (como restaurantes u hoteles) también aparecerán opciones que le permitan editar la descripción de su sitio.

**Salida :**
Aparecerá la opción de “publicar comentario” al seleccionarlo, el comentario y la calificación del usuario serán público y los demás usuarios que accedan al sitio también podrán verlo.

**Escritura :**
Se guardarán los datos proporcionados por el usuario y podrá acceder a ellos y editarlos en el momento que lo desee.



### Requerimientos COULD HAVE

#### *Visualizar Itinerario*

**Entrada :**
El usuario selecciona un itinerario de una lista o mediante una búsqueda específica.

**Entrada :**
El sistema recibe la selección del usuario y procede a buscar la información correspondiente (El identificador del itinerario seleccionado).

**Lectura :**
El sistema consulta la base de datos para obtener los detalles del itinerario seleccionado.

**Lectura :**
Se recuperan los datos del itinerario, incluyendo paradas, tiempos estimados y otros detalles relevantes (El nombre, la descripción, la duración, las coordenadas, las imágenes y los comentarios del itinerario y sus paradas).

**Salida :**
El sistema presenta el itinerario en la interfaz gráfica en el formato elegido por el usuario (lista o mapa).

**Salida :**
Se muestra visualmente el itinerario completo, permitiendo al usuario interactuar con él para obtener más información o modificarlo. (El itinerario y sus paradas con sus respectivos datos).