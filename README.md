# commit-daw-2026
Portal del Evento Tech
Esta práctica se realizará en equipos de 5 personas.
ENUNCIADO:
Vuestra agencia de desarrollo ha recibido el encargo de crear el sitio web oficial para la
conferencia tecnológica “Commit DAW 2026”.
El cliente solicita un sitio web multi-página de mínimo 5 secciones, con un diseño
moderno y totalmente adaptable a dispositivos móviles (responsive). Dado que el plazo
de entrega es corto, trabajaréis 5 desarrolladores en paralelo sobre el mismo repositorio,
lo que exige una coordinación estricta y una gestión avanzada de ramas y conflictos.
ARQUITECTURA DEL SITIO WEB:
El sitio constará de 5 páginas HTML. Todas deben compartir el mismo diseño base, con
Header/Menú y Footer, y hoja de estilos.
1. Index.html: portada con imagen de fondo, título, fechas y resumen visual de las
secciones.
2. Speakers.html: grid con fotos, nombres y biografías de los conferenciantes.
3. Agenda.html: tabla con horarios, salas y títulos de las charlas.
4. Location.html: información de la sede, mapa (imagen o iframe) y cómo llegar.
5. Ticket.html: formulario de inscripción (nombre, email, tipo de entrada) validado y
tabla de precios.
REQUISITOS TÉCNICOS
• HTML5 semántico: uso correcto de etiquetas (header, nav, main, section, footer).
• CSS3 & Responsive:
o Uso de Flexbox y CSS Grid.
o Media Queries (@media): la web debe cambiar su distribución al verse en
móvil (ej: el menú se simplifica, las columnas de ponentes pasan de 3 a 1).
• Gitflow:
o Rama main: solo para producción (versiones finales).
o Rama develop: rama de integración (aquí se unen los trabajos).
o Ramas feature/nombre-tarea: donde trabaja cada desarrollador.
• Gestión: uso obligatorio de GitHub Projects (Kanban) con columnas: ToDo, In
Progress, Review, Done.
• No se pueden mergear PRs sin mínimo un “Aprove” de un “Reviewer”.
ROLES DEL EQUIPO
Una persona puede tener vario roles pero todos deben programar.
• Repo Owner: crea el repositorio, configura los colaboradores y crea la estructura
inicial.
• Scrum Master: mantiene actualizado el tablero Kanban y asigna las tareas
(issues).
• Release Manager: único responsable de hacer los merges a la rama main y
desplegar la web.
• Developers: todos los miembros pican código en sus respectivas ramas.
Para el tablero Kanban utilizaremos la herramienta nativa GitHub Projects.
1. Id a la pestaña Projects del repo -> New Project -> Select Board.
2. Las tareas se crean desde la pestaña Issues. Al crear una Issue, asignadla a un
compañero (Assignees) y vinculadla al proyecto (Projects) en el menú lateral
derecho.
GUÍA DE TRABAJO
CONFIGURACIÓN Y REPARTO
1. GitHub Projects: Cread un tablero y generad las tareas (issues): una por cada
página HTML y tareas extra de diseño. Asignad una página a cada miembro.
2. Repositorio:
a. Cread el repo público o privado y añadid a los colaboradores y a mi
(silvia987654).
b. Subid el index.html base (esqueleto vacío) y style.css (con variables de
colores) a main.
c. Cread la rama develop desde main.
3. Inicio: cada miembro clona el repo, hace “git checkout develop” y crea su rama
feature/su-pagina.
DESARROLLO PARALELO
1. Cada persona desarrolla su página HTML (agenda.html, etc.) y añade estilos en el
CSS compartido.
2. Aseguraos de copiar el bloque del <nav> (menú) y <footer> en vuestra página para
mantener la coherencia.
3. Haced commits pequeños y frecuentes.
4. Subid cambios a vuestra rama y haced Pull Requests (PR) hacia develop conforme
avancéis.
SIMULACIÓN DE CONFLICTO
Al llegar a esta fase, cada uno tiene su página, pero el menú de navegación no tiene los
enlaces a las páginas de los compañeros.
1. Acción coordinada: los 5 miembros debéis editar el archivo index.html (o el
bloque de navegación común) al mismo tiempo.
2. Cada uno añadirá el enlace <li><a href="...">Mi Página</a></li> en la lista del
menú.
3. Intentad hacer Commit y Push a la vez hacia develop, o mergear vuestras PRs
simultáneamente.
4. Se generará un conflicto de Git. Debéis resolverlo en equipo, decidiendo el orden
de los enlaces, limpiar el código de marcas <<<< HEAD y hacer un nuevo commit.
INTEGRACIÓN Y RESPONSIVE
1. Una vez arreglado el menú en develop, todos debéis hacer “git pull origin develop”
para bajar el menú corregido.
2. Copiad ese menú final en vuestras páginas individuales.
3. Revisad el archivo style.css: ¿Hay conflictos de estilos? Unificadlos.
4. Comprobad que la web se ve bien en modo "Inspeccionar -> Móvil" del navegador.
ENTREGA Y DESPLIEGUE
1. Cuando todo funcione en develop, el Release Manager crea un Pull Request hacia
main.
2. Se revisa y se acepta el merge en main.
3. Activad GitHub Pages (desde Settings -> Pages) apuntando a la rama main / root.
ENTREGA
1. Integrantes junto con sus roles.
2. Enlace al repositorio.
3. Enlace de la Web.
4. Captura Kanban.
5. Captura Network Graph.
6. Captura de la resolución de los conflictos que puedan aparecer, mínimo uno.
