## Capítulo V: Product Implementation, Validation & Deployment
### 5.1. Software Configuration Management
#### 5.1.1. Software Development Environment Configuration
En esta sección, detallaremos las plataformas y el software que utilizamos como equipo para el desarrollo y la gestión de nuestro startup. Estas herramientas nos permiten optimizar procesos, colaborar de manera eficiente y asegurar el crecimiento sostenible de nuestro proyecto.<br><br>
**Project Management**<br><br>[Discord](https://discord.com/) y [WhatsApp](https://www.whatsapp.com/?lang=es) han sido los medios principales de comunicación entre los miembros del grupo, donde Discord ha destacado ya que contiene funcionalidades adicionales para organizar grupos de estudio y de trabajo.<br><br>
**Requirements Management**<br><br>Hemos utilizado [Trello](https://trello.com/home) como herramienta principal para la organización y gestión de tareas. En Trello, creamos listas específicas para las etapas del trabajo, como “Entregables”, "Por Hacer", "En Proceso", "Pendiente de Revisión" y "Completado". Cada lista contiene tarjetas que representan tareas individuales asignadas a los miembros del equipo, permitiendo un seguimiento claro del progreso y facilitando la colaboración.<br><br>Además, empleamos Google Drive para crear un documento compartido donde todos los miembros del equipo pueden agregar y revisar sus contribuciones. Este documento sirve como la versión central del trabajo, garantizando que todos puedan verificar la precisión y la coherencia de las partes antes de integrarlas en el formato Markdown final para la entrega.<br><br>
**Product UX/UI Design**<ul><li><strong>UXPressia:</strong><br>Se utilizó <a href="https://uxpressia.com/">UXPressia</a> para el desarrollo de los diagramas user personas, user journey mapping, empathy mapping e impact map.</li><li><strong>Color Space:</strong><br>Se utilizó <a href="https://mycolor.space/">Color Space</a> ha apoyado en la selección de la paleta de colores para el desarrollo del diseño de la web.</li><li><strong>Figma:</strong><br>Se ha utilizado <a href="https://www.figma.com/">Figma</a> para el desarrollo de los wireframes y prototipos del landing page y aplicación web, tanto en dispositivos de escritorio como de móvil.</li><li><strong>Miro:</strong><br>Se utilizó <a href="https://miro.com/es/">Miro</a> para el desarrollo de los escenarios mapping y escenario mapping para ambos segmentos objetivos.</li></ul>

**Software Development**<br><ul>
<li><a href="https://code.visualstudio.com/">Visual Studio Code</a>, <a href="https://visualstudio.microsoft.com/es/vs/community/">Visual Studio Code Community</a> e <a href="https://www.jetbrains.com/idea/">IntelliJ IDEA</a> fueron las IDEs que emplearemos para el desarrollo del código del proyecto. Hemos desarrollado el landing page con Visual Studio Code, luego Visual Studio Code Community para el diagrama C4 y emplearemos IntelliJ IDEA para la aplicación web.</li>
  <li><a href="https://github.com/">Github</a> y <a href="https://git-scm.com/downloads">Git bash</a> nos permitirán el control de versiones del código y el desarrollo colaborativo del proyecto.</li>
</ul>

**Software Testing**
<br><br>Para la fase de pruebas, planeamos utilizar [Postman](https://www.postman.com/) como nuestra herramienta principal para la verificación y validación de las API que serán desarrolladas en la etapa de programación. Una vez que el backend esté implementado, realizaremos pruebas manuales de los endpoints para asegurarnos de que las solicitudes (GET, POST, PUT, DELETE) funcionen correctamente y devuelvan las respuestas esperadas.<br><br>
**Software Deployment**<br><br>[Github Pages](https://github.com/) Se utilizó Github Pages para el deploy del landing page.<br>Se ha utilizado [Firebase](https://firebase.google.com/?hl=es) para desplegar el Frontend a través de su funcionalidad de hosting.<br><br>
**Software Documentation**<br><ul>
<li><strong>Google Drive:</strong><br>Se ha utilizado <a href="https://www.google.com/intl/es-419_pe/drive/">Google Drive</a> para subir archivos de documentos y presentación. Además, se han utilizado herramientas como Google Docs y Google Slides que permiten el desarrollo colaborativo de los informes a entregar.</li><li><strong>Google Meets y Zoom:</strong><br>Se ha utilizado <a href="https://meet.google.com/">Google Meets</a> y <a href="https://zoom.us/">Zoom</a> para videoconferencias y realizar las entrevistas de segmentos objetivos. Las plataformas tienen herramientas de grabación, lo que simplifica el procesamiento de los videos.</li><li><strong>Microsoft Stream:</strong><br>Se ha utilizado el servicio de <a href="https://www.microsoft.com/es-ww/microsoft-365/microsoft-stream">Microsoft Stream</a> para subir el video completo de las entrevistas. La cuenta que ha subido el video está vinculada a la organización de la universidad, lo que permitió tener suficiente espacio de memoria en la nube.</li><li><strong>LucidChart:</strong><br><a href="https://www.lucidchart.com/pages/es">LucidChart</a> ha sido empleado en el desarrollo de diagramas de flujo para asegurar los user goals y guiar en el diseño de los prototipos de la aplicación web. Además, se ha utilizado para el diagrama de clases.</li><li><strong>Structurizr:</strong><br>Para el desarrollo del diagrama C4 en los tres niveles (diagrama de contexto, contenedores y componentes), se empleó <a href="https://structurizr.com/">Structurizr</a> junto a Visual Studio Code Community.</li><li><strong>Vertabelo:</strong><br>Para el desarrollo del diagrama del diseño de base de datos, se ha empleado <a href="https://vertabelo.com/">Vertabelo</a>, software especializado en diagramas de base de datos.</li></ul>

#### 5.1.2. Source Code Management
Se ha creado una organización en Github con los miembros del grupo y un repositorio para el landing page.

|Segmento                          |        URL                        |
|--------------------------------- | --------------------------------- |
|Organización|https://github.com/SpeedyRent|
|Repositorio Landing Page|https://github.com/SpeedyRent/Landing-Page |
|Despliegue del Landing Page en Netlify|https://SpeedyRent.netlify.app/|
|Backend| https://github.com/SpeedyRent/SpeedyRent-Backend |
|Frontend | https://github.com/SpeedyRent/SpeedyRent-Frontend |

**GitFlow Implementation**<br>GitFlow es un modelo estructurado para gestionar el desarrollo y las ramas en Git. Las ramas principales en este flujo son develop y main. La rama develop actúa como la principal rama de trabajo donde se integran nuevas características, mientras que la rama main contiene la versión estable y lista para producción, que se despliega en GitHub Pages. Además, se crean ramas adicionales para cada tarea o funcionalidad específica que se esté desarrollando, garantizando un flujo organizado y controlado.
<br><p align="center"><img src="Assets/Chapter-5/5.1.2/gitFlow.png" alt="GitFlow" /></p>
<br><br>**Feature Branches**<br>Cada nueva funcionalidad se desarrolla en su propia rama individual, creada a partir de develop. Estas ramas permiten aislar el trabajo en progreso y facilitan la integración de nuevas características sin interrumpir el desarrollo principal.
<br><p align="center"><img src="Assets/Chapter-5/5.1.2/Feature branches.png" alt="Feature Branches" /></p>
<br><br>**Release Branches**<br>Las ramas de lanzamiento se crean desde develop cuando se prepara una nueva versión para ser enviada a producción. Estas ramas permiten pulir detalles finales antes de fusionar la versión en main y lanzar el producto.
<br><p align="center"><img src="Assets/Chapter-5/5.1.2/release branches.png" alt="Release Branches" /></p>
<br><br>**Hotfix Branches**<br>Las ramas de hotfix se utilizan para solucionar errores críticos que aparecen en producción. Se crean desde main y, una vez resuelto el problema, se fusionan tanto en main como en develop, garantizando que el arreglo esté presente en las futuras versiones de desarrollo.
<br><p align="center"><img src="Assets/Chapter-5/5.1.2/hotfix branches.png" alt="Hotfix Branches" /></p>
<br><br>**Semantic versioning**<br>Los releases se realizan según los estándares de Semantinc Versioning 2.0 (https://semver.org/), según el formato MAJOR.MINOR.PATCH.
<br><br>**• MAJOR:** versión mayor cuando se implementa cambios de APIs incompatibles.
<br>**• MINOR:** versión menor cuando se añaden features y funcionalidades nuevas.
<br>**• PATCH:** versión de parche de bug fixes y hotfixes.
<br><br>**Conventional Commits**<br>En GitHub, se sigue el estándar de commits convencionales versión 1.1.0 (Conventional Commits 1.1.0).<br>Este sistema organiza los mensajes de commit de forma clara y estructurada, facilitando la comprensión y el seguimiento de cambios. La convención se basa en la siguiente estructura:
<br><p align="center"><img src="Assets/Chapter-5/5.1.2/Commit.png" alt="Commit" /></p>
<br><br>**• Type:** Representa el tipo de commit, sea tipo feature (feat), fix (fix) o docs (docs).
<br>**• Optional scope:** Es opcional y representa el alcance del commit.
<br>**• Description:** Descripción detallada del commit y acciones realizadas.

#### 5.1.3. Source Code Style Guide & Conventions
HTML Style Guide and Coding Conventions Es necesario seguir convenciones estandarizadas de HTML como estructura de la web. Entre las principales de W3 Schools (https://www.w3schools.com/html/html5_syntax.asp) podemos mencionar:

● Siempre declarar el tipo de documento con "" ● Usar siempre letras en minúsculas para los nombres de los elementos. ● Cerrar siempre con los elementos de HTML. ● Siempre poner entre comillas los atributos dentro de un elemento html (

) ● Especificar alt, width, and height para imágenes. ● Espaciado y signo igual estandarizados. ● Evitar líneas de código extensas. ● No olvidar el “<title></title>” al principio. ● Es posible evitar el “”. ● Utilizar meta tags al inicio.
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
