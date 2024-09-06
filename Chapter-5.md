## Capítulo V: Product Implementation, Validation & Deployment
### 5.1. Software Configuration Management
#### 5.1.1. Software Development Environment Configuration
En esta sección, detallaremos las plataformas y el software que utilizamos como equipo para el desarrollo y la gestión de nuestro startup. Estas herramientas nos permiten optimizar procesos, colaborar de manera eficiente y asegurar el crecimiento sostenible de nuestro proyecto.<br><br>
**Project Management**<br><br>[Discord](https://discord.com/) y [WhatsApp](https://www.whatsapp.com/?lang=es) han sido los medios principales de comunicación entre los miembros del grupo, donde Discord ha destacado ya que contiene funcionalidades adicionales para organizar grupos de estudio y de trabajo.<br><br>
**Requirements Management**<br><br>Hemos utilizado [Trello](https://trello.com/home) como herramienta principal para la organización y gestión de tareas. En Trello, creamos listas específicas para las etapas del trabajo, como “Entregables”, "Por Hacer", "En Proceso", "Pendiente de Revisión" y "Completado". Cada lista contiene tarjetas que representan tareas individuales asignadas a los miembros del equipo, permitiendo un seguimiento claro del progreso y facilitando la colaboración.<br><br>Además, empleamos Google Drive para crear un documento compartido donde todos los miembros del equipo pueden agregar y revisar sus contribuciones. Este documento sirve como la versión central del trabajo, garantizando que todos puedan verificar la precisión y la coherencia de las partes antes de integrarlas en el formato Markdown final para la entrega.
<br><p align="center"><img src="Assets/Chapter-5/Trello.png" alt="Trello" /></p>
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
<br><br>**Semantic versioning**<br>Los releases se realizan según los estándares de Semantinc Versioning 2.0 (https://semver.org/), según el formato MAJOR.MINOR.PATCH.<br>
- **MAJOR:** Versión mayor cuando se implementa cambios de APIs incompatibles.
- **MINOR:** versión menor cuando se añaden features y funcionalidades nuevas.
- **PATCH:** versión de parche de bug fixes y hotfixes.<br>

**Conventional Commits**<br>En GitHub, se sigue el estándar de commits convencionales versión 1.1.0 (Conventional Commits 1.1.0).<br>Este sistema organiza los mensajes de commit de forma clara y estructurada, facilitando la comprensión y el seguimiento de cambios. La convención se basa en la siguiente estructura:
<br><p align="center"><img src="Assets/Chapter-5/5.1.2/Commit.png" alt="Commit" /></p>
- **Type:** Representa el tipo de commit, sea tipo feature (feat), fix (fix) o docs (docs).
- **Optional scope:** Es opcional y representa el alcance del commit.
- **Description:** Descripción detallada del commit y acciones realizadas.

#### 5.1.3. Source Code Style Guide & Conventions
Como convención general , todo el codigo realizado por los miembros del equipo debe redactarse en completo inglés.
<br><br>**HTML**<br>
- **Use Lowercase Element Name**<br>
Se recomienda usar lowercase para los nombres de los elementos HTML:<br>
<br><p align="center"><img src="Assets/Chapter-5/5.1.3/Lowercase.png" alt="Lowercase Element Name" /></p><br>
- **Close All HTML Elements**<br>
Se recomienda cerrar todos los elementos HTML:<br>
<br><p align="center"><img src="Assets/Chapter-5/5.1.3/close all html.png" alt="Close all html" /></p><br>
- **Use Lowercase Attribute Names**<br>
Se recomienda usar lowercase para los nombres de los atributos HTML:<br>
<br><p align="center"><img src="Assets/Chapter-5/5.1.3/attribute names.png" alt="attribute Names" /></p><br>
- **Always Specify alt, width, and height for Images**<br>
Se recomienda seguir estas convenciones en caso de que la imagen no se puede mostrar y ayudar con la accesibilidad del contenido:<br>
<br><p align="center"><img src="Assets/Chapter-5/5.1.3/always images.png" alt="always images" /></p>
<br>Para mas información sobre las convenciones de HTML: https://www.w3schools.com/html/html5_syntax.asp

<br>**CSS**<br><br>
- **ID and Class Naming**<br>
Usar nombres de clases y ID significativos que expresen el propósito del elemento:<br>
<br><p align="center"><img src="Assets/Chapter-5/5.1.3/Id and class naming.png" alt="class naming" /></p><br>
- **Block Content Identation**<br>
Sangrar todo el contenido del bloque, es decir, reglas dentro de reglas, así como declaraciones, para reflejar la jerarquía y Mejorar la comprensión<br>
<br><p align="center"><img src="Assets/Chapter-5/5.1.3/Block Content Identation.png" alt="content identation" /></p><br>
- **Section Comments**<br>
Agrupe las secciones de la hoja de estilo mediante comentarios. Separar secciones con nuevas líneas.<br>
<br><p align="center"><img src="Assets/Chapter-5/5.1.3/Section Comments.png" alt="Comments" /></p>
<br>Para mas informacion sobre las convenciones de CSS: https://google.github.io/styleguide/htmlcssguide.html

<br>**JavaScript**<br><br>
- **Array initializers: can be "block-like"**<br>
Cualquier inicializador de matriz puede ser formateado opcionalmente como si fuera un "tipo bloque" construir". Por ejemplo, los siguientes son todos válidos (no es un análisis exhaustivo lista):<br>
<br><p align="center"><img src="Assets/Chapter-5/5.1.3/block-like.png" alt="block like" /></p><br>
- **Type-use annotations**<br>
Las anotaciones de uso de tipo aparecen inmediatamente antes del tipo anotado. Una anotación es un uso de tipo anotación si está meta-anotado con . Ejemplo:@Target(ElementType.TYPE_USE)<br>
<br><p align="center"><img src="Assets/Chapter-5/5.1.3/Type-use annotations.png" alt="type-use annotations" /></p><br>
- **Method and constructor annotations**<br>
Las reglas para las anotaciones en las declaraciones de método y constructor son las mismas que en la sección anterior. Ejemplo:<br>
<br><p align="center"><img src="Assets/Chapter-5/5.1.3/Method and constructor annotations.png" alt="method" /></p>
<br>Para mas informacion sobre las convenciones de JavaScript: https://google.github.io/styleguide/javaguide.html

<br>**TypeScript**<br><br>
- **Imports**<br>
Hay cuatro variantes de instrucciones de importación en ES6 y TypeScript:<br>
<br><p align="center"><img src="Assets/Chapter-5/5.1.3/imports.png" alt="imports" /></p><br>
- **Class declarations**<br>
Las declaraciones de clase no deben terminar con punto y coma:<br>
<br><p align="center"><img src="Assets/Chapter-5/5.1.3/Class declarations.png" alt="Class declarations" /></p><br>
- **Constructors**<br>
Las llamadas al constructor deben usar paréntesis, incluso cuando no se pasa ningún argumento:<br>
<br><p align="center"><img src="Assets/Chapter-5/5.1.3/Constructores.png" alt="constructor" /></p>
<br>Para mas informacion sobre las convenciones de TypeScript: https://google.github.io/styleguide/tsguide.html

<br>**Gherkin**<br><br>
- **Discernible Given-When-Then Blocks**<br>
En teoría, sus escenarios pueden ser tan simples como un solo paso Given, When Then, cada uno. Sin embargo, en la vida real, tienden a crecer y tienen múltiples pasos para cada una de estas palabras clave. Para detectar rápidamente dónde termina un bloque y comienza otro, puede sangrar los pasos que comienzan con "Y". Entonces, el escenario sería algo así:<br>
<br><p align="center"><img src="Assets/Chapter-5/5.1.3/Discernible given when.png" alt="Discernible" /></p><br>
Una alternativa es hacer que cada paso comience con la misma sangría y agregar una nueva línea adicional antes del siguiente bloque de palabras clave.<br><br>
- **Steps with Tables**<br>
A menudo usamos tablas en nuestros pasos. Para que sea inmediatamente reconocible que un paso necesita más información de una tabla, usamos dos puntos al final del paso. Esto ayuda cuando se usa IntelliSense, que no incluye vistas previas de tablas, pero mostrará los dos puntos:<br>
<br><p align="center"><img src="Assets/Chapter-5/5.1.3/Steps with Tables.png" alt="tables" /></p><br>
- **Reducing Noise**<br>
Para reducir el ruido, se recomienda utilizar valores predeterminados para los campos que el sistema requiere, pero que no son relevantes para su escenario.<br>
<br><p align="center"><img src="Assets/Chapter-5/5.1.3/Reducing Noise.png" alt="noise" /></p><br>
Para mas informacion sobre las convenciones de Gherkin: https://specflow.org/gherkin/gherkin-conventions-for-readable-specifications/

#### 5.1.4. Software Deployment Configuration
Se utilizará el servicio de [Netlify](https://www.netlify.com/) para realizar el proceso de deployment del landing page de SpeedyRent.<br>A continuación se presentará el proceso para realizarlo:

1. Crear o tener una cuenta de Netlify ingresando a su página web oficial.<br>Esta cuenta se puede crear con Github, Gitlab o Bitbucket o con un correo convencional.<br><br>
2. Una vez con la sesión iniciado, dirigirse a la sección de sitios y seleccionar “Import from Git”<br><br>
3. Seleccionamos la opción de GitHub<br><br>
4. Seleccionamos la organización con el repositorio a deployar.<br><br>
5. Seleccionamos el repositorio y luego nos aparecerá el botón “Deploy Site” al final del formulario.<br>De esta manera, la página ya estaría deployada en unos instantes.<br>Link de deployment: https://SpeedyRent.netlify.app/ 

### 5.2. Landing Page, Services & Applications Implementation
#### 5.2.1. Sprint 1

## Sprint #1
##### 5.2.1.1 Sprint Planning 1

### Sprint Planning Background
Para este primer sprint nos enfocaremos en los tasks para la
elaboración de la Landing Page. Nos dividiremos entre nosotros cada
una de las tareas identificadas para el sprint.
<table>
<tr>
    <th colspan="5">Sprint #</th>
    <th colspan="9">Sprint 1</th>
  </tr>
      <tr>
    <td colspan="13">Sprint Planning Background</td>
  </tr>
  <tr>
    <td colspan="5">Date</td>
    <td colspan="8">2024-08-19</td>
</tr>
  <tr>
    <td colspan="5">Time</td>
    <td colspan="8">11:30 PM</td>
  </tr>
  <tr>
    <td colspan="5">Location</td>
    <td colspan="8">Via Discord y Google Meet</td>
<tr>
    <td colspan="5">Prepared By</td>
    <td colspan="8">George</td>
</tr>
<tr>
    <td colspan="5">Attendees (to planning meeting)</td>
    <td colspan="8">George, Fabiola Dayane Becerra Llempen,Samuel Ignacio Valera Garces,Maria Fernanda Fernandez Alva,Paolo Eduardo Belleza Tello, Fiorella </td>
</tr>
<tr>
    <td colspan="5">Sprint n – 1 Review Summary</td>
    <td colspan="8">En esta seccion se planteo el desarrollo del landing page para nuestro proyecto llamado SpeedyRent y la reparticion de partes de caracter individual para esta primera entrega</td>
</tr>
<tr>
    <td colspan="5">Sprint n – 1 Retrospective Summary</td>
    <td colspan="8">En esta seccion todos los integrantes mencionaron tener aciertos en las respectivas partes que le correspondia cada uno para esta primera entrega</td>
</tr>
<tr>
    <td colspan="13">Sprint Goal & User Stories</td>
</tr>
<tr>
    <td colspan="5">Sprint n Goal</td>
    <td colspan="8">Culminar el landing Page e Informe</td>
</tr>
<tr>
    <td colspan="5">Sprint n Velocity</td>
    <td colspan="8">6 story points</td>
</tr>
<tr>
    <td colspan="5">Sum of Story Points</td>
    <td colspan="8">9 Story Points</td>
</tr>
</table>

##### 5.2.1.2 Sprint Backlog 1
##### 5.2.1.3 Development Evidence for Sprint Review
##### 5.2.1.4 Testing Suite Evidence for Sprint Review
##### 5.2.1.5 Execution Evidence for Sprint Review
Para esta primera entrega, nuestro equipo a conseguido elaborar la Landing Page del proyecto "LexMed". De tal modo, se podrá visualizar la información necesaria de lo que ofrece nuestro proyecto.

**Sección de inicio**: Se implementó el Header de nuestra Landing Page.
![alt text](../docs/images/inicio.png)
**Sección de Nosotros**: Se implementó la sección de nosotros para describir un poco sobre quienes somos.
![alt text](../docs/images/about.png)
**Sección de Servicios**: Se implementó la sección de los servicios ofrecidos.
![alt text](../docs/images/services.png)
**Sección de Planes**: Se implementó la sección de ver los tipos de suscripción.
![alt text](../docs/images/plans.png) 
**Sección de contacto y creadores**: Se añadió la sección de contacto para facilitar la comunicación con los usuarios y la información de los creadores.
![alt text](../docs/images/contact.png)
##### 5.2.1.6 Services Documentation Evidence for Sprint Review
En este sprint solo se trabajó el landing page.
##### 5.2.1.7 Software Deployment Evidence for Sprint Review

Para el despliegue del Landing Page, hemos utilizado la herramienta de Github Pages para poder hacer un deployment. Para eso, hemos creado un repositorio donde hemos colocado el código de desarrollo de nuestra Landing Page.

![alt text](../docs/images/Soft%20deploy%20landing.png)

Una vez creado el repositorio, entraremos a configuración del repositorio y escogemos el apartado de Pages. Se coloca la información necesaria, como la fuente del branch a utilizar para realizar el deployment. Luego de eso, Github Pages nos brindará el link y desplegará nuestra landing page en la Web.

![alt text](../docs/images/deploy%20landing.png)

##### 5.2.1.8 Team Collaboration Insights during Sprint

Para el desarrollo de este primer sprint, todos los miembros del equipo desarrollaron y colaboraron de manera activa y continua. De tal modo, se muestra como evidencia los insights de cada miembro del equipo.

Commits:

![alt text](../docs/images/commits.png)

Analiticas de Colaboración:

![alt text](../docs/images/contributors.png)
