__Haz que servomotor salude durante 3 segundos, se detenga y regresa al centro .__

- Crear una nueva instancia de `Servo` en al pin ** 9 **
- Usa `servo.sweep` para rotar entre 0˚ y 180˚
- Usa `board.wait` para llarmar 'reset' después de ** 3 segundos **
- Al llamar 'reset' debería `parar` y `centrar` el servo
- Consulte los documentos para ver cómo volver a ponerlo al centro

## Codigo para empezar

```js
  var five = require('johnny-five')
  var board = new five.Board()
  board.on('ready', function () {

    // Tu solucion aqui!

  })
```

## Diagrama de Circuito

```
        Servo
        .---.
        | | |
      -===+===-
        | | |
        |   |
        '---'
        | | |
        | | |
GND  o--. | .--o  Pin 9
          |
 +5  o----.

```

## Componentes

- Servo - http://node-ardx.org/electronics-primer#servo

> Toma un pulso cronometrado y lo convierte en una posición angular del eje de salida.

## Docs

- Servo - https://github.com/rwaldron/johnny-five/wiki/Servo#api
- Board - https://github.com/rwaldron/johnny-five/wiki/Board#api

---
