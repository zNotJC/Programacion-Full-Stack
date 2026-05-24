# Guía de Estándares de Codificación del Proyecto

## 1. Objetivo

Establecer un conjunto de normas y buenas prácticas para garantizar que el código desarrollado en el proyecto sea claro, consistente, mantenible y fácil de entender por cualquier integrante del equipo.

---

## 2. Principios Generales

* El código debe priorizar la **legibilidad sobre la complejidad**.
* Todo desarrollo debe poder ser comprendido rápidamente por otros miembros del equipo.
* Se debe evitar la sobreingeniería y mantener soluciones simples y directas.
* Cada componente del sistema debe cumplir una única responsabilidad.

---

## 3. Convenciones de Nombres

### 3.1 Variables

* Deben ser descriptivas y reflejar su propósito.
* Se utilizará la convención **camelCase**.

**Ejemplo correcto:**

```js
let nombreEmpleado;
let listaUsuarios;
```

**Ejemplo incorrecto:**

```js
let x;
let a1;
```

---

### 3.2 Funciones

* Deben expresar claramente la acción que realizan.
* Deben iniciar con un verbo.

**Ejemplo correcto:**

```js
function validarCedula(cedula) { }
```

**Ejemplo incorrecto:**

```js
function proceso1() { }
```

---

### 3.3 Identificadores en HTML

* Deben ser claros y consistentes.

**Ejemplo:**

```html
id="formEmpleado"
name="correoElectronico"
```

---

## 4. Estructura del Código

### 4.1 HTML

* Debe estar organizado semánticamente:

  * `<header>`
  * `<main>`
  * `<footer>`
* Se debe evitar incluir lógica directamente en el HTML.

---

### 4.2 JavaScript

* El código debe separarse por responsabilidades en distintos archivos.
* Evitar archivos extensos con múltiples funcionalidades no relacionadas.

---

## 5. Funciones y Responsabilidad Única

* Cada función debe cumplir una sola tarea.
* Si una función realiza múltiples acciones, debe dividirse.

**Ejemplo correcto:**

```js
function validarCedula(cedula) {
    return /^\d+$/.test(cedula);
}
```

---

## 6. Evitar Duplicación de Código

* No se debe repetir lógica.
* Se deben reutilizar funciones para tareas comunes.

**Ejemplo:**

```js
function mostrarError(mensaje) {
    alert(mensaje);
}
```

---

## 7. Formato y Estilo

* Se debe mantener una sangría consistente (4 espacios o tabulación uniforme).
* Uso correcto de llaves y estructura:

```js
if (condicion) {
    // código
}
```

* Evitar formatos inconsistentes.

---

## 8. Uso de Comentarios

* El código debe ser autoexplicativo.
* Los comentarios se utilizarán únicamente cuando sea necesario aclarar lógica compleja o decisiones específicas.

**Ejemplo adecuado:**

```js
// Validación especial debido a restricciones del sistema externo
```

---

## 9. Validaciones

* Todos los datos ingresados por el usuario deben ser validados.
* No se debe confiar en la entrada del usuario.

**Ejemplo:**

```js
if (!cedula || !/^\d+$/.test(cedula)) {
    mostrarError("Cédula inválida");
}
```

---

## 10. Consistencia

* Se deben aplicar las mismas convenciones en todo el proyecto.
* No mezclar estilos de programación dentro del mismo sistema.

---

## 11. Mantenimiento del Código

* Cada modificación debe mejorar o mantener la calidad del código existente.
* Se recomienda aplicar la regla de:

  **“Dejar el código más limpio de lo que se encontró.”**

---

## 12. Buenas Prácticas Generales

* Evitar variables innecesarias.
* Mantener funciones pequeñas.
* Escribir código claro en lugar de código “ingenioso”.
* Priorizar la comprensión del código por encima de la optimización prematura.

---

## 13. Conclusión

El cumplimiento de estos estándares permite:

* Mejorar la calidad del software.
* Facilitar el trabajo en equipo.
* Reducir errores.
* Asegurar la mantenibilidad a largo plazo del sistema.

El equipo de desarrollo deberá aplicar estas normas de manera constante durante todo el ciclo de vida del proyecto.
