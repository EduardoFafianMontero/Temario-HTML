# 08 · Elementos inline y block

## 📌 Qué se ve en este tema

Cómo se colocan los elementos en la página: unos ocupan toda la línea (**block**) y otros solo lo que miden (**inline**).

## 🧱 Diferencias

| | **Block** | **Inline** |
| :--- | :--- | :--- |
| Salto de línea | Empieza en línea nueva | Se queda en la misma línea |
| Ancho | Todo el ancho disponible | Solo lo que ocupa su contenido |
| `width` / `height` | ✅ Se respetan | ❌ Se ignoran |
| Margen/padding vertical | ✅ Funcionan | ⚠️ No empujan a los de alrededor |
| Ejemplos | `div`, `p`, `h1`–`h6`, `ul`, `li`, `table`, `form`, `section` | `span`, `a`, `strong`, `em`, `img`, `button`, `input` |

## 🔄 La propiedad `display`

| Valor | Efecto |
| :--- | :--- |
| `block` | Comporta como bloque |
| `inline` | Comporta como en línea |
| `inline-block` | En línea, pero acepta `width`, `height` y márgenes |
| `none` | Desaparece de la página y no ocupa sitio |

## 📦 `div` y `span`

Son contenedores **sin significado propio**: `<div>` es block y `<span>` es inline. Sirven para agrupar y dar estilo.

## 📂 Contenido de este tema

- [`Ejercicios/ejemplo-comentado.html`](./Ejercicios/ejemplo-comentado.html) — block vs inline y los valores de `display`.
- [`Practica/`](./Practica) — retos.

## 📝 Notas

- Un elemento inline **no puede contener** uno block (un `<a>` en HTML5 sí puede envolver bloques, pero un `<span>` con un `<div>` dentro es mala práctica).
- `visibility: hidden` oculta pero **sigue ocupando espacio**; `display: none` no.
