
## 🔁 Las 3 Secciones de un Proyecto Git

**Git** es un sistema de control de versiones distribuido que permite a los desarrolladores gestionar los cambios en el código fuente de manera eficiente. Un proyecto en Git se divide en **tres secciones principales**:

---

### 1. 📂 Directorio de Trabajo (Working Directory)

Es la carpeta donde se encuentran los archivos del proyecto. Aquí es donde los desarrolladores crean, editan y eliminan archivos antes de confirmarlos en el repositorio. Representa una copia del estado actual del proyecto.

- Contiene los archivos visibles del proyecto.
- Los cambios realizados aún **no están guardados en Git** hasta que se añadan al área de preparación.
- Para ver los archivos modificados se puede usar:

```bash
git status
```

---

### 2. 📝 Área de Preparación (Staging Area)

También conocida como **index**, esta zona intermedia almacena los cambios que están listos para ser confirmados.

- Los cambios se añaden con:

```bash
git add nombre_del_archivo
```

o

```bash
git add .
```

- Para visualizar los archivos en esta área:

```bash
git status
git diff --staged
```

- Permite un mayor control sobre **qué se incluirá en el siguiente commit**.

---

### 3. 🗃️ Repositorio (Directorio `.git`)

Es una carpeta oculta donde Git guarda todos los cambios confirmados y metadatos del proyecto.

- Almacena el historial completo del proyecto.
- Para confirmar los cambios desde el área de preparación:

```bash
git commit -m "Mensaje del commit"
```

- Permite:
  - Restaurar versiones anteriores.
  - Gestionar colaboraciones mediante plataformas remotas como **GitHub** o **GitLab**.


