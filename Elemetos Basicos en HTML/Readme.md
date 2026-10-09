# 03 · Elementos básicos de HTML

## 📌 Qué se ve en este tema

Las etiquetas de contenido que se usan en casi todas las páginas: títulos, párrafos, saltos de línea, énfasis, citas, código, imágenes y comentarios.

## 🧩 Etiquetas

| Etiqueta | Para qué sirve |
| :--- | :--- |
| `<h1>` ... `<h6>` | Títulos, de más a menos importante |
| `<p>` | Párrafo de texto |
| `<br>` | Salto de línea **dentro** de un párrafo (etiqueta vacía) |
| `<hr>` | Línea horizontal que separa contenido (etiqueta vacía) |
| `<strong>` | Texto **importante** (negrita con significado) |
| `<em>` | Texto con **énfasis** (cursiva con significado) |
| `<b>` / `<i>` | Negrita / cursiva solo **visual**, sin significado especial |
| `<blockquote>` | Cita larga de otra fuente |
| `<code>` / `<pre>` | Fragmento de código / texto que conserva espacios y saltos de línea |
| `<img>` | Imagen (etiqueta vacía) |
| `<!-- -->` | Comentario: el navegador no lo muestra |

## 🖼️ La etiqueta `<img>`

```html
<img src="imagenes/ejemplo.svg" alt="Logo de HTML" width="150">
```

| Atributo | Para qué sirve |
| :--- | :--- |
| `src` | Ruta del archivo de la imagen (relativa a mi `.html`) |
| `alt` | Texto alternativo: se muestra si la imagen falla y lo leen los lectores de pantalla. **Obligatorio** |
| `width` / `height` | Tamaño en píxeles (sin escribir `px`) |

## 📂 Contenido de este tema

- [`Ejercicios/ejemplo-comentado.html`](./Ejercicios/ejemplo-comentado.html) — todas las etiquetas en una página, comentadas.
- [`Ejercicios/imagenes/ejemplo.svg`](./Ejercicios/imagenes/ejemplo.svg) — imagen de prueba para el ejemplo.
- [`Practica/`](./Practica) — retos.

## 📝 Notas

- **Un solo `<h1>` por página**, y los títulos siguen un orden (`h1` → `h2` → `h3`), sin saltarse niveles. No se usan para "hacer el texto grande": para eso está CSS.
- `<br>` es para saltos puntuales (una dirección, un verso). Para separar ideas se usan **párrafos distintos**.
- `<strong>` y `<em>` **significan** algo (importancia, énfasis), y los lectores de pantalla lo entienden. `<b>` e `<i>` solo cambian el aspecto.
- Si la ruta de `src` está mal escrita, no da error: simplemente se ve el texto de `alt` en vez de la imagen. Es la primera cosa que hay que revisar.