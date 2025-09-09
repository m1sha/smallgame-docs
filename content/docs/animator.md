---
title: "Animator"
---

## Constructors

::list

::constructor-info
#name 
Animator
#overridings
()
#description
Creates a new instance of the Animator object
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

::property-info
#name
animations
#type
[string]{.ts-base}\[]
#accessors
[get]{.ts-getter} 

#description
Gets names of animations
::

::property-info
#name
currentAnimation
#type
[string]{.ts-base}
#accessors
[get]{.ts-getter} 

#description
Gets the name of the current animation
::

::property-info
#name
onEndAnimationLoop
#type
[EndAnimationLoopCallback]{.ts-class} | [null]{.ts-base}
#accessors
[get]{.ts-getter} [set]{.ts-setter}

#description
Gets or sets a callback function occurred on end of the animation
::

::

<br>

## Methods

::list

::method-info
#method
add
#overridings
(name: [string]{.ts-base}, options: [AddAnimationOptions]{.ts-type-intf}) ⇨ [Promise]{.ts-class}<[void]{.ts-base}>

#description
Adds an animation to the Animator
::

::method-info
#method
bulk
#overridings
(list: [\[AnimationName]{.ts-type-intf}, [AnimationSource]{.ts-type-intf}][], options: [AddAnimationOptions]{.ts-type-intf}) ⇨ [Promise]{.ts-class}<[void]{.ts-base}>

#description
Adds the list of an animation to the Animator
::

::method-info
#method
entry
#overridings
(name: [string]{.ts-base}) ⇨ [void]{.ts-base}

#description
Sets the start animation
::

::method-info
#method
addTransition
#overridings
(transition: [AnimationTransition]{.ts-type-intf}) ⇨ [void]{.ts-base}

#description
Adds a transition between animations
::

::method-info
#method
set
#overridings
(name: [string]{.ts-base}) ⇨ [void]{.ts-base}

#description
Sets the animation as current
::

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