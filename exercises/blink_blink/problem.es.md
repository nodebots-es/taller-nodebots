# Bienvenido al taller-nodebots

Vamos a aprender uso basico del API de `johnny-five` como una serie de retos de programacion.

`johnny-five` es un API para trabajar con Arduino y otras placas de desarrollo, pero

**_No se necesita_ tener un Arduino para este taller**

El taller pondra un reto, y luego probara tu solucion.
El codigo para hablar con el Arduino se ha comentado.

**Pero _vamos_ a crear codigo de `johnny-five` que se puede ejecutar**

Cada una de tus soluciones se puede ejecutar directamente como programa de `node`.
Conecta un Arduino al USB, y veras como tu solucion se puede usar de verdad. 

-------------------------------------------------------------------------------

# Blink...Blink

**Escribe un programa para parpadear un LED conectado al pin 13 una vez por segundo.**

- Cuando este lista la conexion (Board.ready), crea una nueva instancia de `Led`.
- Pasale un numero al constructor del `Led` para decirle a que pin esta conectado.
- `Led` tiene un metodo `strobe(ms)`; que toma el intervalo en millisegundos.

## Para esto necesitaras

1. Crear un nuevo directorio para tus respuestas y entrar en el con `cd` en la consola.
2. Bajar johnny-five de npm: `npm install johnny-five`
3. Crear un fichero para tu solucion (e.g. 01-blink-blink.js) y editarlo.

Todas tus soluciones necesitan hacer:

- Un `require` (o `import`) al modulo `johnny-five`
- Crear una instancia con `new Board()`
- Crear una funcion cuando el el evento **ready** este listo
- Pasar la solucion dentro de la funcion...

```js
  var five = require('johnny-five')
  var board = new five.Board()
  board.on('ready', function () {

    // Aqui va tu solucion!

  })
```

## Diagrama de circuito

```
            330     LED
 Pin 13 o--/\/\/---->|------o GND
```

## Componentes

- LED - http://node-ardx.org/electronics-primer#led

> Emite luz cuando se pasa una pequeña corriente electrica (pero solo en una direccion).

## Docs

- Board - https://github.com/rwaldron/johnny-five/wiki/Board
- Led - https://github.com/rwaldron/johnny-five/wiki/Led#api

---
