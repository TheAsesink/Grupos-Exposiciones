# UNIVERSIDAD TÉCNICA ESTATAL DE QUEVEDO

**TEMA:**
Resumen de las exposiciones de cada grupo.

**Estudiante:**
CASTRO ESPINOZA KEVIN MOISES

**DOCENTE:**
DR. GLEISTON CICERÓN GUERRERO ULLOA

**CURSO:**
5TO SOFTWARE "A"

**FECHA:**
VIERNES, 24 DE JULIO DEL 2026

---

## GRUPO SVELTE

**Fred Beltrán:** Presentó Svelte y explicó cómo consumir APIs, además de la estructura que tendría la exposición y las demostraciones. Comentó brevemente la historia de Svelte y SvelteKit, comparándolos con React en aspectos como latencia, rendimiento y el uso de librerías pesadas. Mencionó que una de las principales características de Svelte es que trabaja en tiempo de compilación, evitando el uso del Virtual DOM, lo que mejora el desempeño de las aplicaciones web. También destacó que SvelteKit permite desarrollar aplicaciones full stack, con endpoints versátiles y una sintaxis sencilla para aplicaciones web.

Explicó la estructura básica de un proyecto creado con la plantilla minimal, mostrando una jerarquía pequeña y el archivo main.js como punto de inicio. Además, describió la estructura general para consumir APIs mediante métodos como GET, POST, PUT y DELETE.

Indicó que Svelte está orientado al frontend, permitiendo crear interfaces con un código limpio y directo, sin depender de grandes estructuras de CSS. Como ejemplo utilizó el proyecto BIOPET, aclarando que el framework no necesita conocer cómo está construido el backend.

Posteriormente explicó el código del proyecto, mostrando la URL de la API, el manejo del estado mediante Runes, el proceso de inicio de sesión y la sintaxis utilizada para consumir la API. Describió la función login, que realiza dos solicitudes, enviando la información mediante un JSON en el cuerpo de la petición. También explicó el uso de Spring Boot, JWT y fetch, indicando que algunas peticiones reutilizan la información obtenida anteriormente, como el correo y el usuario.

Durante la demostración mostró el frontend antes de implementar las operaciones GET y POST, desarrollándolas en tiempo real. Destacó que Svelte es un framework muy reactivo y práctico para proyectos pequeños y medianos, aunque puede presentar limitaciones en desarrollos de mayor complejidad.

Como ventajas señaló su rapidez, reactividad y la facilidad de aprendizaje, además de que SvelteKit incorpora herramientas para backend. Entre las desventajas mencionó que su ecosistema es reducido, existen pocos proyectos desarrollados con esta tecnología en Ecuador y puede quedarse corto en sistemas grandes o con múltiples subsistemas.

Finalmente comparó Svelte con React, resaltando que su principal fortaleza es la simplicidad y el buen rendimiento gracias a que utiliza JavaScript sin depender de librerías pesadas, aunque su comunidad y ecosistema siguen siendo más pequeños.

**Alison Zambrano:** Explicó que Svelte trabaja separado del backend, a diferencia de frameworks como Laravel que integran ambas partes. Indicó que esta separación facilita el desarrollo del frontend, aunque requiere mayor organización cuando se trabaja en proyectos grandes.

Utilizó como ejemplo un sistema para una biblioteca, diferenciando las funciones del recepcionista, bibliotecario y usuario. Señaló que el frontend es la parte visible para el usuario, mientras que el backend procesa la información.

Describió el proceso de autenticación: el usuario registra su correo y contraseña, fetch envía los datos al backend mediante una petición POST, el servidor verifica la información, genera un token JWT y lo devuelve al frontend para mantener la sesión.

En la demostración ejecutó primero el backend y luego el frontend, mostrando el funcionamiento independiente de cada uno y la interfaz final que observa el usuario.

## GRUPO ALPINE.JS

**Marlon Loor:** Inició la presentación explicando que anteriormente el proyecto solo contaba con frontend, pero en esta demostración incorporó un backend con persistencia de datos utilizando Express.js y una base de datos SQLite. Indicó que Alpine.js es una librería ligera, mientras que SQLite permite almacenar información localmente sin depender de conexión a Internet ni de servicios externos.

Mostró la estructura del proyecto, explicando el archivo index.html, donde se importan las librerías necesarias para utilizar directivas como x-data. También presentó los archivos de JavaScript encargados de realizar las operaciones CRUD desde el frontend hacia la base de datos. Señaló que SQLite almacena la información en un archivo binario y que el proyecto utiliza un único archivo server.js, sin separar controladores, para gestionar el consumo de la API. Además, explicó que con un solo comando se levantan el frontend y el backend en el puerto 3000, validando el funcionamiento mediante Postman.

Posteriormente mostró un backend desarrollado en Spring Boot ejecutándose en el puerto 8080, donde visualizó los endpoints de autenticación y consulta de usuarios. Comentó que Alpine.js destaca por su facilidad de aprendizaje gracias a directivas como x-data, x-init, x-show, x-text y x-model, que simplifican la interacción con la interfaz.

Durante la demostración explicó la configuración general del proyecto ARTISYNC, incluyendo los estilos, el contenedor principal con x-data y la función de inicio de sesión. Describió la creación del formulario mediante x-model, la validación de campos como correo y contraseña, y el uso de funciones asíncronas con fetch para enviar la información al servidor. También presentó la clase cliente.js, donde se define la URL base del backend, además del manejo de respuestas exitosas y errores. Finalmente mostró el registro de clientes, incluyendo datos como nombres, apellidos, contraseña y fecha de nacimiento, iniciando sesión como administrador para visualizar los registros almacenados.

Como ventajas destacó la curva de aprendizaje corta, ya que Alpine.js cuenta con pocas propiedades, atributos y métodos, lo que facilita su implementación. Además, explicó que directivas como x-show permiten controlar la visualización de elementos de forma sencilla. Como desventaja mencionó que está limitado a las funcionalidades propias de la librería, por lo que no recomienda utilizarlo en proyectos de software de gran tamaño o alta complejidad.

## GRUPO NEXT.JS

**Alejandro Pallo:** Explicó que Next.js está basado en React y que, para la demostración, consumiría una API desde el frontend. Inició creando el proyecto con el comando npm create next, indicando que decidió realizar la configuración manual. Comentó que no utilizaría TypeScript, el compilador de React ni herramientas adicionales para CSS, ya que trabajaría con CSS tradicional.

Mostró la estructura del proyecto y el archivo de configuración donde se establece la conexión con el backend desarrollado en Spring Boot. Explicó que existe una ruta que funciona como intermediaria para capturar todas las solicitudes dirigidas a la API y redirigirlas al servidor correspondiente.

Posteriormente presentó la función encargada del login, la cual verifica las credenciales del usuario y devuelve un mensaje de error cuando la autenticación falla. También explicó el consumo de datos mediante el método GET para obtener la información de los estudiantes desde la API.

Durante la explicación señaló una instrucción utilizada para indicar a Next.js que un componente debe ejecutarse en el navegador. Además, mostró el proceso de cierre de sesión, donde se elimina el estado de autenticación y el usuario es redirigido nuevamente al formulario de inicio de sesión. También explicó el manejo del estado donde se almacenan temporalmente los datos del usuario autenticado y la estructura HTML utilizada en cada página de la aplicación.

Finalmente levantó el backend de su proyecto de gestión para una escuela deportiva y realizó la demostración práctica, mostrando cómo los datos almacenados en el servidor se consumen y visualizan correctamente desde el frontend desarrollado con Next.js.

## GRUPO ASTRO

**Irvin Cajas:** Inició la presentación explicando el consumo de datos mediante API REST. Comentó que Astro fue lanzado en 2021 como un proyecto de código abierto con el objetivo de reducir la cantidad de JavaScript enviado al navegador y evitar recompilar todo el proyecto ante pequeños cambios. Destacó características como su buen rendimiento, la arquitectura de islas y la generación de HTML estático, hidratando componentes únicamente cuando es necesario. Además, mencionó que permite definir rutas sin configurar un enrutador, utiliza fetch para comunicarse con APIs y puede integrarse con diferentes tecnologías.

En la demostración utilizó un proyecto de gestión de biblioteca para explicar el funcionamiento de los métodos GET y POST. Indicó que el método POST se emplea para obtener un token JWT, protegiendo la base de datos de accesos no autorizados. Mostró cómo el frontend realiza peticiones mediante fetch, conectándose al backend en el puerto 8080, y posteriormente realizó el registro de un libro. También verificó el funcionamiento de los endpoints mediante Postman utilizando el método GET.

Presentó una tabla comparativa donde señaló que Astro ofrece una curva de aprendizaje baja y un buen rendimiento para consumir APIs. Además, comparó su uso con tecnologías como Express con TypeScript, Laravel y Django, indicando las diferencias en complejidad y aprendizaje.

**Jaime Mariscal:** Expuso un proyecto de una veterinaria para explicar cómo Astro consume información desde una base de datos mediante el método GET. Comentó que el ORM actúa como intermediario entre la aplicación y la base de datos, evitando realizar consultas directas.

Durante la demostración explicó el flujo de comunicación entre Astro, Spring Boot, JPA, PostgreSQL y Docker. Mostró el backend ejecutándose en el puerto 8080, desde donde Astro consume los endpoints. Después inició sesión con un usuario administrador, indicando que los endpoints están protegidos mediante autenticación. También explicó cómo se recupera el token del usuario autenticado y cómo fetch utiliza el método GET para consultar información sin modificar los registros.

Finalmente mostró la lista de mascotas almacenadas en la base de datos mediante el consumo de la API desarrollada con Spring Boot.

Como caso de uso real mencionó el proyecto Candian Solar, implementado en Brasil para gestionar la retroalimentación de capacitadores. Señaló que Astro no se limita a proyectos educativos y que su adopción es mayor en países como Brasil y Colombia, aunque en Ecuador todavía es poco utilizado.

**María Escudero:** Presentó la estructura principal de un proyecto en Astro, describiendo carpetas como public, src, components, layouts y pages, además de archivos como package.json y tsconfig.json. Posteriormente dio inicio a la práctica.

En la demostración mostró un proyecto donde el frontend consume los métodos GET y POST de una API. Explicó el uso de fetch para realizar las peticiones HTTP y cómo el backend responde en formato JSON, devolviendo un token que se almacena para mantener la sesión del usuario. Luego realizó el inicio de sesión y el registro de nuevos conductores dentro de la aplicación.

Como ventajas destacó el buen rendimiento de Astro, la reducción del código JavaScript enviado al navegador y la posibilidad de consumir APIs desarrolladas con diferentes tecnologías. Entre las desventajas mencionó que no es un framework backend tradicional, no incorpora un ORM obligatorio y que algunas funcionalidades dinámicas requieren adaptadores dependiendo del servidor utilizado.

Como conclusión señaló que Astro facilita el consumo de APIs REST y permite integrarse con distintos lenguajes y plataformas. Recalcó que su función principal es actuar como un frontend rápido para comunicarse con servicios web, más que reemplazar a un framework backend.

## SOLID.JS SOLIDSTAR

**Tejada:** Explica la historia de quien inicio el desarrollo y que se libera como open source y como contratan al equipo de raya y con eso crearon solid star, explica el apartado de estructura del proyecto.

También explico cómo se ve la estructura del proyecto aplicando el framework, usando la terminal con el npm create solid@latest, También muestra su rama y todas las dependencias que tienen, la configuración de drezzle con la migración de los datos con respecto a la estructura.

También mostro como este interactúa con su proyecto fin de curso.

También explico sobre sus ventajas y desventajas, y que es un framework joven y este tiene la desventaja de tener poca documentación o guías.

Su recomendación fue no usarlo no porque fuera malo, si no que este no tiene una guía sólida para poder guiarse.

Explico que como el framework es nuevo, no se pudo encontrar algún proyecto o sistema creado aquí en ecuador, pero menciono que una compañía se junto con estos desarrolladores y se avanzo en el conocimiento de este.

**Moncayo:** Explico la tabla comparativa entre el framework solidstar, Express.js y Spring boot y procedió con su práctica.

Explico el significado de cada carácter y la función de cada una de ellas.

También explico que en la carpeta de validación tiene una sola razón para existir y es verificar si esta cumple los requisitos del sistema, también explico la función de los involucrados en su proyecto y los roles de cada uno de ellos.

**Ricardo:** Explica que Read nació en meta, menciono unos datos sobre el dom y de modular usefech y procedió con la práctica.

Explico sobre los Interceptors y que estos se ejecutan por cada petición y sin este receptor cada token debería iniciarse manualmente, explico sobre las Apis y sobre la validación de las credenciales, menciono que en su pantalla de login manejan 3 cosas, credenciales, errores y el estado de carga.

Explico sobre HandleChange y que, con el protectedlayout que este revisa si esta guardado y protege los datos el navigate regresa hacia atrás y borra los datos del historial ingresados anteriormente para así asegurar que esa información no se divulgue o filtre.

**Arcalle:** Explica como consume el api de estudiantes, explico los servicios que se van a utilizar para los estudiantes, como categoría service en el que se tiene una categoría exportable, utilizo el método get que le retorna un dato response.

Explico que lo que se solicita en el apartado de estudiantes, se piden funciones asíncronas con parámetros de consulta y que este usa un formato de page o paginación.

Explico que el UseState se usa para datos que cambian con el tiempo, Que el UseEffect tiene datos de manera externa y que se pueden trabajar con esos datos, y que, si el usuario hace peticiones constante mente, se usa el Let active para evitar una condición de carrera y que se sobre escriban los datos al recargar la página constantemente.

Explico como uso el HandleOpenModal y su funcionamiento dentro de su función estudiantes y procedió con la practica visual de como se ve en su proyecto.

**Fajardo:** Procedio directamente con la practica, explico sobre el App.jsx, y que uso el UseEffect, enseño donde esta el api_rest localhost, mostro las peticiones de su API_URL con el puerto 8080, uso los seriales de @id para indicarle a pg los identificadores de cada uno de los controladores webservices.

@CrossOrigin, ahí se encuentra el origins='http:localhost'

En el getmaping lo asocia a la ruta api_tareas, ya que este le pide que traiga todas las tareas.

Paso a la pagina del html, creo una nueva tarea y dijo que las casillas se recargan automáticamente sin necesidad de presionar ctrl+r, y cerro diciendo algo sobre
