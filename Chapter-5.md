## Capítulo V: Product Implementation, Validation & Deployment
### 5.1. Software Configuration Management
#### 5.1.1. Software Development Environment Configuration
A continuación, se listará los productos software externos que se han utilizado para el desarrollo del proyecto:
Project Management - Discord y WhatsApp (https://discord.com/) (https://www.whatsapp.com/?lang=es) Discord y WhatsApp han sido los medios principales de comunicación entre los miembros del grupo, donde Discord ha destacado ya que contiene funcionalidades adicionales para organizar grupos de estudio y de trabajo.

Requirements Management - Trello (https://trello.com/es) Trello ha permitido la organización de tareas a realizar en el proyecto, además del desarrollo del product backlog.

Product UX/UI Design - UXPressia (https://uxpressia.com/) Se utilizó UXPressia para el desarrollo de los diagramas user personas, user journey mapping, empathy mapping e impact map. **- Color Space **(https://mycolor.space/) Color Space ha apoyado en la selección de la paleta de colores para el desarrollo del diseño de la web. - Figma (https://www.figma.com/) Se ha utilizado Figma para el desarrollo de los wireframes y prototipos del landing page y aplicación web, tanto en dispositivos de escritorio como de móvil. - Miro (https://miro.com/es/) Miro ha sido empleado en el desarrollo de los escenarios mapping y escenario mapping para ambos segmentos objetivos.

Software Development - Visual Studio Code, Visual Studio Code Community, IntelliJ IDEA (https://code.visualstudio.com/) (https://visualstudio.microsoft.com/es/vs/community/) (https://www.jetbrains.com/idea/) Visual Studio Code, Visual Studio Code Community e IntelliJ IDEA fueron las IDEs que emplearemos para el desarrollo del código del proyecto. Hemos desarrollado el landing page con Visual Studio Code, luego Visual Studio Code Community para el diagrama C4 y emplearemos IntelliJ IDEA para la aplicación web. - Github y Git bash (https://github.com/) (https://git-scm.com/downloads) Github y Git bash nos permitirán el control de versiones del código y el desarrollo colaborativo del proyecto.

Software Testing

Google Chrome Developer (https://www.google.com/intl/es-419/chrome/dev/) Se utilizó Google Chrome en la versión developer para visualizar la interfaz que desarrollamos del landing page.
Software Deployment

Github Pages (https://github.com/) Se utilizó Github Pages para el deploy del landing page.
Software Documentation ● Google Drive (https://www.google.com/intl/es-419_pe/drive/) Se ha utilizado Google Drive para subir archivos de documentos y presentación. Además se han utilizado herramientas como Google Docs y Google Slides que permiten el desarrollo colaborativo de los informes a entregar.

● Google Meets y Zoom (https://meet.google.com/) (https://zoom.us/) Se ha utilizado software para videoconferencias para realizar las entrevistas de segmentos objetivos. Las plataformas tienen herramientas de grabación, por lo que simplifica el procesamiento de los videos. ● Microsoft Stream (https://www.microsoft.com/es-ww/microsoft-365/microsoft-stream) (https://zoom.us/) Se ha utilizado el servicio de Microsoft Stream para subir el video completo de las entrevistas. La cuenta que ha subido el video está vinculado a la organización de la universidad, por lo que se tuvo suficiente espacio de memoria para mantenerlo en la nube. ● LucidChart (https://www.lucidchart.com/pages/es) LucidChart ha sido empleado en el desarrollo de diagramas de flujo para asegurar los user goals y guiar en el diseño de los prototipos de la aplicación web. Además, se ha utilizado para el diagrama de clases. ● Structurizr (https://structurizr.com/) Para el desarrollo del diagrama C4 en los tres niveles: diagrama de contexto, contenedores y componentes se empleó Structurizr junto a Visual Studio Code Community. ● Vertabelo (https://vertabelo.com/) Para el desarrollo del diagrama del diseño de base de datos se ha empleado Vertabelo, software que se especializa en diagramas de base de datos.
#### 5.1.2. Source Code Management
Se ha creado una organización en Github con los miembros del grupo y un repositorio para el landing page. ● Organización: https://github.com/SpeedyRent ● Repositorio landing page: https://github.com/SpeedyRent/Landing-Page ● Despliegue de landing page en Netlify: https://SpeedyRent.netlify.app/ Las ramas principales en el Gitflow serán las ramas developer y master, donde developer será la principal rama de trabajo, mientras que la rama master tendrá la versión final de la web desplegada en Github pages. Por otro lado, se utilizarán ramas secundarias con el nombre de los features que se estén trabajando (hero, navbar branches por ejemplo). Asimismo, se incluyen el branches para release (branch release) y hotfix (branch hotfix).

Commit Conventions Para los commits en Github se han utilizado los estándares convencionales versión 1.1.0 (https://www.conventionalcommits.org/en/v1.0.0/) según la estructura: [optional scope]: ● Type: representa el tipo de commit, sea tipo feature (feat), fix (fix) o docs (docs). ● Optional scope: es opcional y representa el alcance del commit. ● Description: descripción detallada del commit y acciones realizadas.

Semantic Versioning Los releases se realizan según los estándares de Semantinc Versioning 2.0 (https://semver.org/), según el formato MAJOR.MINOR.PATCH. ● MAJOR: versión mayor cuando se implementa cambios de APIs incompatibles. ● MINOR: versión menor cuando se añaden features y funcionalidades nuevas. ● PATCH versión de parche de bug fixes y hotfixes.
#### 5.1.3. Source Code Style Guide & Conventions
HTML Style Guide and Coding Conventions Es necesario seguir convenciones estandarizadas de HTML como estructura de la web. Entre las principales de W3 Schools (https://www.w3schools.com/html/html5_syntax.asp) podemos mencionar:

● Siempre declarar el tipo de documento con "" <div>● Usar siempre letras en minúsculas para los nombres de los elementos.<div> ● Cerrar siempre con los elementos de HTML. <div>● Siempre poner entre comillas los atributos dentro de un elemento html (

)<div> ● Especificar alt, width, and height para imágenes.<div> ● Espaciado y signo igual estandarizados. <div>● Evitar líneas de código extensas.<div> ● No olvidar el “<title></title>” al principio.<div> ● Es posible evitar el “”. <div>● Utilizar meta tags al inicio.
Google HTML/CSS Style Guide Algunas de las convenciones de Google en cuanto a HTML y CSS (https://google.github.io/styleguide/htmlcssguide.html) podemos mencionar: ● Usar la sintaxis y semántica de HTML5. ● Usar minúsculas para los nombres de elementos y atributos. ● Usar comillas dobles para los valores de atributos. ● Usar una nueva línea para cada elemento. ● Usar un espacio después de los dos puntos del nombre de cada propiedad. ● Usar códigos de color hexadecimal (#000000) en vez de nombres propios. ● Usar códigos de color hexadecimales abreviados siempre que sea posible. ● Evitar especificar unidades para valores 0. Por ejemplo, margin: 0px se incluye la unidad de pixeles.

Gherkin Conventions for Readable Specifications Entre las convenciones para Gherkin sobre las pruebas de aceptación se deben considerar convenciones, entre algunas de Specflow (https://specflow.org/gherkin/gherkin-conventions-for-readable-specifications/) están: ● Escribir las especificaciones en un lenguaje simple y fácil de entender por todos los miembros del equipo de desarrollo. ● Utilizar las palabras "Given", "When" y "Then" y “And” para los pasos del escenario. ● Usar verbos finitos y en tiempo presente para las acciones del escenario. ● Evitar redundancias en la descripción de los pasos en el escenario. ● Utilizar formato y estilo consistente en toda la especificación, para todos los escenarios.

Google Java Style Guide A continuación se presentan algunas guías de estilo de Java de la guía de Google (https://google.github.io/styleguide/javaguide.html): ● Las variables y los métodos deben tener nombres descriptivos y seguir la convención de nombres de Java. Los nombres de variables deben comenzar con minúsculas y usar camelcase (por ejemplo prepareOneOrTwo()). ● Las variables constantes deben definirse en mayúsculas y separarse con guiones bajos. ● Los corchetes deben comenzar en la misma línea que la declaración del bloque de código y terminar en una línea separada. ● Los nombres de los paquetes deben ser en minúsculas y seguir la convención de nombres de dominio invertido. ● Usar interfaces para definir tipos, en lugar de clases abstractas. ● Los métodos deben hacer una sola función y respetar el principio de single responsibility.

Spring Boot Features Se mencionarán los core features de Sprint Boot según la documentación oficial de Sprint (https://docs.spring.io/spring-boot/docs/current/reference/html/features.html): ● Clase de aplicación Sprint: empieza con el método main() y inicializa la aplicación con el método SpringApplication.run ● Configuración externalizada: permite realizar cambios en configuración para trabajar en distintos entornos de desarrollo ● Perfiles: segrega funciones según ambiente con @Profile ● Logging: tiene funciones predeterminadas de logging, pero se pueden configurar según necesidad ● Testing: Sprint ofrece varios módulos que facilitan el testing de las funcionalidades ● Soporte con Kotlin
#### 5.1.4. Software Deployment Configuration
Se utilizará el servicio de Netlify (https://www.netlify.com/) para realizar el proceso de deployment del landing page de SpeedyRent. A continuación se presentará el proceso para realizarlo:

Crear o tener una cuenta de Netlify ingresando a su página web oficial (https://www.netlify.com/). Esta cuenta se puede crear con Github, Gitlab o Bitbucket o con un correo convencional.
Una vez con la sesión iniciado, dirigirse a la sección de sitios y seleccionar “Import from Git”
Seleccionamos la opción de GitHub
Seleccionamos la organización con el repositorio a deployar.
Seleccionamos el repositorio y luego nos aparecerá el botón “Deploy Site” al final del formulario. De esta manera, la página ya estaría deployada en unos instantes. Link de deployment: https://SpeedyRent.netlify.app/
### 5.2. Landing Page, Services & Applications Implementation
#### 5.2.1. Sprint 1
##### 5.2.1.1 Sprint Planning 
##### 5.2.1.2 Sprint Backlog 1
##### 5.2.1.3 Development Evidence for Sprint Review
##### 5.2.1.4 Testing Suite Evidence for Sprint Review
##### 5.2.1.5 Execution Evidence for Sprint Review
##### 5.2.1.6 Services Documentation Evidence for Sprint Review
##### 5.2.1.7 Software Deployment Evidence for Sprint Review
##### 5.2.1.8 Team Collaboration Insights during Sprint
