---
title: "gameloop"
---

## Functions

::list

::method-info
#method
gameloop
#overridings
(callback: () ⇨ [void]{.ts-base}) ⇨ [void]{.ts-base}

#description
Creates the game loop. The method use the window.requestAnimationFrame function inside
#example
<br>Example:
```ts
gameloop(() => {
  
  // a some code here
  
  console.log(Time.fps)
})
```
::

::method-info
#method
killgameloop
#overridings
() ⇨ [void]{.ts-base}

#description
Removes the game loop. The method use the window.cancelAnimationFrame function inside
#example
<br>Example:
```ts
gameloop(() => {
  for (const ev of game.events.get()) {
    if (ev.type === "KEYDOWN" && ev.key === Key.ESCAPE) {
      killgameloop()
      return
    }
  }

  // a some code here
})
```
::

::