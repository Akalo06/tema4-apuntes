
# 📄 Documentación con Javadoc en Java

## ✍️ Uso de comentarios estructurados en Java

Javadoc utiliza comentarios especiales para generar documentación HTML a partir del código fuente de Java. Estos comentarios se escriben con el formato `/** ... */` y se colocan justo encima de clases, interfaces, constructores, métodos o atributos.

### 🔹 Estructura básica de un comentario Javadoc

```java
/**
 * Descripción general de la clase o método.
 * @author Nombre del autor
 * @version Versión del código
 * @param nombre Descripción del parámetro (si es un método)
 * @return Descripción del valor devuelto (si es un método)
 * @throws Excepción Descripción de la excepción lanzada (si aplica)
 */
```

### 🔹 Etiquetas más comunes

- `@author`: Autor del código.
- `@version`: Número o nombre de versión.
- `@param`: Describe un parámetro del método.
- `@return`: Explica lo que devuelve el método.
- `@throws` o `@exception`: Indica qué excepciones puede lanzar el método.
- `@see`: Enlaces a otros elementos relacionados.
- `@since`: Desde qué versión está disponible el elemento.
- `@deprecated`: Indica que el elemento está obsoleto.

---

## ⚙️ Generación de documentación con `javadoc`

El comando `javadoc` permite generar documentación HTML a partir del código Java con comentarios estructurados.

### 🔹 Uso básico del comando

```bash
javadoc -d doc NombreDelArchivo.java
```

- `-d doc`: Indica el directorio de salida (en este caso `doc/`).
- `NombreDelArchivo.java`: Es el archivo fuente que contiene comentarios Javadoc.

### 🔹 Opciones adicionales útiles

- `-author`: Incluye la etiqueta `@author`.
- `-version`: Incluye la etiqueta `@version`.
- `-private`: Muestra también miembros privados en la documentación.
- `-classpath`: Permite especificar la ruta de clases dependientes.

---

## 🛠️ Herramientas y buenas prácticas

### 🔹 Herramientas complementarias

- **IDEs como IntelliJ IDEA o Eclipse**: Generan automáticamente los bloques de comentarios Javadoc.
- **Checkstyle / SonarLint**: Herramientas que pueden validar la calidad de los comentarios.

### 🔹 Buenas prácticas

- Escribir descripciones claras y concisas.
- Documentar todas las clases públicas y sus métodos.
- Usar etiquetas adecuadas para describir entradas y salidas.
- Mantener la documentación actualizada con el código.
- Evitar comentarios innecesarios o redundantes.

---

## 📚 Ejemplo completo

```java
/**
 * Clase que representa una persona.
 * @author Manuel
 * @version 1.0
 */
public class Persona {
    private String nombre;
    private int edad;

    /**
     * Constructor de la clase Persona.
     * @param nombre Nombre de la persona
     * @param edad Edad de la persona
     */
    public Persona(String nombre, int edad) {
        this.nombre = nombre;
        this.edad = edad;
    }

    /**
     * Obtiene el nombre de la persona.
     * @return Nombre
     */
    public String getNombre() {
        return nombre;
    }

    /**
     * Establece el nombre de la persona.
     * @param nombre Nuevo nombre
     */
    public void setNombre(String nombre) {
        this.nombre = nombre;
    }
}
```
---

![captura de javadoc1](./capturas/1javadoc.png)
![captura de javadoc2](./capturas/2javadoc.png)
![captura de javadoc3](./capturas/3javadoc.png)

---

✅ Con estos apuntes, puedes empezar a documentar de forma profesional tus proyectos Java usando Javadoc.
