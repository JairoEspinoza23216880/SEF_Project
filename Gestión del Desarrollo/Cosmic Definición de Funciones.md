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
