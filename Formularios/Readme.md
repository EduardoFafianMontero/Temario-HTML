# 09 · Formularios en HTML

## 📌 Qué se ve en este tema

Cómo recoger datos del usuario con `<form>` y sus controles.

## 🧾 El formulario

```html
<form action="/enviar" method="post">
  <label for="nombre">Nombre</label>
  <input type="text" id="nombre" name="nombre" required>
  <button type="submit">Enviar</button>
</form>
```

| Atributo de `form` | Para qué sirve |
| :--- | :--- |
| `action` | A dónde se envían los datos |
| `method` | `get` (datos en la URL) o `post` (datos ocultos en el cuerpo) |

## ⌨️ Tipos de `<input>`

| `type` | Qué muestra |
| :--- | :--- |
| `text` | Texto de una línea |
| `password` | Texto oculto con puntos |
| `email` | Texto que valida formato de correo |
| `number` | Números (con `min`, `max`, `step`) |
| `date` | Selector de fecha |
| `checkbox` | Casilla (varias opciones a la vez) |
| `radio` | Botón de opción (solo una del grupo, mismo `name`) |
| `range` | Barra deslizante |
| `submit` | Botón de enviar |

## 🧩 Otros controles

| Etiqueta | Para qué |
| :--- | :--- |
| `<label>` | Texto asociado a un control (`for` = `id` del input) |
| `<select>` + `<option>` | Lista desplegable |
| `<textarea>` | Texto de varias líneas |
| `<button>` | Botón (`submit`, `reset`, `button`) |
| `<fieldset>` + `<legend>` | Agrupa controles con un título |

## ✅ Atributos útiles

| Atributo | Efecto |
| :--- | :--- |
| `name` | Nombre con el que viajan los datos (imprescindible) |
| `id` | Identificador, para enlazar con `label` |
| `placeholder` | Texto de ayuda dentro del campo |
| `required` | Campo obligatorio |
| `value` | Valor inicial |
| `minlength` / `maxlength` | Longitud mínima y máxima |
| `disabled` | Campo bloqueado |

## 📂 Contenido de este tema

- [`Ejercicios/ejemplo-comentado.html`](./Ejercicios/ejemplo-comentado.html) — formulario de registro con todos los controles.
- [`Practica/`](./Practica) — retos.

## 📝 Notas

- Sin `name`, el dato **no se envía**.
- Los `radio` de un mismo grupo deben compartir `name`; si no, se pueden marcar todos a la vez.
- La validación de HTML ayuda pero no sustituye a validar en el servidor.
