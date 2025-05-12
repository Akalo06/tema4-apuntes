
## 🧪 Inicializar un Repositorio Local en Git



En esta actividad, crearemos un repositorio local en nuestro PC personal. Luego, añadiremos y modificaremos algunos archivos y registraremos los cambios, trabajando desde la terminal de texto.

---

### 🔄 Proceso a seguir

1. **Creamos una carpeta para alojar el proyecto**

```bash
mkdir mi-proyecto-git
cd mi-proyecto-git
```

2. **Comprobamos que tenemos la carpeta vacía**

```bash
ls -a
```

3. **Inicializamos el repositorio**

```bash
git init
```

4. **Comprobamos que se ha creado una carpeta `.git`**

```bash
ls -a
```

> Esta carpeta almacena todo el historial del repositorio y los cambios que realicemos.

---

### 📝 Registro de Cambios

5. **Creamos un archivo `README.md`**

```bash
touch README.md
```

6. **Añadimos una línea al archivo**

Editamos el archivo para incluir:





7. **Registramos los cambios en el repositorio**

- Añadir el archivo al área de preparación:

```bash
git add README.md
```

- Confirmar los cambios en el repositorio local:

```bash
git commit -m "Añadir nombre y apellidos"
```

---

### 🔁 Repetimos el proceso dos veces más

**Primera repetición:**

- Añadimos una línea con la fecha actual al archivo `README.md`.

```markdown
Fecha: 12 de mayo de 2025
```

- Guardamos y ejecutamos:

```bash
git add README.md
git commit -m "Añadir fecha actual"
```

**Segunda repetición:**

- Añadimos una línea con el nombre del centro educativo:

```markdown
IES Inca Garcilaso
```

- Guardamos y ejecutamos:

```bash
git add README.md
git commit -m "Añadir nombre del IES"
```

---

### 🔍 Ver los cambios realizados

Podemos revisar el historial de commits con:

```bash
git log --oneline
```

---

> ✅ Este proceso permite entender el flujo básico de trabajo en Git, asegurando un control eficiente sobre las versiones del proyecto.
