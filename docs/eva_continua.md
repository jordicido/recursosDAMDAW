# EVALUACIÓN CONTINUA DAM/DAW - 1ª ENTREGA

La **Evaluación Continua** es una opción voluntaria para el alumnado que busca distribuir el esfuerzo a lo largo del curso. Esta modalidad aportará un 40% de la calificación final del módulo.
La primera entrega de actividades está prevista para principios de septiembre; la fecha exacta será confirmada próximamente.

## ☕ Proyecto 1 Programacion: Gestión de Clientes para un Negocio

<u>Fecha de entrega máxima</u>: 1 de septiembre a las 23:59

- 📄 [**PDF Proyecto Java**](https://drive.google.com/file/d/1aFklNGRnEcgMVphxF-FxWJMZGCPLCzRv/view) - Documento PDF del Proyecto 1

---

<u>**TÍTULO DEL PROYECTO**</u>

_Ejemplo: Sistema de Gestión para una Pajarería_

<u>**Entidades y clases** _(ejemplo)_</u>

1. Cliente

```java
public class Cliente {
    private String nombre; 
    private String dni; 
    private String telefono;
    private String email;
    // Constructor, getters y setters
}
```

2. Pájaro (lo que se vende)

```java
public class Pajaro {
    private String especie; 
    private String color; 
    private double precio;
    // Constructor, getters y setters
}
```

3. Venta

```java
public class Venta {
    private Cliente cliente;
    private ArrayList<Pajaro> lineasDeVenta; // cada venta contiene varios pájaros private 
    String fecha;
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

## 🐍 Proyecto 1 MPO | Python: Generador de Cuestionarios Interactivo

<u>Fecha de entrega máxima</u>: 1 de septiembre a las 23:59

- 📚 [**Enlace al repositorio de Jordi**](https://jordicido.github.io/jordicido-fp/MPO/proyecto1/) - MD del Proyecto 1

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

## 🖥️ Proyecto 1 Lenguaje de Marcas: Sitio web responsive

<u>Fecha de entrega máxima</u>: 1 de septiembre a las 23:59

- 📄 [**PDF Proyecto 1 Lenguaje de Marcas**](https://drive.google.com/drive/folders/1tX0kKLEfBH9th5pZi_s4y0Dru68gxVYL) - Documento PDF del Proyecto 1
- 📄 [**PDF Memoria Proyecto 1 Lenguaje de Marcas**](https://docs.google.com/document/d/15HnSuzQCUhGg9k8H6D9BY0ri7_GtCwHZ/edit) - Documento PDF de la Memoria del Proyecto 1

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

## 💾 Proyecto 1 Bases de Datos: BBDD de una universidad

<u>Fecha de entrega máxima</u>: 1 de septiembre a las 23:59

- 🔗 [**Enlace al Proyecto de BBDD**](https://app.thepowermba.com/challenges-and-projects/685553c735f33580d83f603f) - enlace al Proyecto 1

---

<u>**Título del Proyecto**</u>

_BBDD de una universidad_

<u>**Enunciado**</u>

*NOTA: Aparecen en negrita entidades; subrayados atributos; entre corchetes el concepto a representar.*

Se quiere implementar la BBDD de una universidad concreta, con las siguientes condiciones o requisitos pactados con el cliente:

El personal que se gestionará desde la BBDD serán: **profesores, alumnos, personal administrativo, auditores y visitas**. No existe otro tipo de personal más allá de estos. Y cada persona sólo puede pertenecer a uno de estos tipos. **\[ISA\]**

Todo personal que accede a la Universidad sea cual sea al grupo al que pertenece, debe identificarse con su <u>DNI, su nombre, apellidos, edad</u>, y **todos los teléfonos** que quieran proporcionar (pues es imprescindible que estén localizables en todo momento dentro de la instalación, por tanto al menos deben aportar un número de teléfono). De manera opcional se podrá registrar su <u>sexo</u> (“Masculino”, “Femenino” o “Prefiero no indicar nada”).

De los alumnos, además, se desea almacenar la <u>especialidad</u> escogida (que puede ser sólo una de las siguientes opciones: ingenierías, filologías, biologías, medicinas, o humanidades).

De los profesores se desea conocer también su **departamento**, y el <u>salario anual</u> (que debe ser mayor que cero, pero nunca superior a 60.000€).

Del personal administrativo, se registrará su **especialización** (que puede ser cualquiera de las que definan el Ministerio de Educación: recursos humanos, secretariado, legal, pedagógico, …etc).

De los auditores, <u>sus años de experiencia como auditores</u>, y <u>si trabajan también fuera de la Universidad como auditores o no</u>.

Todos los profesores imparten alguna de las **asignaturas** de la Universidad. Y algunos profesores pueden impartir más de una en el mismo curso.

Cada profesor puede pertenecer a varios **departamentos**. Y algunos años, alguno de estos departamentos se queda sin profesores adscritos.

Cada asignatura únicamente es impartida por un profesor; y algunas de estas asignaturas tienen a otra como pre-requisito (aunque ni todas las asignaturas son pre-requisitos, ni todas tienen otra como pre-requisito). **\[Relación Reflexiva\]**

De las asignaturas, también se quiere registrar el **aula** en el que se imparten (cada asignatura tiene, de hecho, un aula asignada por curso) **\[Relación Débil\]**. Cada aula, que puede albergar a varias asignaturas, está <u>numerada</u>, pero dicha numeración se repite entre edificios y plantas de dicha Universidad. Ha habido años que alguna aula se ha quedado sin utilizar. Y de algunas aulas, también se conoce:

- su <u>capacidad</u> (en número de alumnos que caben),

- y <u>si tienen tablón de anuncios o no</u>.

Respecto a la matriculación de los alumnos en los exámenes de las **convocatorias** de las asignaturas, nos indican lo siguiente: **\[Relación Ternaria\]**

- Las asignaturas tienen desde una convocatoria por curso, hasta 4 (dependiendo de diversas circunstancias).

- Las convocatorias son comunes a varias asignaturas (“diciembre”, “febrero”, etc…), y siempre, al menos, concurre una asignatura; por tanto, también concurre al menos, un alumno.

- Cualquier asignatura que se activa en un curso, tiene al menos un estudiante.

- Los alumnos pueden matricularse hasta en 4 convocatorias por asignatura, y en cada curso, siempre deben estar matriculados de al menos una asignatura, y una convocatoria.

Algunos alumnos, son representantes de otros, a modo de “vocales”, de cara a solicitudes, reclamaciones, etc… Pero, aunque no es obligatorio que todos los alumnos tengan algún representante, si lo tienen, sólo pueden ser representados por uno. Y un alumno no puede ser representante si no tiene asignado ningún alumno como representado. **\[Relación Reflexiva\]**

A algunos de los profesores, en algunas ocasiones, se les evalúa su trabajo como educadores, realizando una auditoría de su desempeño en la impartición de una asignatura concreta **\[Agregación – ver clase semana 25, última diapositiva\]**. Dichas auditorías las realizan los **auditores**, con las siguientes características:

- Un auditor puede realizar varias auditorías por curso (aunque puede haber auditores que, en un curso completo, no realicen ninguna auditoría).

- Para que un auditor pueda realizar auditorías de la impartición concreta de una asignatura por un profe, debe haber recibido previamente un **curso de orientación** en relación con la metodología del departamento al que pertenece la asignatura referida en la auditoría. **\[Restricción Exclusividad/Exclusión o Inclusividad/Inclusión\]**

- Cada departamento sólo posee un curso de éstos. Y cada curso sólo hace referencia a un departamento.

- Estos cursos, por tanto, cuentan con un <u>identificador único</u>, su <u>nombre</u> vinculado con el del departamento al que se refieren, y el <u>número de horas</u> de dicho curso.

- Y cada departamento tiene un <u>nombre único</u>, y también se conoce sus <u>años de existencia</u>, y el <u>nombre de su primer profesor adscrito</u>.

Además de estas auditorías, la Universidad entrega unos **premios** al desempeño y resultados de la impartición de una asignatura llevada a cabo por su profesor. Es decir, se premia no sólo al profesor, ni al colectivo relacionado con la asignatura, sino el trabajo, resultados y participación derivados de ese trabajo de impartición de una asignatura por parte de un profesor. Relativo a estos premios, nos indican que: **\[Agregación – ver clase semana 25, última diapositiva\]**

- Cada impartición, en caso de ser nominada, puede recibir más de un premio.

- Cada premio, puede ser entregado a varias imparticiones.

- Nunca se queda desierto un premio; y por supuesto, no todas las imparticiones reciben premio.

El sistema también debe poder registrar el <u>precio</u> de cada matriculación, sabiendo que ésta depende de cada alumno, de cada asignatura y de cada convocatoria. Es decir, cada alumno que se matricula en cada convocatoria de cada asignatura paga un precio (que depende de factores relativos a: beca, familia numerosa, matrícula de honor en otras asignaturas, precio del crédito ese año, etc…). Pues bien, en la matrícula se precisa registrar tanto ese precio, como la <u>nota final</u> de ese alumno en dicha convocatoria de dicha asignatura. **\[Relación Ternaria\]**

- Además, el sistema deberá verificar que el precio de la matriculación que paga cada alumno por cada asignatura siempre es mayor que cero.

El sistema debe:

- Permitir modificar los identificadores de: profesores, personal administrativo y visitas; pero no los de los alumnos ni auditores. **\[Restricciones del modelo Relacional\]**

- Si por algún motivo desapareciera un Departamento, su curso de orientación, será reasignado al departamento llamado “General”, para no perder dicho contenido. **\[Restricciones del modelo Relacional\]**

Cualquier dato que nos hayan pedido registrar en la base de datos descrita en este enunciado, y del que no se indique expresamente su carácter “opcional”, será entendido, por tanto, como un parámetro del que deberemos exigir una existencia obligatoria.

<!-- prettier-ignore-start -->

<u>**Cuestiones para Resolver**</u>

1. **Deberemos generar el Diagrama del Modelo Entidad-Relación Extendido.**

    1. Identificando entidades y sus respectivos atributos del MER.

    2. Estableciendo las relaciones pertinentes entre las entidades detectadas.

    3. Reflejando extensiones del MER (si existen: MERE).

    4. Añadiendo una leyenda, si procede, dónde se indique cual restricción o regla de funcionamiento de la BBDD, que no haya quedado reflejada en el MER/MERE, pero consideres oportuna poner de relevancia para el diseñador del MR que recibirá este MER/MERE.

    5. Anexar a este diagrama una breve memoria descriptiva, en la que se explique cualquier suposición tomada en cuenta, o cualquier asunción llevada a cabo por el diseñador, justificando adecuadamente dicha suposición (por falta de información, por mejora del diseño, por mayor legibilidad, etc…).

2. **Deberemos avanzar el posible código SQL para:**

    1. La transformación del MERE en un primer boceto de Modelo Relacional operativo (sin que sea preciso tener en cuenta ningún proceso de normalización). Teniendo en cuenta que sólo será preciso implementar la creación de:

        1. La base de datos.

        2. Las tablas con sus columnas y restricciones propias.

        3. La implementación de la Integridad Referencial derivada de las relaciones marcadas en el MERE que se desprende del enunciado.

        4. Las restricciones de operación de la BBDD, sólo de aquellos triggers que puedan implementarse sin utilizar sentencias “SELECT” en su interior; es decir, aquellos triggers que puedan implementarse únicamente mediante sencillos comandos de control y bucles (IF/ELSE, FOR EACH, …), sin tener que realizar consultas a otras tablas (sino que puedan resolver la restricción realizando las validaciones/verificaciones contra los registros que se están insertando/modificando/borrando (recuerda que podrías utilizar las funciones “NEW” y “OLD”, que hacen referencia a los registros que se están introduciendo, y el que se está intentando modificar, respectivamente).

    2. Para cada una de las demás restricciones que deberíamos incorporar en nuestra implementación (aquellas que precisarían de consultas a otras tablas), simplemente, deja comentado en el código:

        1. Cuáles triggers necesitarías para implementar cuál restricción concreta. Indicando para cada uno:

            1. Ante qué evento se debería activar.

            2. Cuáles serían las comprobaciones/validaciones a realizar en dicho trigger.

            3. Y cuál sería el resultado de su ejecución.

<!-- prettier-ignore-end -->

<u>**Rúbrica de evaluación (EDD)**</u>

| Criterio                                                                                     | Puntos |
| :------------------------------------------------------------------------------------------- | :----- |
| Creación del Modelo Entidad-Relación: Reconocimiento de los diferentes elementos del MER.    | 2      |
| Creación del Modelo Entidad-Relación: Identificación de las relaciones del MER/E.            | 2      |
| Creación del Modelo Entidad-Relación: Reconocimiento de las diferentes extensiones del MERE. | 3      |
| Creación del Modelo Relacional: Implementación de tablas y columnas en SQL                   | 1      |
| Creación del Modelo Relacional: Implementación de la Integridad Referencial.                 | 1      |
| Creación del Modelo Relacional: Implementación de restricciones adicionales.                 | 1      |
| **Total**                                                                                    | **10** |

---

## ⚙️ Proyecto 1 Entornos de Desarrollo: Profesionaliza tu proyecto Java

<u>Fecha de entrega máxima</u>: 1 de septiembre a las 23:59

- 📚 [**Enlace al repositorio de Jordi**](https://jordicido.github.io/jordicido-fp/MPO/proyecto1/) - MD del Proyecto 1

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

## 🖥️ Proyecto 1 Sistemas Informáticos: Máquinas Virtuales

<u>Fecha de entrega máxima</u>: 1 de septiembre a las 23:55

- 📄 [**PDF Proyecto 1 Sistemas Informáticos**](https://drive.google.com/drive/folders/15oLdPWdm-BlKBXMfPYwomb-al1eknTaJ) - Documento PDF del Proyecto 1

---

**<u>Descripción general</u>**

En este proyecto montarse pideás un pequeño laboratorio de máquinas virtuales que recrea, de forma sencilla, un entorno cliente-servidor real: desplegaremos un servidor Windows, un PC Ubuntu, un equipo con arranque dual y un host Proxmox, dejando constancia de la configuración y de la gestión básica de usuarios y recursos.

**<u>Objetivo del trabajo</u>**

El objetivo de este trabajo es que el alumno investigue, comprenda y realice la práctica basándose en el temario impartido en las clases del primer semestre.

**<u>Formato de entrega</u>**

Documento de texto (Word, pdf, Google Docs, etc.) o en formato presentación (PowerPoint, Google Slides, etc.).
Extensión: A determinar por el propio alumno (sugerencia: 8-12 páginas, sin contar portada y bibliografía).
Se valorará la claridad en la exposición, la correcta utilización de la terminología, la capacidad de síntesis y la justificación de los puntos solicitados mas abajo.

<!-- prettier-ignore-start -->

**<u>Secciones del trabajo</u>**

1. Creación de MV Server (4p)
    1. S.0 Windows server 2022
        1. Disco duro 1o: alojara el S.O, Denominado C:
        2. Recursos de la MV según capacidad de equipo de cada alumno(correctamente evidenciado)

    2. Nombre de la Mv DAM o DAW y nombre del alumno DAMPACO

    3. Creación de usuarios y grupos dentro del AD
        1. Lolo grupo (RRHH)
        2. Jaime grupo (CONTABILIDAD)
        3. Pedro (SIA)

2. Creación de Mv Desktop (Ubuntu) (4p)
    1. Debe llamarse PC+apellido del alumno ejemplo PCmartinez

    2. Debe Crear usuarios por consola y directorio personal
        1. Mercedes grupo (RRHH)
        2. Fer grupo (CONTABILIDAD)
        3. Mario (SIA)
        4. Contraseñas de 12 Digitos y que la contraseña
        5. Obligacion de cambiar contraseña cada 60 dias

    3. creación de grupos
        1. (RRHH)
        2. (CONTABILIDAD)
        3. (SIA)

3. Crear una Arranque DUAL en una MV(1p)
    1. En la misma MV Debe estar montado dos sistemas operativos un Windows+Ubuntu y en el arranque nos muestre la opción de cual elegir

4. Crear MV Proxmox (1p) (Según practicas realizadas en aula )
    1. DD con 60GB
    2. Subir una imagen a su directorio de Debian
    3. Crear una MV llamada DebianDAMDAW

<!-- prettier-ignore-end -->

---

## 💼 Supuestos IPE-I

Las entregas de trabajos de Evaluación Continua de IPE, a diferencia del resto de asignaturas, no se realizan divididas en dos grandes proyectos, en su lugar, se ha de realizar un supuesto práctico individual por cada unidad vista en clases (salvo la unidad 1).

Hasta el momento se han establecido los supuestos a entregar de las siguientes unidades:

- 📄 [**Supuestos Prácticos UNIDAD 2**](https://drive.google.com/file/d/1Ac-N_OOSpb4DU3jI6ksdIHJmS_1gr3zU) - Documento PDF de los supuestos prácticos UNIDAD 2

  <u>Fecha de entrega máxima</u>: Prorrogado: 24 de junio a las 23:59 <small>(Original: 21 de abril a las 23:59)</small>

- 📄 [**Supuestos Prácticos UNIDAD 3**](https://drive.google.com/file/d/1w7jG1JOYN7A_gQXak1cVf9Vx5B2TyVbP) - Documento PDF de los supuestos prácticos UNIDAD 3

  <u>Fecha de entrega máxima</u>: Prorrogado: 24 de junio a las 23:59 <small>(Original: 5 de mayo a las 23:59)</small>

- 📄 [**Supuestos Prácticos UNIDAD 4**](https://drive.google.com/file/d/14X7keRh7tT9sBDNaSorip3lEThbFwqzl) - Documento PDF de los supuestos prácticos UNIDAD 4

  <u>Fecha de entrega máxima</u>: Prorrogado: 24 de junio a las 23:59 <small>(Original: 20 de junio a las 23:59)</small>

---

<!-- prettier-ignore-start -->

**<u>Supuesto Práctico Individual UNIDAD 2</u>**

1. ¿Cuáles son los principales riesgos derivados de los lugares de trabajo?

2. ¿Qué es un equipo de trabajo?

3. ¿Cuáles son las principales causas de los accidentes eléctricos en el trabajo?

4. ¿Qué factores contribuyen a la aparición de trastornos musculoesqueléticos en el trabajo?

5. ¿Qué es el estrés laboral y cuáles son sus principales causas?

6. Describe tres conductas que pueden ser consideradas como acoso psicológico en el trabajo.

    <small>Se entregará en formato PDF y el diseño es libre.</small>

**<u>Supuesto Práctico Individual UNIDAD 3</u>**

En España, cada comunidad autónoma regula dónde deben instalarse los DEA/DESA y quién está autorizado para utilizarlos.
Cada vez más CCAA están legislando para instalar DEA/DESA en lugares de gran afluencia, como en centros comerciales, piscinas, gimnasios, edificios de oficinas, etc.

Consulta en la red información sobre estos desfibriladores y contesta a las siguientes preguntas:

1. ¿Puede utilizarlos cualquier persona que no sea personal sanitario? En caso negativo, ¿quién puede usarlo?

2. ¿Cuál es el procedimiento básico de uso de un DESA o DEA?

    <small>Se entregará en formato PDF y el diseño es libre.</small>

**<u>Supuesto Práctico Individual UNIDAD 4</u>**

1. Según el Texto Refundido del Estatuto de los Trabajadores, las personas trabajadoras autónomas y los transportistas y agentes comerciales por cuenta propia no están incluidos en las relaciones laborales. ¿Por qué motivo?

2. Las condiciones de trabajo que se pretenden pactar en un convenio colectivo contradicen las normas de una ley orgánica aprobada por las Cortes. ¿Qué principio jurídico sobre aplicación de las normas laborales debemos aplicar? ¿Qué finalidad tiene dicho principio?

3. Cita las principales fuentes externas del derecho del trabajo. Determina cuál de ellas son directamente aplicables y las que deban ratificarse por las Cortes Generales.

4. La Unión Europea exige que las condiciones de trabajo deban ser “armonizadas” en todos los estados miembros. ¿Significa esto que las condiciones laborales deben ser las mismas en estos países? Argumenta tu respuesta.

    <small>Se entregará en formato PDF y el diseño es libre.</small>

<!-- prettier-ignore-end -->
