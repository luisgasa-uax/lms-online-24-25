# Apuntes de HTML5

## Etiquetas clásicas de HTML

### `<html>`
Elemento raíz de cualquier documento HTML.

```html
<html>
  ...
</html>
```

### `<head>`
Contiene metadatos del documento, como el título, enlaces a hojas de estilo, scripts, etc.

```html
<head>
  <title>Mi sitio web</title>
  <meta charset="UTF-8">
</head>
```

### `<title>`
Define el título del documento que aparece en la pestaña del navegador.

```html
<title>Mi sitio web</title>
```

### `<body>`
Contiene todo el contenido visible de la página web.

```html
<body>
  <h1>Hola mundo</h1>
</body>
```

### `<h1>` a `<h6>`
Definen encabezados, siendo `<h1>` el más importante y `<h6>` el menos.

```html
<h1>Encabezado principal</h1>
<h2>Subencabezado</h2>
```

### `<p>`
Define un párrafo.

```html
<p>Este es un párrafo.</p>
```

### `<a>`
Define un enlace.

```html
<a href="https://www.ejemplo.com">Visita nuestro sitio</a>
```

### `<img>`
Inserta una imagen.

```html
<img src="imagen.jpg" alt="Descripción de la imagen">
```

### `<ul>`, `<ol>` y `<li>`
Listas no ordenadas (`<ul>`), ordenadas (`<ol>`) y elementos de lista (`<li>`).

```html
<ul>
  <li>Elemento 1</li>
  <li>Elemento 2</li>
</ul>

<ol>
  <li>Paso 1</li>
  <li>Paso 2</li>
</ol>
```

### `<br>`
Inserta un salto de línea.

```html
Hola<br>mundo
```

### `<hr>`
Inserta una línea horizontal (separador).

```html
<p>Texto antes de la línea</p>
<hr>
<p>Texto después de la línea</p>
```

## Etiquetas semánticas HTML5

### `<header>`
Define la cabecera de un documento o sección. Suele contener el logo, título o menú de navegación.

```html
<header>
  <h1>Bienvenidos a mi sitio web</h1>
  <nav>
    <ul>
      <li><a href="#inicio">Inicio</a></li>
      <li><a href="#acerca">Acerca de</a></li>
      <li><a href="#contacto">Contacto</a></li>
    </ul>
  </nav>
</header>
```

### `<footer>`
Representa el pie de página de un documento o sección. Generalmente incluye información de contacto o derechos de autor.

```html
<footer>
  <p>&copy; 2025 Mi Sitio Web. Todos los derechos reservados.</p>
</footer>
```

### `<article>`
Define contenido independiente y autónomo, como un artículo de blog o una noticia.

```html
<article>
  <h2>Título del artículo</h2>
  <p>Contenido del artículo...</p>
</article>
```

### `<section>`
Representa una sección genérica de un documento, como un capítulo o parte de una página.

```html
<section>
  <h2>Sección 1</h2>
  <p>Contenido de la sección...</p>
</section>
```

### `<nav>`
Define un bloque de navegación. Se utiliza para agrupar enlaces de navegación.

```html
<nav>
  <ul>
    <li><a href="#inicio">Inicio</a></li>
    <li><a href="#servicios">Servicios</a></li>
    <li><a href="#contacto">Contacto</a></li>
  </ul>
</nav>
```

### `<aside>`
Representa contenido que está indirectamente relacionado con el contenido principal, como una barra lateral.

```html
<aside>
  <h3>Noticias relacionadas</h3>
  <ul>
    <li><a href="#">Noticia 1</a></li>
    <li><a href="#">Noticia 2</a></li>
  </ul>
</aside>
```

### `<figure>` y `<figcaption>`
`<figure>` define contenido multimedia con su leyenda, mientras que `<figcaption>` proporciona la leyenda.

```html
<figure>
  <img src="imagen.jpg" alt="Descripción de la imagen">
  <figcaption>Descripción de la imagen</figcaption>
</figure>
```

### `<mark>`
Resalta texto que es relevante o importante.

```html
<p>Este es un <mark>texto resaltado</mark> en el párrafo.</p>
```

### `<progress>`
Muestra el progreso de una tarea en curso.

```html
<progress value="70" max="100">70%</progress>
```

###  `<time>`
Representa una fecha, hora o intervalo de tiempo.

```html
<p>La conferencia será el <time datetime="2025-04-15">15 de abril de 2025</time>.</p>
```

---
---

## Tablas en HTML

Las tablas en HTML permiten organizar datos en filas y columnas. Se componen de varias etiquetas y atributos que controlan su estructura y presentación.



### Estructura básica

#### `<table>`
Etiqueta contenedora principal de una tabla.

```html
<table>
  <!-- contenido -->
</table>
```

#### `<tr>` (table row)
Define una fila de la tabla.

```html
<tr>
  <!-- celdas -->
</tr>
```

#### `<th>` (table header)
Define una celda de encabezado. Generalmente aparece al principio de cada columna.

```html
<th>Nombre</th>
```

#### `<td>` (table data)
Define una celda de datos.

```html
<td>Ana</td>
```

---

### Secciones de la tabla

#### `<thead>`
Agrupa las filas de encabezado de la tabla.

```html
<thead>
  <tr>
    <th>Nombre</th>
    <th>Edad</th>
  </tr>
</thead>
```

#### `<tbody>`
Agrupa el contenido principal de la tabla.

```html
<tbody>
  <tr>
    <td>Ana</td>
    <td>30</td>
  </tr>
</tbody>
```

#### `<tfoot>`
Agrupa el pie de la tabla (por ejemplo, totales).

```html
<tfoot>
  <tr>
    <td>Total</td>
    <td>2 registros</td>
  </tr>
</tfoot>
```


### Atributos importantes

#### `colspan`
Permite que una celda abarque varias columnas.

```html
<td colspan="2">Contenido combinado</td>
```

#### `rowspan`
Permite que una celda abarque varias filas.

```html
<td rowspan="2">Repetido</td>
```

---

### Ejemplo completo

```html
<table border="1">
  <caption>Horario de clases</caption>
  <thead>
    <tr>
      <th>Día</th>
      <th>Hora</th>
      <th>Asignatura</th>
      <th>Aula</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="2">Lunes</td>
      <td>08:00 - 09:00</td>
      <td>Matemáticas</td>
      <td>Aula 1</td>
    </tr>
    <tr>
      <td>09:00 - 10:00</td>
      <td>Lengua</td>
      <td>Aula 2</td>
    </tr>
    <tr>
      <td>Martes</td>
      <td>08:00 - 09:00</td>
      <td colspan="2">Excursión escolar</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td colspan="4">Horario sujeto a cambios</td>
    </tr>
  </tfoot>
</table>
```

---
---


## Formularios

### `<form>`
Crea un formulario interactivo para el usuario.

```html
<form action="/enviar" method="post">
  <label for="nombre">Nombre:</label>
  <input type="text" id="nombre" name="nombre">
  <input type="submit" value="Enviar">
</form>
```

### `<input>`
Campo de entrada para datos. Puede tener diferentes tipos: `text`, `email`, `password`, `checkbox`, `radio`, etc.

```html
<input type="email" placeholder="Tu correo electrónico">
```

### `<textarea>`
Campo de texto multilínea.

```html
<textarea name="comentario" rows="4" cols="50"></textarea>
```

### `<select>` y `<option>`
Menú desplegable.

```html
<select name="pais">
  <option value="es">España</option>
  <option value="mx">México</option>
</select>
```

### `<label>`
Etiqueta descriptiva para un control del formulario.

```html
<label for="correo">Correo:</label>
<input type="email" id="correo">
```

### Tipos de `<input>` en HTML y sus atributos

El elemento `<input>` es uno de los más utilizados en formularios HTML. Puede adoptar distintos comportamientos según el valor del atributo `type`.


#### 1. `type="text"`
Campo de texto de una sola línea.
```html
<input type="text" name="nombre">
```

#### 2. `type="password"`
Campo para contraseñas, oculta los caracteres ingresados.
```html
<input type="password" name="clave">
```

#### 3. `type="email"`
Valida direcciones de correo electrónico.
```html
<input type="email" name="correo">
```

#### 4. `type="tel"`
Campo para ingresar números de teléfono.
```html
<input type="tel" name="telefono">
```

#### 5. `type="url"`
Valida URLs.
```html
<input type="url" name="sitio">
```

#### 6. `type="number"`
Permite ingresar números.
```html
<input type="number" name="edad" min="0" max="120">
```

#### 7. `type="range"`
Selector de rango (deslizador).
```html
<input type="range" name="volumen" min="0" max="100">
```

#### 8. `type="date"`
Selector de fecha.
```html
<input type="date" name="fecha_nacimiento">
```

#### 9. `type="time"`
Selector de hora.
```html
<input type="time" name="hora">
```

#### 10. `type="datetime-local"`
Selector de fecha y hora local.
```html
<input type="datetime-local" name="cita">
```

#### 11. `type="month"`
Selector de mes y año.
```html
<input type="month" name="mes">
```

#### 12. `type="week"`
Selector de semana y año.
```html
<input type="week" name="semana">
```

#### 13. `type="checkbox"`
Casilla de verificación.
```html
<input type="checkbox" name="suscribirse" checked>
```

#### 14. `type="radio"`
Botón de opción (solo uno puede seleccionarse dentro del mismo grupo `name`).
```html
<input type="radio" name="genero" value="hombre"> Hombre
<input type="radio" name="genero" value="mujer"> Mujer
```

#### 15. `type="file"`
Permite subir archivos.
```html
<input type="file" name="cv">
```

#### 16. `type="hidden"`
Campo invisible usado para enviar datos sin mostrarlos al usuario.
```html
<input type="hidden" name="id" value="123">
```

#### 17. `type="submit"`
Botón para enviar el formulario.
```html
<input type="submit" value="Enviar">
```

#### 18. `type="reset"`
Botón para restablecer el formulario.
```html
<input type="reset" value="Limpiar">
```

#### 19. `type="button"`
Botón genérico que puede ser manejado por JavaScript.
```html
<input type="button" value="Haz clic" onclick="alert('Hola')">
```

---

## Atributos comunes

- `name`: Nombre del campo (clave en el envío de datos).
- `value`: Valor inicial del campo.
- `placeholder`: Texto de sugerencia dentro del campo.
- `required`: Campo obligatorio.
- `readonly`: Campo de solo lectura.
- `disabled`: Campo deshabilitado.
- `maxlength`: Máximo número de caracteres permitidos.
- `min`, `max`: Valores mínimo y máximo (para `number`, `range`, `date`, etc.).
- `step`: Incremento para valores numéricos o fechas.
- `pattern`: Expresión regular para validar el contenido.
- `autofocus`: El campo recibe el foco automáticamente al cargar la página.
- `checked`: Define si un checkbox o radio está marcado por defecto.
- `multiple`: Permite seleccionar varios archivos (solo en `file`) o múltiples opciones (en `select`).

---

Este documento proporciona una visión completa de los tipos de campos de entrada de formularios HTML, esenciales para recolectar distintos tipos de datos de los usuarios.



---
---

### Multimedia

#### `<audio>`
Incorpora audio en la página.

```html
<audio controls>
  <source src="audio.mp3" type="audio/mpeg">
  Tu navegador no soporta el elemento de audio.
</audio>
```

#### `<video>`
Incorpora video en la página.

```html
<video width="320" height="240" controls>
  <source src="video.mp4" type="video/mp4">
  Tu navegador no soporta el elemento de video.
</video>
```

---