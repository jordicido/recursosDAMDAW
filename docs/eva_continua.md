# EVALUACIÓN CONTINUA DAM/DAW - 1ª ENTREGA

La **Evaluación Continua** es una opción voluntaria para el alumnado que busca distribuir el esfuerzo a lo largo del curso. Esta modalidad aportará un 40% de la calificación final del módulo.
La primera entrega de actividades está prevista para principios de septiembre; la fecha exacta será confirmada próximamente.

## ☕ Proyecto 1 Programacion: Gestión de Clientes para un Negocio

<u>Fecha de entrega máxima</u>: PENDIENTE (Inicio Septiembre - Fecha por determinar aún)

- 📄 [**PDF Proyecto Java**](https://drive.google.com/file/d/1aFklNGRnEcgMVphxF-FxWJMZGCPLCzRv/view) - Documento PDF del Proyecto 1

---

<u>**TÍTULO DEL PROYECTO**</u>

_Ejemplo: Sistema de Gestión para una Pajarería_

<u>**Entidades y clases** _(ejemplo)_</u>

1. Cliente

```java
public class Cliente {
    private String
            nombre; private
    String dni; private
    String telefono;
    private String
            email;
    // Constructor, getters y setters
}
```

2. Pájaro (lo que se vende)

```java
public class Pajaro {
    private String
            especie; private
    String color; private
    double precio;
    // Constructor, getters y setters
}
```

3. Venta

```java
public class Venta {
    private Cliente
            cliente;
    private ArrayList<Pajaro> lineasDeVenta; // cada venta contiene
    varios pájaros private String fecha;
    // Constructor, método para añadir pájaros, calcular total, etc.
}
```

<u>**Funcionalidades obligatorias del sistema**</u>

| GESTIÓN DE CLIENTES | GESTIÓN DE PÁJAROS (productos)           | GESTIÓN DE VENTAS                                                                                                                                        |
| :------------------ | :--------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1 Alta de clientes  | 1 Alta de pájaros disponibles (catálogo) | 1 Crear nueva venta: <br>&nbsp;&nbsp;&nbsp;&nbsp;1.1 Seleccionar cliente <br>&nbsp;&nbsp;&nbsp;&nbsp;1.2 Añadir uno o más pájaros de la lista disponible |
| 2 Baja              | 2 Listado del catálogo                   | 2 Mostrar todas las ventas realizadas                                                                                                                    |
| 3 Modificación      | 3 Búsqueda por especie                   | 3 Mostrar ventas por cliente                                                                                                                             |
| 4 Búsqueda por DNI  |                                          | 4 Mostrar importe total de cada venta                                                                                                                    |
| 5 Listado           |                                          |                                                                                                                                                          |

<u>**Estructura del menú principal**</u>

```
=== MENÚ PRINCIPAL ===
1. Gestión de clientes
2. Gestión de pájaros
3. Realizar venta
4. Mostrar ventas
5. Salir
```

Cada opción abre un submenú con sus propias opciones (alta, baja, listado...).

<u>**Conceptos que se evalúan**</u>

| Tema                      | Evaluación                                            |
| :------------------------ | :---------------------------------------------------- |
| Variables, entrada/salida | Captura y validación de datos                         |
| Estructuras de control    | Menús, búsquedas, selección                           |
| Clases y objetos          | Cliente, Pajaro, Venta                                |
| Colecciones (ArrayList)   | Listas de clientes, productos y líneas de venta       |
| Funciones (static)        | Métodos organizados por funcionalidad                 |
| Relaciones entre objetos  | Una venta está asociada a un cliente y varios pájaros |
| Modularidad y claridad    | Separación por métodos y clases                       |

<u>**Evaluación**</u>

| Criterio                                | Puntos |
| :-------------------------------------- | :----- |
| Correcta gestión de clases y relaciones | 3      |
| Menús y lógica funcional                | 2      |
| Uso de listas (ArrayList) correctamente | 2      |
| Separación del código en funciones      | 1      |
| Validaciones y claridad del código      | 1      |
| Buenas prácticas y organización         | 1      |
| **Total**                               | **10** |

<u>**Extras opcionales** _(para subir nota)_</u>

- Mostrar importe total de ventas por cliente
- Gestión de stock (disminuir cantidad de pájaros disponibles al vender)
- Ordenar clientes o pájaros por campos (por nombre, especie, etc.)

---

## 🖥️ Proyecto 1 Lenguaje de Marcas: Sitio web responsive

<u>Fecha de entrega máxima</u>: 1 de septiembre a las 23:59

- 📚 [**PDF Proyecto 1 Lenguaje de Marcas**](https://drive.google.com/drive/folders/1tX0kKLEfBH9th5pZi_s4y0Dru68gxVYL)
- 📚 [**PDF Memoria Proyecto 1 Lenguaje de Marcas**](https://docs.google.com/document/d/15HnSuzQCUhGg9k8H6D9BY0ri7_GtCwHZ/edit)

---

**<u>Descripción general</u>**

Esta práctica consiste en el desarrollo de un sitio web de tipo portfolio personal.
La finalidad es que este proyecto no solo sirva como actividad de evaluación, sino
también como una herramienta personal y profesional que puedas utilizar en el
futuro para presentar tu perfil, tus trabajos y tus habilidades.

Esta práctica contará un 28% para la nota total de la evaluación continua. Faltando el otro 12% que será la 2o práctica (28%+12% = 40%).

**<u>Objetivo principal</u>**

El objetivo de la práctica es que diseñes y desarrolles un sitio web responsive,
utilizando HTML5 y CSS3. El uso de JavaScript será opcional, excepto para ciertas
funcionalidades como el menú en dispositivos móviles o la gestión de cookies,
estos casos si será obligatorio.

**<u>Requisitos técnicos</u>**

<!-- prettier-ignore-start -->

- Tecnologías obligatorias:
    - HTML5 y CSS3.
    - Técnicas responsive: puedes usar media queries, Flexbox, Grid, Bootstrap, o combinarlas.
    - Uso de JavaScript para:
        - Menú responsive.
        - Popup de cookies.
        - (Otros usos no serán puntuables, pero pueden sumar en originalidad).
- Diseño previo obligatorio:
    - Boceto mínimo realizado en Figma.
    - Debes realizar dos versiones: escritorio y móvil.
- Tipografías:
    - Mínimo dos tipografías diferentes, cargadas de forma local (no desde Google Fonts ni fuentes externas).
- Repositorio Git:
  - Obligatorio crear un repositorio desde el inicio del trabajo.
    - El repositorio debe estar alojado en GitHub.
    - Se debe ver actividad clara de trabajo con commits progresivos.
    - Puedes usar herramientas como:
        - SourceTree
        - Git desde terminal
        - Git integrado en Visual Studio Code
- Legalidad y buenas prácticas:
    - Implementación obligatoria de un popup de cookies.
    - Página o sección con textos simulados de política de privacidad de datos.
    - Todas las imágenes utilizadas deben estar libres de derechos (de sitios como Unsplash, Pexels, Pixabay, etc.).

<!-- prettier-ignore-end -->

**<u>Requisitos del contenido de una web tipo portfolio</u>**

El portfolio debe incluir como mínimo:

1. Página de inicio con una breve presentación.
2. Sección de proyectos: al menos 3 proyectos (pueden ser ficticios, pero
   deben tener descripción e imagen representativa).
3. Currículum: breve resumen formativo y profesional.
4. Contacto: formulario funcional o una dirección de email visible.
5. Blog o sección de intereses personales (opcional pero recomendado).
6. Diseño adaptado a móvil y escritorio.

**<u>Requisitos de entrega</u>**

<!-- prettier-ignore-start -->

Junto con la entrega del proyecto, es obligatorio presentar una memoria en formato PDF utilizando la plantilla proporcionada. Esta memoria debe incluir los siguientes apartados:

- <u>Capturas del diseño en Figma</u>: Bocetos para versión escritorio y versión móvil.
- <u>Enlace al repositorio de GitHub</u>: Debe ser público y mostrar un historial de trabajo progresivo.
- <u>Enlace al sitio web publicado en un hosting gratuito</u>: Puedes usar servicios como GitHub Pages, Netlify, Vercel, entre otros.
- <u>Complicaciones encontradas y soluciones aplicadas</u>: Explica al menos dos problemas reales surgidos durante el desarrollo y cómo los resolviste.
- <u>Tipografías utilizadas</u>: Especifica el nombre de cada fuente utilizada y su origen (recordatorio: deben estar cargadas localmente y libres de derechos).
- <u>Plan de pruebas</u>:
    - Detalla un plan básico de pruebas que hayas realizado para validar el correcto funcionamiento de la web.
    - Incluye pruebas como:
        - Visualización en distintos tamaños de pantalla (responsive).
        - Funcionamiento de enlaces y formularios.
        - Visualización en varios navegadores (Chrome, Firefox, etc.).
        - Funcionamiento del menú y del popup de cookies.
        - Carga correcta de fuentes e imágenes.

<!-- prettier-ignore-end -->

| Criterio                                                | Puntos | Descripción detalla de la puntuación                                                                                                                                          |
| :------------------------------------------------------ | :----- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Estructura y uso correcto de HTML5 y CSS3               | 2      | 2 pts: HTML y CSS bien estructurados, semánticos, sin errores.<br>1 pt: estructura básica pero errores leves.<br>0 pt: uso incorrecto, desordenado o incompleto.              |
| Diseño responsive funcional (mínimo en 2 resoluciones)  | 2      | 2 pts: correcta adaptación a móvil y escritorio, sin fallos. <br>1 pt: adaptación parcial, errores en algún dispositivo.<br>0 pt: no es responsive.                           |
| Boceto previo en Figma (escritorio + móvil)             | 2      | 1 pt: se incluyen ambos bocetos y capturas claras.<br>0.5 pts: solo un boceto o capturas incompletas.<br>0 pt: no se entrega diseño en Figma.                                 |
| Tipografías locales (mínimo 2)                          | 0.50   | 0.5 pt: se usan dos fuentes distintas y están cargadas localmente.<br>0 pt: no se usan o no son locales.                                                                      |
| Repositorio Git en GitHub (uso correcto)                | 1      | 1 pt: repositorio creado desde el inicio, con commits progresivos.<br>0.5 pts: pocos commits o repositorio mal estructurado.<br>0 pt: no se usa Git/GitHub.                   |
| JavaScript para menú responsive y cookies               | 1      | 1 pt: funcionalidad correcta del menú móvil y popup de cookies.<br>0.5 pts: uno de los dos funciona.<br>0 pt: ninguna funcionalidad presente.                                 |
| Política de privacidad simulada                         | 0.50   | 0.5 pt: texto simulado claro, accesible desde algún lugar del sitio.<br>0 pt: no está presente.                                                                               |
| Calidad del diseño visual y experiencia de usuario (UX) | 2      | 2 pts: diseño cuidado, navegación clara, estética coherente.<br> 1 pt: diseño aceptable pero con fallos visuales o de estructura.<br>0 pt: diseño pobre, caótico o inacabado. |

---

## 💾 Proyecto 1 Bases de Datos

<u>Fecha de entrega máxima</u>: PENDIENTE

- 📄 [Proyecto BBDD] - En desarrollo

---

## ⚙️ Proyecto 1 Entornos de Desarrollo: Profesionaliza tu proyecto Java

<u>Fecha de entrega máxima</u>: PENDIENTE (Inicio Septiembre - Fecha por determinar aún)

- 📄 [**Enlace al repositorio de Jordi**](https://jordicido.github.io/jordicido-fp/MPO/proyecto1/) - MD del Proyecto 1

---

<u>**Título del Proyecto**</u>

_Profesionaliza tu proyecto Java_

<u>**Objetivo del proyecto**</u>

Aplicar herramientas y prácticas profesionales del desarrollo de software sobre un proyecto Java ya desarrollado en el módulo de Programación o uno que yo os proveeré. El objetivo no es modificar la funcionalidad, sino estructurar, documentar, versionar y testear el proyecto como si fuera software profesional.

<u>**Tareas a realizar**</u>

Tu trabajo consistirá en preparar el entorno del proyecto Java aplicando los siguientes aspectos:

<!-- prettier-ignore-start -->

1. Control de versiones con Git

    - Crear un repositorio en GitHub (puede ser privado o público, aunque si es privado deberás invitarme al mismo).
    - Subir correctamente el proyecto Java al repositorio, con estructura clara:

    ```java
    /src/
    /test/
    /docs/
    README.md
    ```

    - Aplicar una estrategia de ramas, como mínimo:

        - main: versión estable.
        - dev: desarrollo activo.
        - feature/<nombre>: ramas para mejoras o tareas.

    - Realizar al menos 5 commits significativos con mensajes descriptivos (no usar "subida", "commit 1", etc.).
    - Crear un .gitignore que excluya archivos de compilación, temporales o IDEs.

2. README.md en Markdown

    - Crear un archivo README.md en la raíz del repositorio con:

        - Nombre del proyecto.
        - Breve descripción funcional.
        - Requisitos para compilar y ejecutar.
        - Instrucciones de uso.
        - Autoría y licencia.

3. Documentación técnica con Javadoc

    - Comentar las clases y sus métodos públicos usando la sintaxis estándar de Javadoc:

    ```java
    /**
    * Representa un producto en el inventario.
    * @author Nombre
    * @version 1.0
    */
    public class Producto {
        /**
        * Devuelve el precio con IVA.
        * @return precio final
        */
        public double calcularPrecioFinal() { ... }
    }
    ```

    - Generar la documentación HTML con Javadoc y colocarla en la carpeta /docs/.

4. Testing automático con JUnit

- Añadir al proyecto al menos 2 clases de test JUnit en el paquete /test.
- Crear métodos de prueba para comprobar el funcionamiento de los métodos principales (casos positivos y negativos).
- Usar anotaciones como @Test, @BeforeEach, @AfterEach.

Ejemplo básico:

```java
@Test
void testCalcularPrecio() {
    Producto p = new Producto("Pan", 1.0, 10);
    assertEquals(1.1, p.calcularPrecioFinal(), 0.01);
}
```

5. Gestión de dependencias con Maven o Gradle

    - Convertir el proyecto Java en un proyecto gestionado por Maven o Gradle:
        - Si usas Maven, incluir un pom.xml.
        - Si usas Gradle, incluir un build.gradle.
    - Declarar como mínimo las dependencias necesarias para:
        - JUnit 5.
        - Cualquier otra librería adicional que uses (opcional).

<u>Entregables</u>

- Enlace al repositorio con:
    - Estructura clara de carpetas.
    - README.md completo.
    - Código Java documentado con Javadoc.
    - Estructura de proyecto con Maven o Gradle.
    - Carpeta docs/ con la documentación HTML generada.
    - Carpeta test/ con pruebas JUnit funcionales.
    - Historial de commits y ramas en Git.

<!-- prettier-ignore-end -->

<u>**Rúbrica de evaluación (EDD)**</u>

| Criterio                                         | Puntos |
| :----------------------------------------------- | :----- |
| Uso correcto de Git y estructura del repositorio | 2      |
| Commits claros y estrategia de ramas             | 2      |
| README en Markdown bien elaborado                | 1      |
| Documentación con Javadoc y carpeta /docs/       | 1      |
| Pruebas unitarias con JUnit                      | 2      |
| Configuración de Maven o Gradle funcional        | 2      |
| **Total**                                        | **10** |

---

## 🐍 Proyecto 1 MPO | Python: Generador de Cuestionarios Interactivo

<u>Fecha de entrega máxima</u>: PENDIENTE (Inicio Septiembre - Fecha por determinar aún)

- 📄 [**Enlace al repositorio de Jordi**](https://jordicido.github.io/jordicido-fp/MPO/proyecto1/) - MD del Proyecto 1

---

<u>**Título del Proyecto**</u>

_Generador de Cuestionarios Interactivo_

<u>**Objetivo del proyecto**</u>

Desarrollar una aplicación de consola en Python que permita realizar cuestionarios tipo test. El usuario podrá responder a una serie de preguntas, y el programa corregirá automáticamente las respuestas, mostrando la puntuación obtenida al finalizar.

<u>**Requisitos funcionales mínimos**</u>

Tu aplicación deberá permitir:

<!-- prettier-ignore-start -->

1. Implementar un menú que se ejecute indefinidamente hasta que el usuario finalice, que permita las siguientes opciones:

   ```markdown
   ### MENÚ

   1. Empezar cuestionario
   2. Ranking (opcional)
   3. Salir
   ```

2. Mostrar una serie de preguntas una a una al usuario.

3. Cada pregunta debe tener:

   - Enunciado de la pregunta.
   - Cuatro opciones de respuesta.
   - Una única opción correcta.

4. El usuario debe poder introducir su respuesta (por ejemplo: A, B, C o D).

5. El programa debe indicar si la respuesta es correcta o incorrecta.

6. Al finalizar el test, debe mostrar:

   - Número total de preguntas.
   - Número de aciertos.
   - Porcentaje de aciertos.
   - Una valoración final (por ejemplo: “¡Muy bien!”, “Necesitas practicar”, etc.).

<!-- prettier-ignore-end -->

<u>**Contenidos del módulo que se aplican**</u>

- Tipos de datos primitivos y estructuras complejas (listas, diccionarios).
- Control de flujo (if, elif, else).
- Bucles (for, while).
- Funciones con parámetros y retorno.
- Entrada/salida de datos por consola.

<u>**Estructura sugerida del programa**</u>

Puedes organizar tu programa en funciones como:

- cargar_preguntas() → Devuelve una lista de preguntas (pueden estar "hardcodeadas" al principio).
- mostrar_pregunta(pregunta) → Muestra la pregunta y sus opciones.
- obtener_respuesta() → Pide al usuario su respuesta y la valida.
- corregir_respuesta(respuesta, correcta) → Comprueba si es correcta.
- mostrar_resultados(aciertos, total) → Muestra el resumen final.

<u>**Ejemplo de estructura de una pregunta (diccionario)**</u>

```python
{
    "pregunta": "¿Cuál es la capital de Francia?",
    "opciones": ["A. Madrid", "B. Roma", "C. París", "D. Berlín"],
    "respuesta_correcta": "C"
}
```

<u>**Extras (para subir nota o como ampliación)**</u>

- Leer las preguntas desde un archivo .json o .txt (puedes usar el módulo json para leer la información .json y la función open() para los archivos .txt).
- Guardar los resultados del usuario (nombre y puntuación) en un fichero.
- Permitir elegir entre distintos temas o niveles de dificultad.
- Tiempo límite para cada pregunta.
- Sistema de ranking de usuarios.

<u>**Fases de trabajo sugeridas**</u>

1. Diseño del modelo de datos: ¿Cómo guardarás las preguntas?
2. Estructura básica del programa: Flujo general y funciones principales.
3. Implementación: Desarrollo progresivo de funciones.
4. Pruebas y validación: Comprobar que todo funcione correctamente.
5. Mejoras y presentación: Añadir extras, limpiar código, comentarios, etc.

<u>**Rúbrica de evaluación (orientativa)**</u>

| Criterio                            | Puntos |
| :---------------------------------- | :----- |
| Funcionalidad básica completa       | 4      |
| Uso correcto de funciones           | 2      |
| Uso adecuado de listas/diccionarios | 2      |
| Legibilidad y buenas prácticas      | 2      |
| **Total**                           | **10** |

<u>**Consejos finales**</u>

- Comienza por lo básico y ve añadiendo funcionalidades poco a poco.
- Prueba tu código frecuentemente para detectar errores a tiempo.
- Utiliza comentarios para explicar partes complejas del código.
- No dudes en pedir ayuda si te atascas en algún punto.

---

## 💼 Proyecto 1 IPE-I

<u>Fecha de entrega máxima</u>: PENDIENTE

- 📄 [Proyecto IPE-I] - En desarrollo

---

## 🖥️ Proyecto 1 Sistemas Informáticos

<u>Fecha de entrega máxima</u>: PENDIENTE

- 📄 [Proyecto Sistemas Informáticos] - En desarrollo
