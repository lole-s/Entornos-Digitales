<!--- imagen de encabezado --->
<p align="left">
  <img alt="" style="{max-height: 0px}" src="./dino-game/The%20Dinosaur%20Game.png">
</p>

## Cómo jugar al juego del dinosaurio

Puedes hacer clic [aquí](chrome://dino/) para jugar o apagar tu Internet para acceder a `Dinosaur Game`

- Simplemente abre `chrome://dino` en tu navegador web y serás llevado a un "modo arcade" donde podrás practicar en un entorno de ventana completa.

- Presione `Espacio` para reproducir `▶`.

- Puedes ver "HI" para verificar tu puntuación "Highest" y "Current".

<p align="left">
  <img alt="" style="{max-height: 0px}" src="./dino-game/Presiona espacio para jugar.PNG">
</p>

# Automatización/Hack para el juego Dinasour

#### Ajustando la velocidad

Escribe el siguiente comando en la consola y pulsa Intro. Puedes usar cualquier otra velocidad en lugar de 1000.

```js
Runner.instance_.setSpeed(1000)
```

#### Inmortalidad

Después de cada comando, presione Enter. Todos los comandos distinguen entre mayúsculas y minúsculas.

Almacenamos la función original de fin de juego en una variable:

```js
var original = Runner.prototype.gameOver
```

Luego, dejamos vacía la función juego terminado:

```js
Runner.prototype.gameOver = función(){}
```

Detener el juego después de usar la Inmortalidad

Cuando quieras detener el juego, vuelve a la función de fin del juego original:

```js
Runner.prototype.gameOver = original
```

#### Establecer la puntuación actual

Establezcamos la puntuación en 12345. Puedes establecer cualquier otra puntuación menor a 99999. La puntuación actual se restablece al finalizar el juego.

```js
Runner.instance_.distanceRan = 12345 / Runner.instance_.distanceMeter.config.COEFICIENTE
```

#### ¿ El Dino saltando demasiado alto?

Puedes controlar la altura del salto del dinosaurio con la siguiente función. Ajusta el valor según sea necesario.

```js
Runner.instance_.tRex.setJumpVelocity(10)
```

# Dino totalmente automatizado / Salto automático

Puedes automatizar completamente tu dinosaurio usando el código proporcionado en la consola.

```js
function keyDown(e){Podium={};var n=document.createEvent("KeyboardEvent");Object.defineProperty(n,"keyCode",{get:function(){return this.keyCodeVal}}),n.initKeyboardEvent?n.initKeyboardEvent("keydown",!0,!0,document.defaultView,e,e,"","",!1,""):n.initKeyEvent("keydown",!0,!0,document.defaultView,!1,!1,!1,!1,e,0),n.keyCodeVal=e,document.body.dispatchEvent(n)}function keyUp(e){Podium={};var n=document.createEvent("KeyboardEvent");Object.defineProperty(n,"keyCode",{get:function(){return this.keyCodeVal}}),n.initKeyboardEvent?n.initKeyboardEvent("keyup",!0,!0,document.defaultView,e,e,"","",!1,""):n.initKeyEvent("keyup",!0,!0,document.defaultView,!1,!1,!1,!1,e,0),n.keyCodeVal=e,document.body.dispatchEvent(n)}setInterval(function(){Runner.instance_.horizon.obstacles.length>0&&(Runner.instance_.horizon.obstacles[0].xPos<25*Runner.instance_.currentSpeed-Runner.instance_.horizon.obstacles[0].width/2&&Runner.instance_.horizon.obstacles[0].yPos>75&&(keyUp(40),keyDown(38)),Runner.instance_.horizon.obstacles[0].xPos<30*Runner.instance_.currentSpeed-Runner.instance_.horizon.obstacles[0].width/2&&Runner.instance_.horizon.obstacles[0].yPos<=75&&keyDown(40))},5);

Runner.instance_.setSpeed(1000)

var original = Runner.prototype.gameOver
Runner.prototype.gameOver = function(){}

//Runner.prototype.gameOver = original

Runner.instance_.distanceRan = 12345 / Runner.instance_.distanceMeter.config.COEFFICIENT

Runner.instance_.tRex.setJumpVelocity(10)
```

## Fin del juego de los dinosaurios

- Es un juego de carrera "endless", como una versión "en línea recta (straight-line)" de Temple Run sin niveles.

- Literalmente interminable: llega al puntaje «máximo» posible de «99.999» y el juego simplemente se «reinicia».

<p align="center">
  <img alt="" style="{max-height: 0px}" src="./dino-game/Dino.gif">
</p>

