---
title: "Sketch"
---

## Constructors

::list

::constructor-info
#name 
Sketch
#overridings
()
#description
Creates a new instance of the sketch
::

::

## Properties

::list

::property-info
#name
styleNames
#type
[string]{.ts-base}\[]
#accessors
[get]{.ts-getter} 

#description
Gets list of style names
::

::property-info
#name
bounds
#type
[Rect]{.ts-class}
#accessors
[get]{.ts-getter} 

#description
Gets a bounded rectangle
::

::

## Methods

::list

::method-info
#method
defineStyle
#overridings
(name: [string]{.ts-base}, style: [TShapeStyle]{.ts-type-intf}) ⇨ [ShapeStyle]{.ts-class}

#description
Creates a named style in the sketch
::

::method-info
#method
copyStyles
#overridings
(source: [Sketch]{.ts-class}) ⇨ [void]{.ts-base}

#description
Copies style from a source sketch to the current sketch
::

::method-info
#method
cloneStyles
#overridings
(source: [Sketch]{.ts-class}) ⇨ [void]{.ts-base}

#description
Creates new instance of styles from a source sketch and copies those to the current sketch
::

::method-info
#method
getStyle
#overridings
(name: [string]{.ts-base}) ⇨ [ShapeStyle]{.ts-class}

#description
Gets a style by the name
::

::method-info
#method
clear
#overridings
() ⇨ [void]{.ts-base}

#description
Deletes all shapes from the sketch
::

::method-info
#method
rect
#overridings
(style: [ShapeStyleTypes]{.ts-type-intf}, rect: [TRect]{.ts-type-intf}) ⇨ [Rectangle]{.ts-type-intf}

#description
Creates a rectangle by specified parameters
::

::method-info
#method
rects
#overridings
(style: [ShapeStyleTypes]{.ts-type-intf} | [ShapeStyleTypes]{.ts-type-intf}\[] | [ShapeStyleTypes]{.ts-type-intf}\[]\[], rect: [TRect]{.ts-type-intf}, cols: [number]{.ts-base} = 1, rows: [number]{.ts-base} = 1, options?: [TRectDrawOptions]{.ts-type-intf}) ⇨ [Rectangle]{.ts-type-intf}\[]

#description
Creates a grid of rectangles by specified parameters
::

::method-info
#method
polyrect
#overridings
(style: [ShapeStyleTypes]{.ts-type-intf}, rect: [PolyRect]{.ts-class}) ⇨ [PolyRectangle]{.ts-type-intf}

#description
Creates a non-AABB rectangle by specified parameters
::

::method-info
#method
polygon
#overridings
(style: [ShapeStyleTypes]{.ts-type-intf}, points: [TPoint]{.ts-type-intf}\[]) ⇨ [Polygon]{.ts-type-intf}

#description
Creates a polygon by specified parameters
::

::method-info
#method
dots
#overridings
(style: [ShapeStyleTypes]{.ts-type-intf}, points: [TPoint]{.ts-type-intf}\[], radius: [number]{.ts-base} = 1) ⇨ [Polydots]{.ts-type-intf}

#description
Creates dots by specified parameters
::

::method-info
#method
arrows
#overridings
(style: [ShapeStyleTypes]{.ts-type-intf}, segments: [TSegment]{.ts-type-intf}\[], options?: [TCreateArrowOptions]{.ts-type-intf}) ⇨ [Arrows]{.ts-type-intf}

#description
Creates arrows by specified parameters
::

::method-info
#method
roundedrect
#overridings
(style: [ShapeStyleTypes]{.ts-type-intf}, rect: [TRect]{.ts-type-intf}, radii?: [number]{.ts-base} | [number]{.ts-base}\[]) ⇨ [RoundedRectangle]{.ts-type-intf}

#description
Creates a rounded rectangle by specified parameters
::

::method-info
#method
circle
#overridings
(style: [ShapeStyleTypes]{.ts-type-intf}, center: [TPoint]{.ts-type-intf}, radius: [number]{.ts-base}) ⇨ [Circle]{.ts-type-intf}

#description
Creates a circle by specified parameters
::

::method-info
#method
line
#overridings
(style: [ShapeStyleTypes]{.ts-type-intf}, p0: [TPoint]{.ts-type-intf}, p1: [TPoint]{.ts-type-intf}) ⇨ [Line]{.ts-type-intf}

#description
Creates a line by specified parameters
::

::method-info
#method
vline
#overridings
(style: [ShapeStyleTypes]{.ts-type-intf}, p: [TPoint]{.ts-type-intf}, height: [number]{.ts-base}) ⇨ [VLine]{.ts-type-intf}

#description
Creates a vertical line by specified parameters
::

::method-info
#method
hline
#overridings
(style: [ShapeStyleTypes]{.ts-type-intf}, p: [TPoint]{.ts-type-intf}, width: [number]{.ts-base}) ⇨ [HLine]{.ts-type-intf}

#description
Creates a horizontal line by specified parameters
::

::method-info
#method
segmentline
#overridings
(style: [ShapeStyleTypes]{.ts-type-intf}, startPoint: [TPoint]{.ts-type-intf}) ⇨ [SegmentLine]{.ts-type-intf}

#description
Creates a line from segments line by specified parameters
::

::method-info
#method
setPixel
#overridings
(style: [ShapeStyleTypes]{.ts-type-intf}, point: [TPoint]{.ts-type-intf}) ⇨ [Pixel]{.ts-type-intf}

#description
Creates a pixel by specified parameters
::

::method-info
#method
draw
#overridings
(surface: [Surface]{.ts-class}) ⇨ [void]{.ts-base}

#description
Draws a sketch on the surface
::

::method-info
#method
toSurface
#overridings
(width?: [number]{.ts-base}, height?: [number]{.ts-base}, coordinateSystem?: [CoordinateSystem]{.ts-type-intf}) ⇨ [Surface]{.ts-class}

#description
Creates a surface from the sketch
::

::method-info
#method
toPattern
#overridings
(repetition: "repeat" | "repeat-x" | "repeat-y" | "no-repeat", width?: [number]{.ts-base}, height?: [number]{.ts-base}, coordinateSystem?: [CoordinateSystem]{.ts-type-intf}) ⇨ [Surface]{.ts-class}

#description
Creates a pattern from the sketch
::

::