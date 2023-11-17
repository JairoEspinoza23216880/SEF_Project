# Investigación


[Infografía](/IS.pdf)

### Habilidades Técnicas de la Ingeniería de Requerimientos

##### Análisis de Requerimientos
El análisis de requisitos o ingeniería de requisitos es un proceso utilizado para determinar las necesidades y expectativas de un nuevo producto. Implica una comunicación frecuente con las partes interesadas y los usuarios finales del producto para definir expectativas, resolver conflictos y documentar todos los requisitos clave.

##### Especificación de Requerimientos
Una especificación de requisitos de software (SRS) es un documento que describe lo que hará el software y cómo se espera que funcione. También describe la funcionalidad que el producto necesita para satisfacer las necesidades de todas las partes interesadas (negocios, usuarios).

##### Modelado de Requerimientos
El modelado de requisitos es el proceso de documentar, analizar y gestionar requisitos. Los requisitos pueden ser cualquier cosa que un cliente o usuario desee de un sistema de software. Pueden incluir requisitos funcionales (lo que debería hacer el sistema), requisitos no funcionales (como rendimiento, seguridad, etc.), así como restricciones (cosas que podrían limitar lo que el sistema puede hacer).

### Casos de Uso VS Historias de Usuario

##### Casos de Uso
Un modelo de casos de uso es un modelo de cómo diferentes tipos de usuarios interactúan con el sistema para resolver un problema. Como tal, describe los objetivos de los usuarios, las interacciones entre los usuarios y el sistema y el comportamiento requerido del sistema para satisfacer estos objetivos.

Se utiliza un diagrama de casos de uso para representar gráficamente un subconjunto del modelo para simplificar las comunicaciones. Normalmente habrá varios diagramas de casos de uso asociados con un modelo determinado, cada uno de los cuales muestra un subconjunto de elementos del modelo relevantes para un propósito particular.

El modelo de casos de uso sirve como hilo conductor a lo largo del desarrollo del sistema. Se utiliza como especificación principal de los requisitos funcionales del sistema, como base para el análisis y el diseño, como entrada para la planificación de iteraciones, como base para definir casos de prueba y como base para la documentación del usuario.

##### Historias de Usuario
Una historia de usuario es la unidad de trabajo más pequeña en un marco ágil. Es un objetivo final, no una función, expresado desde la perspectiva del usuario del software.

Una historia de usuario es una explicación general e informal de una función de software escrita desde la perspectiva del usuario final o cliente.

El propósito de una historia de usuario es articular cómo un elemento de trabajo entregará un valor particular al cliente. Ten en cuenta que los "clientes" no tienen por qué ser usuarios finales externos en el sentido tradicional, también pueden ser clientes internos o colegas dentro de tu organización que dependen de tu equipo.

Las historias de usuario son unas pocas frases en lenguaje sencillo que describen el resultado deseado. No entran en detalles, ya que los requisitos se añaden más tarde, una vez acordados por el equipo.

##### VS
La historia de usuario se redacta para explicar las necesidades de un usuario. Pone de relieve un problema al que se enfrenta un usuario en su día a día. El lenguaje de este borrador es muy simple. Está desarrollado para mantener a todas las partes interesadas en la misma página. Por otro lado, los casos de uso se desarrollan únicamente para el equipo de producto. Le da al equipo una idea de lo que debería lograr el software. También destaca todos los pasos que los desarrolladores deben seguir para crear el software. Por esta razón, los casos de uso contienen muchos más detalles que las historias de usuarios.
La historia de usuario es una forma simplificada de muchos usuarios que interactúan con un software. Los casos de uso son muy específicos en relación con las historias de usuarios. Describen acciones específicas del usuario con cualquier sistema.
Las historias de usuarios pierden muchos detalles. Esto se debe a que da lugar a la discusión y la mejora. Este aspecto de las historias de usuarios es deliberado. Esto anima a las partes interesadas a iniciar debates y mejorar el producto. Por otro lado, los casos de uso son específicos. Describen en detalle todos los pasos que seguirá un desarrollador. Generalmente no hay lugar para la discusión.
Las historias de usuario se desarrollan antes que el caso del uso. En la mayoría de los casos se desarrollan mediante la interacción del usuario. Una historia de usuario puede generar múltiples casos de uso. La combinación de todos estos casos de uso produce un documento detallado. Este documento tiene una descripción de la interacción entre todo el software y los usuarios.

![[UserStory_VS_UseCase.png]]

### Diseño y Métodos

##### Diseño UI
El diseño de interfaz de usuario (UI) es el proceso que utilizan los diseñadores para crear interfaces en software o dispositivos computarizados, centrándose en la apariencia o el estilo. Los diseñadores pretenden crear interfaces que los usuarios encuentren fáciles de usar y placenteras. El diseño de UI se refiere a interfaces gráficas de usuario y otras formas, por ejemplo, interfaces controladas por voz.

##### Método (Prototipado)
Un prototipo en el desarrollo de software es una simulación de cómo funcionará y se sentirá un producto real. Se utiliza para comentarios de diseño y pruebas de usuarios.

Con una definición intencionadamente amplia, pueden presentarse en todos los niveles de sofisticación, desde una idea esbozada en el reverso de una servilleta hasta un prototipo en el que se puede hacer clic que imita un software real.

Y dependiendo de lo que necesites, un prototipo puede servir como simulación de una aplicación móvil completa o solo de una interacción digital.

### Desarrollo y Pruebas

##### Método para Pruebas en Desarrollo (TDD)
En términos sencillos, Test Driven Development (TDD) es una práctica de desarrollo de software que se centra en la creación de casos de prueba unitaria antes de desarrollar el código real. Es un enfoque iterativo que combina programación, creación de pruebas unitarias y refactorización.

- El enfoque TDD se origina en los principios del manifiesto ágil y la programación extrema.
- Como sugiere el nombre, el proceso de prueba impulsa el desarrollo de software.
- Además, es una práctica estructurante que permite a los desarrolladores y evaluadores obtener código optimizado que resulta resistente a largo plazo.
- En TDD, los desarrolladores crean pequeños casos de prueba para cada característica basándose en su comprensión inicial. La intención principal de esta técnica es modificar o escribir código nuevo sólo si las pruebas fallan. Esto evita la duplicación de scripts de prueba.

1) **Cree pruebas precisas:** los desarrolladores deben crear pruebas unitarias exactas para verificar la funcionalidad de funciones específicas. Deben asegurarse de que la prueba se compile para que pueda ejecutarse. En la mayoría de los casos, la prueba está destinada a fallar. Este es un error significativo ya que los desarrolladores crean pruebas compactas basadas en sus suposiciones sobre cómo se comportará la característica.
2) **Corrección del código:** una vez que una prueba falla, los desarrolladores deben realizar los cambios mínimos necesarios para actualizar el código para que se ejecute correctamente cuando se vuelva a ejecutar.
3) **Refactorice el código:** una vez que la prueba se ejecute correctamente, verifique la redundancia o cualquier posible optimización del código para mejorar el rendimiento general. Asegúrese de que la refactorización no afecte el comportamiento externo del programa.

![[TDD.png]]

### Manifiesto Ágil, Valores y Conflictos

##### Valores
- *Individuos e interacciones sobre procesos y herramientas:* Este valor significa que se debe dar más importancia a las personas que trabajan en el proyecto y a la forma en que se comunican y colaboran, que a los procedimientos y las herramientas que utilizan.
- *Software funcionando sobre documentación exhaustiva:* Este valor significa que se debe dar más importancia a entregar software que funcione y que aporte valor al cliente, que a generar documentación detallada y extensa que describa el software.
- *Colaboración con el cliente sobre negociación contractual:* Este valor significa que se debe dar más importancia a establecer una relación de confianza y cooperación con el cliente, que a seguir un contrato rígido y formal que defina el alcance, el costo y el tiempo del proyecto.
- *Respuesta ante el cambio sobre seguir un plan:* Este valor significa que se debe dar más importancia a adaptarse a los cambios que surjan en el entorno o en las necesidades del cliente, que a seguir un plan preestablecido que defina el producto final.

### Metodologías Ágiles

##### Scrum
La metodología Scrum divide el trabajo en pequeñas cápsulas de tiempo (sprints) que suelen durar entre dos semanas y un mes, y en las que se fijan unos objetivos en base a las necesidades del usuario. 

Al finalizar un sprint, se obtiene un prototipo del producto o servicio, de forma que el cliente puede empezar a utilizar las características más importantes del mismo. Por ello, Scrum puede utilizarse en el desarrollo de soluciones de cualquier industria y en cualquier tipo de proyecto, sea cual sea su complejidad.

##### Kanban
La metodología Kanban se basa en el trabajo en equipo y en el flujo de tareas permanente, potenciando la visualización para ahorrar tiempo en la planificación.

Los flujos de trabajo contemplados en los tableros Kanban deben contener tres elementos fundamentales para poder organizar el desarrollo de las tareas: pendientes, en curso y realizadas.

Para garantizar que el flujo de trabajo sea ágil, el número máximo de tareas que pueden realizarse a la vez debe limitarse. La clave está en no abrir más tareas hasta que se hayan cerrado otras. Por ejemplo, si hay un máximo de 3 tareas y se cierra 1 de 3, podremos abrir la siguiente.

# Referencias

*Habilidades Técnicas de la Ingeniería de Requerimientos:*
https://www.simplilearn.com/what-is-requirement-analysis-article#:~:text=Requirements%20analysis%20or%20requirements%20engineering,document%20all%20the%20key%20requirements.

https://www.perforce.com/blog/alm/how-write-software-requirements-specification-srs-document#:~:text=Tool%20for%20SRS-,What%20Is%20a%20Software%20Requirements%20Specification%20(SRS)%20Document%3F,stakeholders%20(business%2C%20users).

https://visuresolutions.com/blog/requirements-modeling/

*Casos de Uso VS Historias de Usuario:*
https://www.utm.mx/~caff/doc/OpenUPWeb/openup/guidances/concepts/use_case_model_CD178AF9.html

https://www.atlassian.com/es/agile/project-management/user-stories

https://www.digitalnatives.hu/blog/user-story-vs-use-case/#:~:text=User%20story%20is%20a%20simplified,user%20actions%20with%20any%20system.

*Diseño y Métodos:*
https://www.interaction-design.org/literature/topics/ui-design

https://sparkbusinessworks.com/blog/prototyping-in-software-development/

*Desarrollo y Pruebas:*
https://www.browserstack.com/guide/what-is-test-driven-development#:~:text=In%20layman%27s%20terms%2C%20Test%20Driven,unit%20test%20creation%2C%20and%20refactoring.

*Manifiesto Ágil, Valores y Conflictos:*
https://www.bbva.es/finanzas-vistazo/agile/metodologia-agile/valores-principios-manifiesto-agil.html

https://sentrio.io/blog/valores-principios-agile-manifiesto-agil/

*Metodologías Ágiles:*
https://www.grupodigital.eu/blog/metodologias-agiles/

