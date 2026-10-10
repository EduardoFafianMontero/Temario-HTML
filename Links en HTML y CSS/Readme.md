# 05 · Links en HTML y CSS

## 📌 Qué se ve en este tema

Cómo enlazar páginas con la etiqueta `<a>` (*anchor*) y cómo darles estilo con CSS según su estado.

## 🔗 La etiqueta `<a>`

```html
<a href="https://www.google.com" target="_blank" rel="noopener noreferrer">Ir a Google</a>
```

| Atributo | Para qué sirve |
| :--- | :--- |
| `href` | A dónde lleva el enlace (la dirección) |
| `target="_blank"` | Abre el enlace en una pestaña nueva |
| `rel="noopener noreferrer"` | Seguridad al abrir pestañas nuevas; se pone siempre junto a `_blank` |
| `title` | Texto que aparece al pasar el ratón |
| `download` | Hace que el enlace descargue el archivo en vez de abrirlo |

## 🧭 Tipos de destino

| Tipo | Ejemplo de `href` | A dónde lleva |
| :--- | :--- | :--- |
| **Absoluto** | `https://www.wikipedia.org` | Otra web |
| **Relativo** | `otra-pagina.html` | Otro archivo de mi proyecto (misma carpeta) |
| **Relativo con carpeta** | `../index.html` | Un archivo en la carpeta superior |
| **Ancla interna** | `#contacto` | Una sección de la misma página (la que tenga `id="contacto"`) |
| **Correo** | `mailto:alguien@correo.com` | Abre el programa de correo |
| **Teléfono** | `tel:+34600000000` | Llama desde el móvil |

## 🎨 Estados del enlace con CSS

| Selector | Cuándo se aplica |
| :--- | :--- |
| `a:link` | Enlace sin visitar |
| `a:visited` | Enlace ya visitado |
| `a:hover` | Cuando el ratón está encima |
| `a:active` | Mientras se hace clic |

⚠️ **El orden importa:** debe ser `link` → `visited` → `hover` → `active` (truco: *LoVe HAte*). Si lo cambias, unos estados tapan a otros.

Otras propiedades útiles: `color`, `text-decoration` (`none` quita el subrayado), `font-weight`.

## 📂 Contenido de este tema

- [`Ejercicios/ejemplo-comentado.html`](./Ejercicios/ejemplo-comentado.html) — todos los tipos de enlace y los estados, comentados.
- [`Ejercicios/otra-pagina.html`](./Ejercicios/otra-pagina.html) — segunda página para probar el enlace relativo.
- [`Practica/`](./Practica) — retos.

## 📝 Notas

- El texto del enlace debe **describir el destino** ("Ver el temario de Java"), no ser "haz clic aquí".
- Un error de escritura en el `href` (una letra de más en una web, un nombre de archivo mal puesto) **no da ningún aviso**: el enlace simplemente no lleva a ninguna parte. Prueba siempre los enlaces haciendo clic.
- Las rutas son sensibles a mayúsculas en muchos servidores: `Pagina.html` y `pagina.html` pueden no ser el mismo archivo.
