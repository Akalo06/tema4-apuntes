1.1 Las 3 Secciones de un Proyecto Git

Git es un sistema de control de versiones distribuido que permite a los desarrolladores
gestionar los cambios en el código fuente de manera eficiente. Un proyecto en Git se
divide en tres secciones principales:

---

1. Directorio de Trabajo (Working Directory)
El directorio de trabajo es la carpeta en la que se encuentran los archivos del proyecto.
Aquí es donde los desarrolladores crean, editan y eliminan archivos antes de
confirmarlos en el repositorio. Es una copia del estado del proyecto en un momento
dado.

• Contiene los archivos actuales del proyecto.
• Los cambios realizados en esta sección aún no están guardados en Git hasta que
se agreguen al área de preparación.
• Se pueden ver los archivos modificados usando el comando git status.

---

2. Área de Preparación (Staging Area)

El área de preparación (también conocida como "index") es donde se colocan los
cambios que están listos para ser confirmados en el repositorio. Permite a los
desarrolladores seleccionar qué modificaciones serán parte del próximo commit.
• Se agregan cambios con el comando git add nombre_del_archivo o git add .
para agregar todos los cambios.
• Se pueden visualizar los archivos en esta área con git status o git diff --staged.
• Permite un mayor control sobre qué cambios se guardarán en la próxima
confirmación.

---

3. Repositorio (Directorio .git)
El repositorio es el almacenamiento donde Git guarda todos los cambios confirmados.
Se encuentra en una carpeta oculta llamada .git dentro del proyecto.
• Almacena el historial de versiones del proyecto.
• Se realiza una confirmación de cambios desde el área de preparación con git
commit -m "Mensaje del commit".
• Permite restaurar versiones anteriores del proyecto y gestionar colaboraciones
mediante sistemas remotos como GitHub o GitLab.
Cada una de estas secciones juega un papel clave en el flujo de trabajo con Git,
permitiendo un control detallado sobre las modificaciones y versiones del código.

---
