# Justificaciones SEGUNDA PARTE

## 1. Organización de testimonios

* Organizamos la sección de testimonios utilizando Flexbox mediante display:flex.
* Aplicamos flex-direction:row-reverse para invertir el orden visual de los elementos y utilizamos justify-content:space-between para distribuir los testimonios de forma equitativa dentro del contenedor.
* De esta manera logramos ubicar el primer y último elemento en los extremos disponibles, cumpliendo con la distribución solicitada.

---

## 2. Login centrado horizontal y verticalmente

* Centramos la sección de login utilizando propiedades de Flexbox y distribución automática de márgenes dentro del contenedor principal.
* Dimensionamos la sección empleando medidas relativas como %, rem y vh, permitiendo que el tamaño se adapte al espacio disponible de la ventana.
* También utilizamos unidades tipográficas relativas para favorecer una mejor adaptabilidad visual entre distintos tamaños de pantalla.

---

## 3. Comparación entre content-box y border-box

* Aplicamos content-box en la sección Bienvenida y border-box en la sección Contacto con el objetivo de comparar ambos modelos de caja.
* Observamos que en content-box el ancho definido contempla únicamente el contenido, por lo que el padding y el border aumentan el tamaño total del elemento.
* En cambio, con border-box el contenido, el borde y el relleno quedan incluidos dentro de la medida establecida.
* Concluimos que border-box resulta más conveniente al trabajar con tamaños definidos, padding y bordes, ya que facilita el control del diseño y evita variaciones inesperadas en el tamaño final.

---

## 4. Operaciones administrativas en columna

* Modificamos las operaciones del sistema administrativo utilizando Flexbox sobre el contenedor .acciones.
* Aplicamos flex-direction:column para organizar las opciones verticalmente y utilizamos gap para mantener una separación uniforme entre los botones.
* Esta implementación permitió mejorar la organización visual de las acciones disponibles, facilitando su lectura e interacción dentro del panel administrativo.

---

## 5. Productos en fila centrados y separados

* Organizamos la lista de productos utilizando Flexbox para controlar la distribución horizontal de sus elementos.
* Aplicamos justify-content:center para centrar visualmente los productos dentro del contenedor y utilizamos gap para mantener una separación uniforme entre ellos.
* Incorporamos además flex-wrap para conservar una correcta adaptación ante diferentes tamaños de pantalla.
* De esta manera logramos mostrar los productos en fila, centrados dentro de la sección y sin que queden pegados a los extremos del contenedor.

---

## 6. Reorganización del encabezado sin modificar HTML

* Reorganizamos visualmente el encabezado utilizando el selector header como contenedor principal mediante Flexbox.
* Centramos la navegación usando el selector .navbar junto con propiedades de alineación flexibles.
* Ubicamos los elementos .logo y header h1 hacia el extremo derecho mediante posicionamiento dentro del encabezado, sin modificar la estructura HTML original.
* Para lograrlo utilizamos position:relative en el contenedor principal y position:absolute sobre los elementos que debían desplazarse visualmente hacia la derecha.

---

## 7. Labels junto a campos de formulario

* Analizamos la estructura actual de los formularios e identificamos que la mayoría de los campos utilizan atributos placeholder en lugar de elementos <label>.
* Debido a esta implementación, no fue posible ubicar cada label junto a su campo correspondiente sin modificar el HTML existente.
* Resolvimos el caso compatible con la estructura actual correspondiente al checkbox, utilizando Flexbox para alinear correctamente el campo y su texto asociado sin emplear saltos de línea manuales.
* Consideramos que una solución completa requeriría incorporar elementos <label> asociados a cada campo mediante los atributos for e id, permitiendo un control más preciso de la disposición y una mejor accesibilidad del formulario.

---