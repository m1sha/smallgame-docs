---
title: "Animation"
---

## Constructors

::list

::constructor-info
#name 
Animation
#overridings
(map: [TileMap]{.ts-class}, rate: [number]{.ts-base})
#description
Creates a new instance of the Animation object
::

::

<br>

## Properties

::list

::property-info
#name
image
#type
[Surface]{.ts-base}
#accessors
[get]{.ts-getter} 

#description
Gets the current animation frame
::

::

<br>

## Methods

::list

::method-info
#method
play
#overridings
() ⇨ [void]{.ts-base}

#description
Plays the animation
::

::method-info
#method
pause
#overridings
() ⇨ [void]{.ts-base}

#description
Pauses the animation
::

::method-info
#method
stop
#overridings
() ⇨ [void]{.ts-base}

#description
Stops the animation
::

::method-info
#method
tick
#overridings
() ⇨ [void]{.ts-base}

#description
Counts the time until the frame is switched
::

::