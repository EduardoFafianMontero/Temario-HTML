 02 · Instalación de herramientas (Visual Studio Code)

## 📌 Qué necesito para empezar

Para escribir HTML solo hacen falta **un editor de texto** y **un navegador**. Usaré **Visual Studio Code** (VS Code) por sus extensiones y atajos.

## 🛠️ Instalación

1. Descargar VS Code desde la web oficial: <https://code.visualstudio.com>
2. Instalarlo (en Windows, marcar *"Añadir al PATH"* y *"Abrir con Code"* en el menú contextual).
3. Abrirlo y crear una carpeta de trabajo, por ejemplo `Temario-HTML`.
4. Desde la terminal, dentro de esa carpeta, `code .` la abre en VS Code.

## 🧩 Extensiones recomendadas

| Extensión | Para qué sirve |
| :--- | :--- |
| **Live Server** | Abre la página en el navegador y la **recarga sola** cada vez que guardo |
| **Prettier – Code formatter** | Formatea el código automáticamente (sangría, comillas) |
| **Auto Rename Tag** | Al cambiar una etiqueta de apertura, cambia también la de cierre |
| **HTML CSS Support** | Autocompleta clases e ids de CSS dentro del HTML |
| **Material Icon Theme** *(opcional)* | Iconos por tipo de archivo en el explorador |

## ⌨️ Atajos que uso a diario (Windows)

| Atajo | Acción |
| :--- | :--- |
| `Ctrl + S` | Guardar |
| `Ctrl + /` | Comentar / descomentar la línea |
| `Alt + Shift + F` | Formatear el documento |
| `Alt + ↑ / ↓` | Mover la línea arriba / abajo |
| `Shift + Alt + ↓` | Duplicar la línea |
| `Ctrl + D` | Seleccionar la siguiente coincidencia |
| `Ctrl + P` | Buscar un archivo por nombre |
| `Ctrl + ñ` o ``Ctrl + ` `` | Abrir / cerrar la terminal integrada |

## ⚡ Emmet: escribir HTML más rápido

VS Code trae **Emmet**: escribo una abreviatura y pulso `Tab`.

| Abreviatura | Resultado |
| :--- | :--- |
| `!` | La estructura mínima completa de una página |
| `p*3` | Tres párrafos `<p></p>` |
| `ul>li*3` | Una lista `<ul>` con tres `<li>` dentro |
| `div.caja` | `<div class="caja"></div>` |
| `div#principal` | `<div id="principal"></div>` |
| `h1{Mi título}` | `<h1>Mi título</h1>` |

## 📂 Contenido de este tema

- [`Ejercicios/ejemplo-comentado.html`](./Ejercicios/ejemplo-comentado.html) — la estructura que genera `!` + `Tab`, explicada.
- [`Practica/`](./Practica) — retos para configurar el entorno.

## 📝 Notas

- Emmet escribe `lang="en"` por defecto: hay que **cambiarlo a `es`** a mano.
- Live Server necesita abrir la **carpeta** (no un archivo suelto) en VS Code para funcionar bien.
