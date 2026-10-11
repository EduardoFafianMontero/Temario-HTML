# 10 · Elementos semánticos en HTML

## 📌 Qué se ve en este tema

Etiquetas que **describen su significado**, no solo su aspecto. Sustituyen a los `<div>` genéricos y mejoran la accesibilidad, el SEO y la lectura del código.

## 🏗️ Estructura típica de una página

```
┌──────────── header ────────────┐
│             nav                │
├──────────────┬─────────────────┤
│     main     │      aside      │
│  article     │                 │
│  article     │                 │
├──────────────┴─────────────────┤
└──────────── footer ────────────┘
```

## 🏷️ Etiquetas

| Etiqueta | Significado |
| :--- | :--- |
| `<header>` | Cabecera de la página o de una sección (logo, título) |
| `<nav>` | Bloque de enlaces de navegación |
| `<main>` | Contenido principal (**solo uno** por página) |
| `<section>` | Sección temática con su propio título |
| `<article>` | Contenido independiente (noticia, entrada de blog) |
| `<aside>` | Contenido secundario (barra lateral, anuncios) |
| `<footer>` | Pie de la página o de una sección |
| `<figure>` + `<figcaption>` | Imagen o ilustración con su pie |
| `<time>` | Fecha u hora legible por máquinas |

## 🆚 `div` vs semántica

| | `<div>` | Semánticas |
| :--- | :--- | :--- |
| Significado | Ninguno | Describen su función |
| Lectores de pantalla | No ayudan | Permiten saltar entre zonas |
| Buscadores | Sin pistas | Entienden la estructura |
| Cuándo usar | Solo para agrupar por estilo | Siempre que exista una etiqueta adecuada |

## 📂 Contenido de este tema

- [`Ejercicios/ejemplo-comentado.html`](./Ejercicios/ejemplo-comentado.html) — página completa con todas las etiquetas semánticas.
- [`Practica/`](./Practica) — retos.

## 📝 Notas

- Visualmente no cambian nada por sí solas: el aspecto lo da el CSS.
- Un `<article>` debe tener sentido por sí mismo, copiado en otra web.
- Cada `<section>` debería llevar un encabezado (`h2`, `h3`...).