---
title: "Sprite"
---

## Constructors

::list

::constructor-info
#name 
Sprite
#overridings
()
#description
Creates a new instance of the sprite
::

::

## Properties

::list

::property-info
#name
image
#type
[Surface]{.ts-class}
#accessors
[get]{.ts-getter} [set]{.ts-setter}

#description
Gets or sets an image of sprite
::

::property-info
#name
rect
#type
[Rect]{.ts-class}
#accessors
[get]{.ts-getter} [set]{.ts-setter}

#description
Gets or sets a draw rect of sprite
::

::

## Methods

::list

::method-info
#method
draw
#overridings
(suface: [Suface]{.ts-class}) ⇨ [void]{.ts-base}

#description
Draws the sprite on a suface
::

::method-info
#method
[abstract]{.keyword} create
#overridings
() ⇨ [Promise]{.ts-class}\<[void]{.ts-base}\>

#description
A method for the sprite initialization. Implementing in a child class
::

::method-info
#method
[protected]{.keyword} update
#overridings
() ⇨ [void]{.ts-base}

#description
A method for the sprite update. Implementing in a child class
::

::