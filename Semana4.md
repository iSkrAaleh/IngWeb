
---

# 🧩 Semana 4 – Ingeniería Web

## 📘 Metodología UWE (UML-based Web Engineering)

### 🔹 Introducción

La **metodología UWE** (*UML-based Web Engineering*) es un enfoque orientado a modelar y desarrollar **aplicaciones web** utilizando los principios del **lenguaje UML**.
Su objetivo es ofrecer una forma estructurada de diseñar sitios o sistemas web desde la **captura de requisitos** hasta el **mantenimiento final**, garantizando consistencia, escalabilidad y claridad.

---

## ⚙️ Fases de la metodología UWE

### 1️⃣ Captura, análisis y especificación de requisitos

* En esta etapa se **reúnen, analizan y documentan** las características funcionales y no funcionales de la aplicación web.
* Se identifican los **actores**, los **casos de uso**, y los **requerimientos del sistema**.

**Ejemplo:**

> El sistema debe permitir a los usuarios registrarse, iniciar sesión, agregar productos al carrito y realizar compras.

---

### 2️⃣ Diseño del sistema

* Se basa en los requisitos analizados.
* Aquí se define **cómo funcionará el sistema**, tanto a nivel de estructura como de interacción entre los componentes.
* Se crean **diagramas de clases, secuencia y componentes** que servirán como guía para la codificación.

---

### 3️⃣ Codificación o desarrollo

* Se implementan los diseños usando lenguajes web (HTML, CSS, JS, PHP, etc.).
* Se crean las páginas, bases de datos y funcionalidades.

**Ejemplo:**

> Programar el módulo de registro y login de usuarios.

---

### 4️⃣ Pruebas

* Se verifican los módulos desarrollados.
* Se prueban errores, validaciones, flujos de usuario y compatibilidad entre navegadores y dispositivos.

---

### 5️⃣ Instalación o implementación

* Consiste en **desplegar la aplicación** en un servidor web.
* Se configuran el dominio, la base de datos y los parámetros del servidor.

---

### 6️⃣ Mantenimiento

* Se corrigen errores, se realizan mejoras o nuevas versiones.
* El sistema se mantiene actualizado con las necesidades del usuario y los cambios tecnológicos.

---

## 🧱 Extensión de UML en UWE

UWE amplía UML con estereotipos y modelos específicos para el desarrollo web:

### 🔸 Etapas principales:

* **Análisis de requisitos**
* **Diseño conceptual**
* **Diseño de navegación**
* **Diseño de presentación**

---

## 🧩 Modelos utilizados en UWE

### 1️⃣ Modelo de requisitos

Incluye:

* Diagramas de casos de uso
* Identificación de actores y funcionalidades del sistema
* Es la base del diseño posterior

---

### 2️⃣ Modelo de actividades

* Representa los **flujos de trabajo** y los **procesos** del sistema.
* Incluye **estereotipos** y sus **íconos correspondientes** (por ejemplo: acción, decisión, inicio, fin).

---

### 3️⃣ Modelo conceptual

* Define las **entidades, relaciones y atributos** del sistema.
* Equivale al modelo de clases en UML.

---

### 4️⃣ Modelo de navegación

* Representa **cómo se mueven los usuarios** dentro de la aplicación.
* Define los enlaces entre las vistas y las opciones accesibles (inicio, carrito, contacto, administración, reportes, etc.).

---

### 5️⃣ Modelo de presentación

* Muestra la **interfaz gráfica** del sistema.
* Se enfoca en la **experiencia del usuario (UI/UX)**.

---

### 6️⃣ Modelo de proceso

* Describe la **lógica interna** de cómo se ejecutan las operaciones dentro del sistema.
* Se puede representar con diagramas de secuencia o de flujo.

---

# 🌐 HTML5 – Introducción y teoría

## 📜 Breve historia

| Año  | Tecnología         |
| ---- | ------------------ |
| 1991 | HTML               |
| 1994 | HTML 2             |
| 1996 | CSS 1 / JavaScript |
| 1997 | HTML 4             |
| 1998 | CSS 2              |
| 2000 | XHTML 1            |
| 2005 | AJAX               |
| 2009 | HTML 5             |

**Organización que regula los estándares web:**
👉 **W3C (World Wide Web Consortium)**

---

## ⚡ HTML5 = Evolución

HTML5 surge como una **evolución del HTML tradicional**, ofreciendo:

* Mejor manejo de errores
* Mayor estandarización
* Código más **semántico y accesible**
* Soporte para **multimedia y aplicaciones web modernas**

---

## 💾 Capacidades de HTML5

### 🔸 Almacenamiento y acceso

* Aplicaciones **100% offline**
* Almacenamiento **interno, temporal o persistente**
* Funciones de **geolocalización**

### 🔸 CSS3

* Transformaciones y animaciones **2D y 3D**
* Transiciones visuales avanzadas

### 🔸 Multimedia

* Etiquetas `<audio>` y `<video>`
* Subtítulos y control de pistas

### 🔸 Gráficos y efectos 3D

* `<canvas>` para gráficos 2D
* **WebGL / OpenGL** para 3D

---

## 💡 Aliados del HTML5

**HTML + CSS + JavaScript = el trío base del desarrollo web moderno**

---

## 📱 HTML5 y diseño responsive

Permite crear **aplicaciones adaptables** a diferentes navegadores, resoluciones y dispositivos móviles.

---

## 🌍 HTML5 y la Web Semántica

La **web semántica** busca añadir **metadatos y significados** al contenido de la web para que los sistemas puedan **interpretar y procesar información automáticamente**.

**Ejemplo:**
Un artículo puede incluir etiquetas `<article>` y `<section>` que permiten entender su estructura y propósito.

---

## 🧱 Nuevos elementos semánticos de HTML5

`<article>`, `<aside>`, `<audio>`, `<canvas>`, `<command>`, `<datagrid>`, `<datalist>`, `<embed>`, `<event>`, `<figure>`, `<footer>`, `<header>`, etc.

---

# 🧰 Maquetación y estructura (Wireframing)

Antes de programar, se realiza una **maqueta o wireframe**, que es un esquema visual de la estructura de la página web.
Permite planificar dónde irán los elementos principales: encabezado, navegación, contenido y pie de página.

---

## 🧠 Teoría: Etiquetas estructurales HTML5

A continuación, las etiquetas más importantes con **explicaciones y ejemplos**.

---

### 🏷️ `<header>` – Cabecera de la página

Define el encabezado principal, puede incluir logotipo, menú, título o barra de navegación.

```html
<header>
  <h1>Mi Tienda Online</h1>
  <nav>Menú principal</nav>
</header>
```

**👉 Pregunta de examen:** ¿Qué contiene la etiqueta `<header>` y cuántas veces puede repetirse en una web?

---

### 🧭 `<nav>` – Navegación

Define los enlaces de navegación principales del sitio.

```html
<nav>
  <ul>
    <li><a href="index.html">Inicio</a></li>
    <li><a href="productos.html">Productos</a></li>
    <li><a href="contacto.html">Contacto</a></li>
  </ul>
</nav>
```

---

### 🧩 `<main>` – Contenido principal

Indica el contenido principal único del documento.

```html
<main>
  <h2>Bienvenido a nuestra tienda</h2>
  <p>Ofertas especiales por tiempo limitado.</p>
</main>
```

---

### 📰 `<article>` – Unidad de contenido

Representa un bloque independiente (noticia, publicación, producto, etc.).

```html
<article>
  <h3>Nuevo lanzamiento</h3>
  <p>Descubre nuestro nuevo producto...</p>
</article>
```

---

### 📚 `<section>` – Porción de contenido

Agrupa contenido relacionado en secciones temáticas.

```html
<section>
  <h2>Servicios</h2>
  <p>Diseño, desarrollo y mantenimiento web.</p>
</section>
```

---

### 💬 `<aside>` – Bloques relacionados

Contiene información secundaria (como una barra lateral o enlaces).

```html
<aside>
  <h4>Publicidad</h4>
  <p>Promoción de productos.</p>
</aside>
```

---

### 🦶 `<footer>` – Pie de página

Incluye derechos de autor, enlaces o información de contacto.

```html
<footer>
  <p>&copy; 2025 Mi Empresa. Todos los derechos reservados.</p>
</footer>
```

---

### 🔲 `<div>` – Contenedor genérico

Sirve para agrupar elementos sin significado semántico específico.

```html
<div class="contenedor">
  <p>Contenido agrupado visualmente.</p>
</div>
```


---

---

## 🌐 Práctica: creación de una página web con HTML y CSS en XAMPP

---

## 📁 Paso 1 – Crear la estructura del proyecto

1️⃣ Abre la carpeta de instalación de **XAMPP** → entra en **htdocs**.
2️⃣ Crea una nueva carpeta llamada:

```
PagJuego
```

3️⃣ Abre **Visual Studio Code (VSC)** → selecciona **Abrir carpeta** → elige `PagJuego`.

---

## 📄 Paso 2 – Crear el archivo principal `index.html`

Dentro de `PagJuego`, crea un archivo llamado:

```
index.html
```

Abre el archivo y escribe el siguiente código:

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Página de inicio de turismo</title>
    <link rel="stylesheet" href="css/estilos.css">
</head>

<body>
    <header class="cabeceraPrincipal">
        <div class="logotipo">
            Logotipo
        </div>

        <div class="busqueda">
            Formulario de búsqueda
        </div>
    </header>

    <nav class="menuPrincipal">
        <a href="#">Inicio</a>
        <a href="#">Servicios</a>
        <a href="#">Portafolio</a>
        <a href="#">Contactos</a>
    </nav>

    <section class="sliderPrincipal">
        <div>
            <h2>Slider de la página principal</h2>
        </div>
    </section>

    <section id="noticias">
        <article>Noticia 1</article>
        <article>Noticia 2</article>
    </section>

    <section>
        <div class="auspiciantes">
            Auspiciantes
        </div>
    </section>

    <footer>
        <h6>Derechos reservados UTPL 2025 - Power by @</h6>
    </footer>
</body>
</html>
```

---

## 🧠 Pregunta de examen

> 💡 El documento **HTML** consta de dos partes principales:
>
> * `<head>` → Contiene metadatos, título y enlaces a estilos o scripts.
> * `<body>` → Contiene todo el contenido visible de la página.

---

## 🎨 Paso 3 – Crear carpetas adicionales

Dentro de tu carpeta `PagJuego` crea:

```
css
imagenes
```

Dentro de la carpeta `css`, crea el archivo:

```
estilos.css
```

---

## 🎨 Paso 4 – Código CSS (`css/estilos.css`)

```css
/* ====================================== */
/* Importación de fuente desde Google Fonts */
/* ====================================== */
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap');

/* ====================================== */
/* Reset general                         */
/* ====================================== */
* {
    padding: 0;
    margin: 0;
}

/* ====================================== */
/* Estilos generales del documento        */
/* ====================================== */
body {
    font-family: 'Montserrat', Arial, Helvetica, sans-serif;
    background-color: beige;
}

/* ====================================== */
/* Cabecera principal                     */
/* ====================================== */
.cabeceraPrincipal {
    background-color: blue;
    color: azure;
    width: 80%;
    margin: 0 auto;
    padding: 20px;
}

/* Logotipo */
.cabeceraPrincipal .logotipo {
    background-color: white;
    color: blue;
    width: 30%;
    display: inline-block;
    margin: 10px;
}

/* Buscador */
.cabeceraPrincipal .busqueda {
    background-color: yellow;
    color: blue;
    width: 60%;
    display: inline-block;
    margin: 10px;
}

/* ====================================== */
/* Estilos del menú principal             */
/* ====================================== */
.menuPrincipal {
    background-color: red;
    color: azure;
    width: 80%;
    margin: 0 auto;
    padding: 10px 0;
    text-align: center;
}

/* estilos del menú principal */
nav.menuPrincipal a {
    color: white;
    text-decoration: none;
    padding: 10px;
}

/* Efecto hover del menú */
nav.menuPrincipal a:hover {
    background-color: #fff;
    color: #ff0000;
    border-bottom: 3px solid blue;
}

/* ====================================== */
/* Slider principal                       */
/* ====================================== */
section.sliderPrincipal {
    height: 400px;
    text-align: center;
    background-color: lightgray;
}

section.sliderPrincipal div {
    padding-top: 20px;
}

section.sliderPrincipal h2 {
    font-family: 'Montserrat', sans-serif;
    font-size: 30px;
}

/* ====================================== */
/* Noticias                               */
/* ====================================== */
#noticias {
    background-color: blue;
    color: aqua;
    padding: 20px;
    text-align: center;
}

/* ====================================== */
/* Auspiciantes                           */
/* ====================================== */
.auspiciantes {
    background-color: lightblue;
    text-align: center;
    padding: 20px;
}

/* ====================================== */
/* Pie de página                          */
/* ====================================== */
footer {
    background-color: black;
    color: white;
    text-align: center;
    padding: 15px;
}
```

---

## 🔎 Paso 5 – Explicación de selectores

| Selector                 | Descripción                                                              |
| ------------------------ | ------------------------------------------------------------------------ |
| `*`                      | Aplica a todos los elementos del documento (resetea márgenes y relleno). |
| `.cabeceraPrincipal`     | Clase que define el encabezado principal.                                |
| `.logotipo`, `.busqueda` | Subdivisiones internas de la cabecera, colocadas en línea.               |
| `.menuPrincipal`         | Barra de navegación principal.                                           |
| `#noticias`              | Sección de noticias, identificada con un **id**.                         |
| `.sliderPrincipal`       | Sección central tipo banner o slider.                                    |
| `.auspiciantes`          | Bloque inferior para logos o apoyos.                                     |
| `footer`                 | Pie de página con créditos y derechos reservados.                        |

---

## 💻 Paso 6 – Ver la página

Abre tu navegador y entra a:

```
http://localhost/PagJuego/index.html
```

Deberías ver:

* Encabezado con logotipo y formulario
* Menú principal centrado y con hover rojo
* Sección de slider con texto grande
* Noticias y auspiciantes
* Pie de página con “Derechos reservados UTPL 2025”

---

## 📚 Investigación adicional

### 🔹 **Flexbox**

Sirve para distribuir elementos horizontal o verticalmente, alinearlos y crear diseños adaptativos fácilmente.

Ejemplo:

```css
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
```

### 🔹 **CSS Grid**

Permite organizar contenido en filas y columnas fácilmente.

Ejemplo:

```css
section {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 10px;
}
```

---

## 🧠 Preguntas de examen destacadas

1. ¿Cuáles son las dos partes principales de un documento HTML?
2. ¿Qué etiqueta define la cabecera principal de una página web?
3. ¿Para qué sirve la propiedad `display: inline-block`?
4. ¿Qué diferencia hay entre un **id** y una **class** en CSS?
5. ¿Qué significa `text-decoration: none`?
6. ¿Qué hace la propiedad `border-bottom: 3px solid blue;` dentro de un hover?

---




