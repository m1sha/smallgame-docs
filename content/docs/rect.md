---
title: "Rect (AABB Rectangle)"
---

## Constructors

::list

::constructor-info
#name 
Rect
#overridings
(x: [number]{.ts-base}, y: [number]{.ts-base}, width: [number]{.ts-base}, height: [number]{.ts-base})
#description
Creates a new instance of the rectangle with certain parameters
::

::static-method-info
#class-name
Rect
#method
zero
#overridings
()
#description
Creates a new instance of the rectangle with coordinates (0,0) and zero size
::

::static-method-info
#class-name
Rect
#method
size
#overridings
(width: [number]{.ts-base}, height: [number]{.ts-base})<br>
(size: [TSize]{.ts-type-intf})
#description
Creates a new instance of the rectangle from a size with coordinates (0,0)
::

::static-method-info
#class-name
Rect
#method
from
#overridings
(rect: [TRect]{.ts-type-intf})
#description
Creates a new instance of the rectangle from a rect like object
::

::static-method-info
#class-name
Rect
#method
fromTwoPoints
#overridings
(p0: [TPoint]{.ts-type-intf}, p1: [TPoint]{.ts-type-intf})
#description
Creates a new instance from two points a top-left and a bottom-right corners
::

::static-method-info
#class-name
Rect
#method
fromCenter
#overridings
(center: [TPoint]{.ts-type-intf}, width: [number]{.ts-base}, height: [number]{.ts-base})<br>

#description
Creates a new instance of the rectangle from a center point and specified width and height
::

::static-method-info
#class-name
Rect
#method
merge
#overridings
(rects: [TRect]{.ts-type-intf}\[])<br>

#description
Gets bounded rect 
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
Gets or sets x position of the rect
::

::property-info
#name
y
#type
[number]{.ts-base}
#accessors
[get]{.ts-getter} [set]{.ts-setter}

#description
Gets or sets y position of the rect
::

::property-info
#name
width
#type
[number]{.ts-base}
#accessors
[get]{.ts-getter} [set]{.ts-setter}

#description
Gets or sets width position of the rect
::

::property-info
#name
height
#type
[number]{.ts-base}
#accessors
[get]{.ts-getter} [set]{.ts-setter}

#description
Gets or sets height position of the rect
::

::property-info
#name
absWidth
#type
[number]{.ts-base}
#accessors
[get]{.ts-getter} 

#description
Gets absolute width position of the rect
::

::property-info
#name
absHeight
#type
[number]{.ts-base}
#accessors
[get]{.ts-getter} 

#description
Gets absolute height position of the rect
::

::property-info
#name
absCenter
#type
[TPoint]{.ts-type-intf}
#accessors
[get]{.ts-getter} 

#description
Gets the absolute center position of the rect
::

::property-info
#name
center
#type
[Point]{.ts-class}
#accessors
[get]{.ts-getter} [set]{.ts-setter}

#description
Gets or sets the center position of the rect <br> (changes to the x and y properties will have no effect on the target object)
::

::property-info
#name
topLeft
#type
[Point]{.ts-class}
#accessors
[get]{.ts-getter} [set]{.ts-setter}

#description
Gets or sets top-left corner of the rect <br> (changes to the x and y properties will have no effect on the target object)
::

::property-info
#name
topRight
#type
[Point]{.ts-class}
#accessors
[get]{.ts-getter} [set]{.ts-setter}

#description
Gets or sets top-right corner of the rect <br> (changes to the x and y properties will have no effect on the target object)
::

::property-info
#name
bottomLeft
#type
[Point]{.ts-class}
#accessors
[get]{.ts-getter} [set]{.ts-setter}

#description
Gets or sets bottom-left corner of the rect <br> (changes to the x and y properties will have no effect on the target object)
::

::property-info
#name
bottomRight
#type
[Point]{.ts-class}
#accessors
[get]{.ts-getter} [set]{.ts-setter}

#description
Gets or sets bottom-right corner of the rect <br> (changes to the x and y properties will have no effect on the target object)
::

::property-info
#name
diagonal
#type
[number]{.ts-base}
#accessors
[get]{.ts-getter}

#description
Gets a diagonal of the rect
::

::property-info
#name
points
#type
[number]{.ts-base}\[]
#accessors
[get]{.ts-getter}

#description
Gets array of points  <br> \[top-left.x, top-left.y, top-right.x, top-right.y, bottom-left.x, bottom-left.y, bottom-right.x, bottom-right.y]
::

::

## Methods

::list

::method-info
#method
move [Self]{.ts-self}
#overridings
(x: [number]{.ts-base}, y: [number]{.ts-base}, pivote?: [TPivote]{.ts-type-intf}) ⇨ [Rect]{.ts-class}<br>
(point: [TPoint]{.ts-type-intf}, pivote?: [TPivote]{.ts-type-intf}) ⇨ [Rect]{.ts-class}<br>
#description
Sets a rect new position
::

::method-info
#method
shift [Self]{.ts-self}
#overridings
(dx: [number]{.ts-base}, dy: [number]{.ts-base}, pivote?: [TPivote]{.ts-type-intf}) ⇨ [Rect]{.ts-class}<br>
(dp: [TPoint]{.ts-type-intf}, pivote?: [TPivote]{.ts-type-intf}) ⇨ [Rect]{.ts-class}<br>
#description
Shifts a rect
::

::method-info
#method
resize [Self]{.ts-self}
#overridings
(width: [number]{.ts-base}, height: [number]{.ts-base}) ⇨ [Rect]{.ts-class}<br>
(value: [number]{.ts-base}) ⇨ [Rect]{.ts-class}<br>
(size: [TSize]{.ts-type-intf}) ⇨ [Rect]{.ts-class}<br>
#description
Resizes a rect
::

::method-info
#method
scalesize [Self]{.ts-self}
#overridings
(dw: [number]{.ts-base}, dh: [number]{.ts-base}) ⇨ [Rect]{.ts-class}<br>
(value: [number]{.ts-base}) ⇨ [Rect]{.ts-class}<br>
(dsize: [TSize]{.ts-type-intf}) ⇨ [Rect]{.ts-class}<br>
#description
Scales a size of the rect
::

::method-info
#method
scale [Self]{.ts-self}
#overridings
(dx: [number]{.ts-base}, dy: [number]{.ts-base}) ⇨ [Rect]{.ts-class}<br>
(d: [number]{.ts-base}) ⇨ [Rect]{.ts-class}<br>
#description
Scales a rect
::

::method-info
#method
union [Self]{.ts-self}
#overridings
(rect: [TRect]{.ts-type-intf}) ⇨ [Rect]{.ts-class}<br>

#description
Unions rectangles by min & max points
::

::method-info
#method
rotate
#overridings
(deg: [number]{.ts-base}, pivote?: [TPivote]{.ts-type-intf}) ⇨ [PolyRect]{.ts-class}<br>
(deg: [number]{.ts-base}, pivote?: [TPoint]{.ts-type-intf}) ⇨ [PolyRect]{.ts-class}<br>

#description
Returns a rotated non-AABB rectangle
::

::method-info
#method
overlaps
#overridings
(rect: [TRect]{.ts-type-intf}) ⇨ [boolean]{.ts-base}<br>

#description
Check overlaps
::

::method-info
#method
inside
#overridings
(rect: [TRect]{.ts-type-intf}) ⇨ [boolean]{.ts-base}<br>

#description
Check inside
::

::method-info
#method
contains
#overridings
(rect: [TRect]{.ts-type-intf}) ⇨ [boolean]{.ts-base}<br>

#description
Check contains
::

::method-info
#method
containsPoint
#overridings
(point: [TPoint]{.ts-type-intf}) ⇨ [boolean]{.ts-base}<br>

#description
Check a point inside the rect
::

::method-info
#method
equals
#overridings
(rect: [TRect]{.ts-type-intf}) ⇨ [boolean]{.ts-base}<br>

#description
Check equals
::

::method-info
#method
outline
#overridings
(padding: [number]{.ts-base}) ⇨ [Rect]{.ts-class}<br>
(top: [number]{.ts-base}, left: [number]{.ts-base}, bottom: [number]{.ts-base}, right: [number]{.ts-base}) ⇨ [Rect]{.ts-class}<br>

#description
Create an outline
::

::method-info
#method
touchSide
#overridings
(rect: [TRect]{.ts-type-intf}) ⇨ [TSide]{.ts-type-intf}\[]

#description
Return one or two touched sides
::


::method-info
#method
clone
#overridings
()

#description
Clones the current rectangle
::

::