# EVALUACIÓN CONTINUA DAM/DAW - 1ª ENTREGA

La **Evaluación Continua** es una opción voluntaria para el alumnado que busca distribuir el esfuerzo a lo largo del curso. Esta modalidad aportará un 40% de la calificación final del módulo. 
La primera entrega de actividades está prevista para principios de septiembre; la fecha exacta será confirmada próximamente.



## ☕ Proyecto 1 Programacion: Gestión de Clientes para un Negocio

<u>Fecha de entrega máxima</u>: PENDIENTE (Inicio Septiembre - Fecha por determinar aún)

- 📄 [**PDF Proyecto Java**](https://drive.google.com/file/d/1aFklNGRnEcgMVphxF-FxWJMZGCPLCzRv/view) - Documento PDF del Proyecto 1

---

<u>**TÍTULO DEL PROYECTO**</u> 

*Ejemplo: Sistema de Gestión para una Pajarería*

<u>**Entidades y clases** *(ejemplo)*</u>

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

| GESTIÓN DE CLIENTES           | GESTIÓN DE PÁJAROS (productos)                | GESTIÓN DE VENTAS                             | 
| :---------------------------  | :-------------------------------------------- | :-------------------------------------------- | 
| 1 Alta de clientes            | 1 Alta de pájaros disponibles (catálogo)      |1 Crear nueva venta: <br>&nbsp;&nbsp;&nbsp;&nbsp;1.1 Seleccionar cliente  <br>&nbsp;&nbsp;&nbsp;&nbsp;1.2 Añadir uno o más pájaros de la lista disponible |
| 2 Baja                        | 2 Listado del catálogo                        | 2 Mostrar todas las ventas realizadas         |
| 3 Modificación                | 3 Búsqueda por especie                        | 3 Mostrar ventas por cliente                  |
| 4 Búsqueda por DNI            |                                               | 4 Mostrar importe total de cada venta         |      
| 5 Listado                     |                                               |                                               |


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

| Tema                         | Evaluación                                    |
| :--------------------------- | :-------------------------------------------- |
| Variables, entrada/salida    | Captura y validación de datos                 |
| Estructuras de control       | Menús, búsquedas, selección                   |
| Clases y objetos             | Cliente, Pajaro, Venta                        |
| Colecciones (ArrayList)      | Listas de clientes, productos y líneas de venta |
| Funciones (static)           | Métodos organizados por funcionalidad         |
| Relaciones entre objetos     | Una venta está asociada a un cliente y varios pájaros |
| Modularidad y claridad       | Separación por métodos y clases               |

<u>**Evaluación**</u>

| Criterio                                  | Puntos |
| :---------------------------------------- | :----- |
| Correcta gestión de clases y relaciones   | 3      |
| Menús y lógica funcional                  | 2      |
| Uso de listas (ArrayList) correctamente   | 2      |
| Separación del código en funciones        | 1      |
| Validaciones y claridad del código        | 1      |
| Buenas prácticas y organización           | 1      |
| **Total** | **10** |

<u>**Extras opcionales** *(para subir nota)*</u>

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

| Criterio                                      | Puntos | Descripción detalla de la puntuación     |
| :----------------------------------------     | :----- |:---------------------------------------- |
| Estructura y uso correcto de HTML5 y CSS3     | 2      | 2 pts: HTML y CSS bien estructurados, semánticos, sin errores.<br>1 pt: estructura básica pero errores leves.<br>0 pt: uso incorrecto, desordenado o incompleto.|
| Diseño responsive funcional (mínimo en 2 resoluciones) | 2      | 2 pts: correcta adaptación a móvil y escritorio, sin fallos. <br>1 pt: adaptación parcial, errores en algún dispositivo.<br>0 pt: no es responsive. |
| Boceto previo en Figma (escritorio + móvil)   | 2      | 1 pt: se incluyen ambos bocetos y capturas claras.<br>0.5 pts: solo un boceto o capturas incompletas.<br>0 pt: no se entrega diseño en Figma. |
| Tipografías locales (mínimo 2)                | 0.50   | 0.5 pt: se usan dos fuentes distintas y están cargadas localmente.<br>0 pt: no se usan o no son locales. |
| Repositorio Git en GitHub (uso correcto)      | 1      | 1 pt: repositorio creado desde el inicio, con commits progresivos.<br>0.5 pts: pocos commits o repositorio mal estructurado.<br>0 pt: no se usa Git/GitHub.|
| JavaScript para menú responsive y cookies     | 1      | 1 pt: funcionalidad correcta del menú móvil y popup de cookies.<br>0.5 pts: uno de los dos funciona.<br>0 pt: ninguna funcionalidad presente.|
| Política de privacidad simulada               | 0.50 | 0.5 pt: texto simulado claro, accesible desde algún lugar del sitio.<br>0 pt: no está presente.|
| Calidad del diseño visual y experiencia de usuario (UX)| 2       | 2 pts: diseño cuidado, navegación clara, estética coherente.<br> 1 pt: diseño aceptable pero con fallos visuales o de estructura.<br>0 pt: diseño pobre, caótico o inacabado.|

---

## 💾 Proyecto 1 Bases de Datos

<u>Fecha de entrega máxima</u>: PENDIENTE

- 📄 [Proyecto BBDD] - En desarrollo

---

## ⚙️ Proyecto 1 Entornos de Desarrollo

<u>Fecha de entrega máxima</u>: PENDIENTE

- 📄 [Proyecto Entornos de Desarrollo] - En desarrollo

---

## 🐍 Proyecto 1 MPO | Python

<u>Fecha de entrega máxima</u>: PENDIENTE

- 📄 [Proyecto MPO] - En desarrollo

---

## 💼 Proyecto 1 IPE-I

<u>Fecha de entrega máxima</u>: PENDIENTE

- 📄 [Proyecto IPE-I] - En desarrollo

---

## 🖥️ Proyecto 1 Sistemas Informáticos

<u>Fecha de entrega máxima</u>: PENDIENTE

- 📄 [Proyecto Sistemas Informáticos] - En desarrollo
