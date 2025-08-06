# Point

## Constructors

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





## Properties

x:number get set Gets or sets x position of the point

y:number get set Gets or sets x position of the point

length:number get Gets a length

magnitude:number get Gets a magnitude

magnitudeSq:number get Gets a magnitudeSq

## Methods

moveX (x:number)⇨Point

Moves the point by the x axis


moveY (y:number)⇨Point

Moves the point by the y axis


shift (d:number)⇨Point

Shifts the point on a new position