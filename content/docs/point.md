---
title: "Point"
---

## Constructors

::list

::constructor-info
#name 
Point
#overridings
(x: [number]{.ts-base}, y: [number]{.ts-base})<br>
(point: [TPoint]{.ts-type-intf})
#description
Creates a new instance of the point with certain parameters
::

::static-method-info
#class-name
Point
#method
zero
#overridings
()
#description
Creates a new instance of the point with coordinates (0,0)
::

::static-method-info
#class-name
Point
#method
one
#overridings
()
#description
Creates a new instance of the point with coordinates (1,1)
::


::static-method-info
#class-name
Point
#method
from
#overridings
(point: [TPoint]{.ts-type-intf})
#description
Creates a new instance of the point from a point like object
::

::static-method-info
#class-name
Point
#method
middle
#overridings
(p0: [TPoint]{.ts-type-intf}, p1: [TPoint]{.ts-type-intf})
#description
Creates a new instance of the point in the between of two p0 and p1 points
::

::



## Properties

::list

::property-info
#name
x
#type
[number]{.ts-base}
#accessors
[get]{.ts-getter} [set]{.ts-setter}

#description
Gets or sets x position of the point
::

::property-info
#name
y
#type
[number]{.ts-base}
#accessors
[get]{.ts-getter} [set]{.ts-setter}

#description
Gets or sets y position of the point
::

::property-info
#name
length
#type
[number]{.ts-base}
#accessors
[get]{.ts-getter} 

#description
Gets a length
::

::property-info
#name
magnitude
#type
[number]{.ts-base}
#accessors
[get]{.ts-getter} 

#description
Gets a magnitude
::

::property-info
#name
magnitudeSq
#type
[number]{.ts-base}
#accessors
[get]{.ts-getter} 

#description
Gets a magnitudeSq
::

::

## Methods

::list

::method-info
#method
moveX [Self]{.ts-self}
#overridings
(x: [number]{.ts-base}) ⇨ [Point]{.ts-class}
#description
Sets the point specified x coordinate
::

::method-info
#method
moveY [Self]{.ts-self}
#overridings
(y: [number]{.ts-base}) ⇨ [Point]{.ts-class}
#description
Sets the point specified y coordinate
::

::method-info
#method
move [Self]{.ts-self}
#overridings
(x: [number]{.ts-base}, y: [number]{.ts-base}) ⇨ [Point]{.ts-class}<br>
(xy: [number]{.ts-base}) ⇨ [Point]{.ts-class}<br>
(point: [TPoint]{.ts-type-intf}) ⇨ [Point]{.ts-class}<br>
#description
Sets the point specified x and y coordinates
::

::method-info
#method
shiftX [Self]{.ts-self}
#overridings
(dx: [number]{.ts-base}) ⇨ [Point]{.ts-class}
#description
Shifts the point specified x coordinate
::

::method-info
#method
shiftY [Self]{.ts-self}
#overridings
(dy: [number]{.ts-base}) ⇨ [Point]{.ts-class}
#description
Shifts the point specified y coordinate
::

::method-info
#method
shift [Self]{.ts-self}
#overridings
(dx: [number]{.ts-base}, dy: [number]{.ts-base}) ⇨ [Point]{.ts-class}<br>
(dxy: [number]{.ts-base}) ⇨ [Point]{.ts-class}<br>
(d: [TPoint]{.ts-type-intf}) ⇨ [Point]{.ts-class}<br>
#description
Shifts the point on a new position
::

::method-info
#method
scaleX [Self]{.ts-self}
#overridings
(dx: [number]{.ts-base}) ⇨ [Point]{.ts-class}
#description
Scales the point by x axis
::

::method-info
#method
scaleY [Self]{.ts-self}
#overridings
(dy: [number]{.ts-base}) ⇨ [Point]{.ts-class}
#description
Scales the point by y axis
::

::method-info
#method
scale [Self]{.ts-self}
#overridings
(dx: [number]{.ts-base}, dy: [number]{.ts-base}) ⇨ [Point]{.ts-class}<br>
(dxy: [number]{.ts-base}) ⇨ [Point]{.ts-class}<br>
(d: [TPoint]{.ts-type-intf}) ⇨ [Point]{.ts-class}<br>
#description
Scales the point by specified axises
::

::method-info
#method
negX [Self]{.ts-self}
#overridings
() ⇨ [Point]{.ts-class}
#description
Does negative x coordinate (x * -1)
::

::method-info
#method
negY [Self]{.ts-self}
#overridings
() ⇨ [Point]{.ts-class}
#description
Does negative y coordinate (y * -1)
::

::method-info
#method
neg [Self]{.ts-self}
#overridings
() ⇨ [Point]{.ts-class}
#description
Does negative x and y coordinates (x * -1, y * -1)
::

::method-info
#method
abs [Self]{.ts-self}
#overridings
() ⇨ [Point]{.ts-class}
#description
Converts axises to absolute
::

::method-info
#method
equals
#overridings
(point: [TPoint]{.ts-type-intf}) ⇨ [boolean]{.ts-base}
#description
Equals points
::

::method-info
#method
swapAxis [Self]{.ts-self}
#overridings
() ⇨ [Point]{.ts-class}
#description
Swaps axises
::

::method-info
#method
clone
#overridings
() ⇨ [Point]{.ts-class}
#description
Creates copy of the point
::

::method-info
#method
rotate [Self]{.ts-self}
#overridings
(deg: [number]{.ts-base}) ⇨ [Point]{.ts-class}
#description
Rotates the point around (0,0) point
::

::method-info
#method
dot
#overridings
(point: [TPoint]{.ts-type-intf}) ⇨ [number]{.ts-base}
#description
Does dot
::

::method-info
#method
cross
#overridings
(point: [TPoint]{.ts-type-intf}) ⇨ [number]{.ts-base}
#description
Does cross
::

::



