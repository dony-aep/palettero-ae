# Registro de cambios

Todos los cambios notables de este proyecto se documentan en este archivo.

El formato está basado en [Keep a Changelog](https://keepachangelog.com/es-ES/1.1.0/),
y este proyecto sigue el [Versionado Semántico](https://semver.org/lang/es/).

## [Sin publicar]

## [1.2.0] - 2026-10-05

### Añadido

- Flecha de deshacer en la franja, junto al «+». Recupera un color quitado por error con
  Shift+click y deshace también los demás cambios en las paletas: un color editado o añadido,
  la paleta aleatoria anterior, una paleta eliminada, renombrada o guardada. Alt+click (Option
  en Mac) rehace. El Ctrl+Z de After Effects no sirve para esto, porque las paletas no forman
  parte del proyecto. Guarda hasta 30 pasos mientras After Effects está abierto.

## [1.1.0] - 2026-10-04

### Añadido

- Shift+click en una muestra la quita de la paleta. Antes solo se podía quitar la última y,
  para borrar un color del medio, había que quitar y volver a añadir los que venían detrás.
- Botón «+» junto al dado para añadir un color sin estirar el panel. Hasta ahora Añadir color
  solo estaba entre las opciones, que no se ven con el panel como franja fina.

### Cambiado

- Las paletas se eligen viéndolas, no por el nombre. Al estirar el panel aparecen todas en
  filas, cada una con sus colores, y un click activa la que quieras. Sustituye al desplegable
  de nombres. Si no caben todas, una barra permite desplazarlas.

### Corregido

- En Windows, la franja flotante ya no deja huecos vacíos al pasar el cursor por las muestras
  o los botones mientras Solid Settings, el selector de color u otro diálogo de After Effects
  está abierto.

## [1.0.0] - 2026-10-02

Primera versión. Palettero es una paleta de colores para After Effects pensada para pantallas
pequeñas: cabe en una franja fina encima del visor y sigue siendo útil a ese tamaño.

### Añadido

- Panel acoplable con una fila de muestras de color. Como franja fina, los cuadrados se
  encogen para caber; al estirar el panel aparecen las opciones, repartidas en filas según el
  ancho, sin botones cortados ni solapados.
- Click en una muestra para cambiar su color. Alt+click (Option en Mac) lo aplica a las
  propiedades de color o a las capas seleccionadas: sólidos, texto y rellenos de forma.
  Ctrl+click (Cmd en Mac) crea un sólido de ese color. Las dos acciones ponen el valor exacto,
  se deshacen con un solo paso y respetan las capas bloqueadas.
- Franja flotante con la misma paleta que el panel, para tomar colores con el cuentagotas de
  Solid Settings y del selector de color, que en Windows no pueden leer los paneles acoplados.
  Recuerda su posición y tamaño.
- Cinco paletas de partida, paletas aleatorias con armonías de color, y paletas propias con
  nombre que se pueden guardar, renombrar y eliminar. Se conservan entre sesiones.
- Ventana de información con la versión, los atajos de cada sistema y el enlace a
  donyaep.vercel.app, que también abre la marca «Made by dony.» del panel.
- Probado en After Effects 2026 sobre Windows y en After Effects 2022 sobre macOS.
- Licencia: gratis para uso personal y comercial, distribuido solo compilado.

[Sin publicar]: https://github.com/dony-aep/palettero-ae/compare/v1.2.0...HEAD
[1.2.0]: https://github.com/dony-aep/palettero-ae/compare/v1.1.0...v1.2.0
[1.1.0]: https://github.com/dony-aep/palettero-ae/compare/v1.0.0...v1.1.0
[1.0.0]: https://github.com/dony-aep/palettero-ae/releases/tag/v1.0.0
