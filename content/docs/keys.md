---
title: "Keys"
---

## Constructors

::list

::constructor-info
#name 
Keys
#overridings
()
#description
Creates a new instance of the keyboard event handler
::

::

<br>

## Methods

::list

::method-info
#method
getPressed
#overridings
() ⇨ [ReadonlyArray]{.ts-type-intf}\<[number]{.ts-base}\>
#description
Returns an array of keyboard keys, if the value is one, then the key is pressed
#example
<br>Example:
```ts
gameloop(() => {
  const keys = game.key.getPressed()
  
  if (keys[Key.K_A])
    console.log('The key A is pressed!')
})
```
::

::