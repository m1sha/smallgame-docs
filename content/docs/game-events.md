---
title: 'GameEvents'
---

## Constructors

::list

::constructor-info
#name 
GameEvents
#overridings
()
#description
Creates a new instance of the GameEvents object
::

::

<br>

## Methods

::list

::method-info
#method
get
#overridings
() ⇨ [Generator]{.ts-class}<[GameEvent]{.ts-type-intf}> 
#description
Returns the event that occurred one at a time
#example
<br>Example:
```ts
gameloop(() => {
  for (const ev of game.events.get()) {
    console.log(ev.type)
  }
})
```
::

::