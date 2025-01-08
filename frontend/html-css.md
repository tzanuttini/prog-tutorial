# Documentación Básica de HTML y CSS

## Introducción
HTML (HyperText Markup Language) y CSS (Cascading Style Sheets) son las tecnologías fundamentales para construir páginas web. HTML proporciona la estructura del contenido, mientras que CSS define el diseño y el estilo visual.

---

## Temas a Tratar

### HTML
1. **Estructura básica de una página HTML**
   - Etiquetas principales: `<!DOCTYPE>`, `<html>`, `<head>`, `<body>`
2. **Etiquetas comunes**
   - Encabezados (`<h1>` a `<h6>`)
   - Párrafos (`<p>`)
   - Listas (`<ul>`, `<ol>`, `<li>`)
   - Enlaces (`<a>`)
   - Imágenes (`<img>`)
   - Tablas (`<table>`, `<tr>`, `<td>`, `<th>`)
   - Formularios (`<form>`, `<input>`, `<button>`, `<textarea>`, `<select>`)
3. **Atributos globales**
   - `id`, `class`, `style`, `title`
4. **Semántica en HTML5**
   - Etiquetas como `<header>`, `<footer>`, `<article>`, `<section>`

### CSS
1. **Selectores básicos**
   - Elementos (`tag`), clases (`.class`), IDs (`#id`)
   - Selectores avanzados (combinadores, pseudo-clases, pseudo-elementos)
2. **Propiedades comunes**
   - Colores: `color`, `background-color`
   - Texto: `font-size`, `font-family`, `text-align`
   - Bordes y márgenes: `border`, `margin`, `padding`
   - Dimensiones: `width`, `height`
3. **Modelo de caja (Box Model)**
   - Contenido, padding, border, margin
4. **Diseño responsivo**
   - Media queries
   - Unidades relativas (`em`, `rem`, `%`, `vh`, `vw`)
5. **Flexbox y Grid**
   - Conceptos y uso básico

---

## Ejercicios Propuestos

### HTML
1. **Estructura básica**
   - Crea un archivo HTML con la estructura mínima: encabezado, párrafo y un enlace.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Mi Primera Página</title>
</head>
<body>
    <h1>Bienvenido a mi página</h1>
    <p>Este es un párrafo de ejemplo.</p>
    <a href="https://www.ejemplo.com">Visita este enlace</a>
</body>
</html>
```

2. **Listas**
   - Crea una lista ordenada con tus tres libros favoritos y una lista desordenada con tus pasatiempos.

3. **Tablas**
   - Crea una tabla con 3 filas y 2 columnas para organizar información básica (por ejemplo, nombre y edad).

### CSS
1. **Estilos básicos**
   - Cambia el color de fondo de la página y el color del texto de los párrafos.

```css
body {
    background-color: lightblue;
    color: darkblue;
}
```

2. **Clases e IDs**
   - Aplica estilos diferentes a elementos con una clase específica y a un elemento con un ID.

```css
.clase-ejemplo {
    font-size: 20px;
    text-align: center;
}

#id-ejemplo {
    color: red;
    font-weight: bold;
}
```

3. **Flexbox**
   - Crea un contenedor con tres elementos distribuidos de manera equitativa.

```css
.contenedor {
    display: flex;
    justify-content: space-between;
}
```

### Proyecto Final
- Crea una página web básica con:
  - Un encabezado con el título del sitio
  - Una sección con información personal
  - Una lista de enlaces favoritos
  - Un formulario de contacto
  - Diseña la página usando CSS (colores, tamaños, tipografías, etc.)

---

## Recursos Adicionales
- [MDN Web Docs - HTML](https://developer.mozilla.org/es/docs/Web/HTML)
- [MDN Web Docs - CSS](https://developer.mozilla.org/es/docs/Web/CSS)
- [Flexbox Froggy](https://flexboxfroggy.com/)
- [Grid Garden](https://cssgridgarden.com/)
