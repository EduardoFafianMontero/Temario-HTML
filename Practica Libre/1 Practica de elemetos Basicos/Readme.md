# Práctica libre 1 · Mi nuevo yo

## 📌 Sobre esta práctica

Primera práctica libre: una página con un texto **personal** sobre mis ganas de aprender y el mundo del desarrollo. Primero la planteé en papel y después la pasé a código. Sirve para practicar los **elementos básicos de HTML**: estructura del documento, títulos, párrafos, énfasis y texto preformateado.

## 🧩 Qué incluye

| Elemento | Uso en la página |
| :--- | :--- |
| `<!DOCTYPE html>` | Indica que es un documento HTML5 |
| `<html lang="es">` | Raíz del documento, con el idioma en español |
| `<head>` + `<meta charset="UTF-8">` | Configuración y codificación para ver bien tildes y la ñ |
| `<meta name="viewport">` | Adapta la página a pantallas de móvil |
| `<title>` | Título de la pestaña: "El comienzo" |
| `<h1>` | Título principal: "Mi nuevo yo" |
| `<p>` | Los párrafos del texto |
| `<i>` | Cursiva en la palabra *informática* |
| `<strong>` | Importancia: **"Hay que estar a la altura."** |
| `<pre>` | Bloque de texto preformateado con las ramas del desarrollo (Frontend, Backend, Apps móviles) |

### 🔎 Estructura de la página

```
html
├── head   → charset, viewport, title
└── body
    ├── h1  "Mi nuevo yo"
    ├── p   (ganas de aprender)
    ├── p   (informática: i + strong)
    ├── p   "En el mundo del desarrollo hay muchas ramas:"
    ├── pre (Frontend / Backend / Apps móviles)
    └── p   (cierre)
```

## 💻 Cómo verla

Abrir `index.html` con doble clic (se abre en el navegador) o, en VS Code, con la extensión **Live Server**.

## 📝 Notas

✅ **Se ve correctamente en el navegador.**

Cosas que aprendí al revisarla:

- **`<pre>` no puede ir dentro de un `<p>`.** Es un elemento de bloque; el navegador cierra el párrafo por su cuenta y el `</p>` final queda sobrando. Por eso el `<pre>` va **entre** dos párrafos.
- **`lang="es"`:** el idioma del documento debe coincidir con el del texto (antes estaba en `en`). Lo usan los lectores de pantalla y los traductores.
- **`<b>` dentro de `<strong>` era redundante:** los dos ponen negrita, así que se usa solo `<strong>` para lo importante.
- **`<pre>` respeta los espacios y saltos de línea tal cual,** por eso su contenido va pegado a la izquierda: si se indenta, esos espacios se ven en la página.
- **Varios `<p>` en lugar de `<br>`:** `<br>` es para saltos dentro de una frase; para separar ideas se usan párrafos.
- Revisar la ortografía del texto antes de hacer el commit: es contenido mío y se verá en mi GitHub.

**Ideas para ampliarla:** añadir un `<h2>` por sección, un enlace `<a>` a mi GitHub y una imagen `<img>` con su `alt`.