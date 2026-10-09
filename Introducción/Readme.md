# 01 · Introducción a HTML

## 📌 Qué es HTML

**HTML** (*HyperText Markup Language*) es el lenguaje que da **estructura** a una página web. No es un lenguaje de programación: no calcula nada, solo **describe qué es cada cosa** (un título, un párrafo, una imagen, un enlace...) usando **etiquetas**. El navegador lee esas etiquetas y dibuja la página.

Las tres piezas de la web:

| Tecnología | Se encarga de... |
| :--- | :--- |
| **HTML** | La estructura y el contenido |
| **CSS** | El aspecto (colores, tamaños, posición) |
| **JavaScript** | El comportamiento (interacción, lógica) |

## 🧱 Anatomía de una etiqueta

```html
<p class="intro">Hola, mundo</p>
```

| Parte | Ejemplo | Qué es |
| :--- | :--- | :--- |
| Etiqueta de apertura | `<p>` | Dónde empieza el elemento |
| Atributo | `class="intro"` | Información extra, con formato `nombre="valor"` |
| Contenido | `Hola, mundo` | Lo que se ve |
| Etiqueta de cierre | `</p>` | Dónde termina (lleva `/`) |

Apertura + contenido + cierre = **elemento**.

Algunas etiquetas son **vacías**: no tienen contenido ni cierre. Ejemplos: `<br>`, `<hr>`, `<img>`, `<meta>`, `<input>`.

## 🏗️ Estructura mínima de una página

| Etiqueta | Para qué sirve |
| :--- | :--- |
| `<!DOCTYPE html>` | Indica al navegador que es HTML5. Siempre en la primera línea |
| `<html lang="es">` | Elemento raíz; `lang` declara el idioma (accesibilidad, buscadores, traductor) |
| `<head>` | Metadatos: información sobre la página que **no se ve** |
| `<meta charset="UTF-8">` | Codificación de caracteres: así se ven bien tildes y ñ |
| `<meta name="viewport" ...>` | Hace que la página se adapte al ancho del móvil |
| `<title>` | Texto de la pestaña del navegador |
| `<body>` | Todo lo que **sí se ve** en pantalla |

## 📂 Contenido de este tema

- [`Ejercicios/ejemplo-comentado.html`](./Ejercicios/ejemplo-comentado.html) — la página mínima, con cada línea explicada.
- [`Practica/`](./Practica) — retos para hacer sin mirar el ejemplo.

## 📝 Notas

- Las etiquetas se **cierran en orden inverso** al que se abren: `<p><strong>texto</strong></p>`, nunca `<p><strong>texto</p></strong>`.
- El navegador **ignora los espacios y saltos de línea repetidos** del código. Para separar contenido hay que usar etiquetas (`<p>`, `<br>`), no pulsar Enter varias veces.
- Una página sin `lang` o sin `<title>` funciona, pero es peor para accesibilidad y buscadores.
