# 04 · Introducción a CSS

## 📌 Qué es CSS

**CSS** (*Cascading Style Sheets*) controla el **aspecto** de la página: colores, tipografías, tamaños, espacios, posición. HTML dice *qué es* cada cosa; CSS dice *cómo se ve*.

## 🔗 Tres formas de añadir CSS

| Forma | Cómo se escribe | Cuándo usarla |
| :--- | :--- | :--- |
| **En línea** | `<p style="color: red;">` | Casi nunca: mezcla estructura y estilo |
| **Interna** | Bloque `<style>` dentro de `<head>` | Pruebas rápidas o una sola página |
| **Externa** | `<link rel="stylesheet" href="estilos.css">` en `<head>` | **La normal**: un `.css` reutilizable en muchas páginas |

## 🧱 Anatomía de una regla

```css
h1 {
  color: navy;
  font-size: 32px;
}
```

`h1` es el **selector** (a quién), `color` y `font-size` son **propiedades** (qué cambio) y `navy` y `32px` son **valores**.

## 🎯 Selectores básicos

| Selector | Ejemplo | A quién afecta |
| :--- | :--- | :--- |
| Etiqueta | `p { }` | Todos los `<p>` |
| Clase | `.destacado { }` | Elementos con `class="destacado"` (reutilizable) |
| Id | `#cabecera { }` | El único elemento con `id="cabecera"` |
| Grupo | `h1, h2 { }` | Varios selectores a la vez |
| Descendiente | `nav a { }` | Los `<a>` que están dentro de un `<nav>` |

## 🎨 Propiedades y valores habituales

| Propiedad | Para qué | Ejemplos de valor |
| :--- | :--- | :--- |
| `color` | Color del texto | `red`, `#ff6600`, `rgb(255, 102, 0)` |
| `background-color` | Color de fondo | `#f4f4f4` |
| `font-family` | Tipografía | `Arial, sans-serif` |
| `font-size` | Tamaño del texto | `16px`, `1.2rem` |
| `text-align` | Alineación | `left`, `center`, `right` |
| `border` | Borde | `1px solid black` |
| `margin` | Espacio **fuera** del borde | `20px` |
| `padding` | Espacio **dentro** del borde | `10px` |

## 📏 Unidades

| Unidad | Qué es |
| :--- | :--- |
| `px` | Píxeles: tamaño fijo |
| `%` | Porcentaje del elemento padre |
| `em` | Relativa al tamaño de letra del propio elemento |
| `rem` | Relativa al tamaño de letra de la raíz (`html`); la más cómoda para tamaños de texto |

## 📦 El modelo de caja

Todo elemento es una caja formada por 4 capas, de dentro hacia fuera: **contenido → padding → border → margin**.

Con `box-sizing: border-box;` el `width` incluye padding y borde, y los cálculos son mucho más intuitivos. Es habitual ponerlo a todo:

```css
* {
  box-sizing: border-box;
}
```

## ⚖️ La cascada: ¿quién gana si hay conflicto?

1. Estilo **en línea** > selector de **id** > selector de **clase** > selector de **etiqueta**.
2. Si dos reglas tienen la misma fuerza, **gana la que está escrita después**.

## 📂 Contenido de este tema

- [`Ejercicios/ejemplo-comentado.html`](./Ejercicios/ejemplo-comentado.html) y [`Ejercicios/estilos.css`](./Ejercicios/estilos.css) — HTML + CSS externo, comentados.
- [`Practica/`](./Practica) — retos.

## 📝 Notas

- En CSS los comentarios son `/* así */` (no `<!-- -->`).
- Cada declaración termina en `;` y cada regla va entre llaves `{ }`. Olvidar un `;` es el error más común: rompe esa declaración y la siguiente.
- Un nombre de clase mal escrito no da error: el estilo simplemente no se aplica. Si "no funciona", revisa primero el nombre.
