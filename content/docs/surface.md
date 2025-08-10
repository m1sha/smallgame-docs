---
title: "Surface"
---

## Constructors

::list

::constructor-info
#name 
Surface
#overridings
(width: [number]{.ts-base}, height: [number]{.ts-base}, options?: [SurfaceCreateOptions]{.ts-type-intf}, canvas?: [HTMLCanvasElement]{.ts-type-intf})<br>

#description
Creates a new instance of the surface with certain parameters
::

::static-method-info
#class-name
Surface
#method
fromImage
#overridings
(image: [HTMLImageElement]{.ts-type-intf} | [ImageBitmap]{.ts-type-intf}, rect: [TRect]{.ts-type-intf}, options?: [SurfaceCreateOptions]{.ts-type-intf})
#description
Creates a new instance of surface from an image
::

::static-method-info
#class-name
Surface
#method
fromImages
#overridings
(image: [HTMLImageElement]{.ts-type-intf}\[],  rect: [TRect]{.ts-type-intf}, rows: [number]{.ts-base} = 1, cols: [number]{.ts-base} = -1, options?: [SurfaceCreateOptions]{.ts-type-intf})
#description
Creates a new instance of surface from an images
::

::static-method-info
#class-name
Surface
#method
fromCanvas
#overridings
(canvas: [HTMLCanvasElement]{.ts-type-intf}, options?: [SurfaceCreateOptions]{.ts-type-intf})
#description
Creates a new instance of surface from an exist canvas
::

::static-method-info
#class-name
Surface
#method
default
#overridings

#description
Creates a new instance of surface with 1x1px size
::

::static-method-info
#class-name
Surface
#method
combine
#overridings
(surfaces: [ISurface]{.ts-type-intf}\[], rows: [number]{.ts-base} = 1, cols: [number]{.ts-base} = -1, options?: [SurfaceCreateOptions]{.ts-type-intf})
#description
Combines surfaces in new instance of surface
::

::

<br>

## Properties

::list

::property-info
#name
width
#type
[number]{.ts-base}
#accessors
[get]{.ts-getter} 

#description
Gets a width of the surface
::

::property-info
#name
height
#type
[number]{.ts-base}
#accessors
[get]{.ts-getter} 

#description
Gets a height of the surface
::

::property-info
#name
rect
#type
[TRect]{.ts-type-intf}
#accessors
[get]{.ts-getter} 

#description
Gets a distribute rect of the surface
::

::property-info
#name
imageRendering
#type
'auto' | 'pixelated'
#accessors
[get]{.ts-getter} [set]{.ts-setter} 

#description
Gets or sets an image scaling method linear interpolation or nearest neighbor
::

::property-info
#name
pixels
#type
[Pixels]{.ts-class}
#accessors
[get]{.ts-getter} 

#description
Gets object for a pixel manipulation
::

::property-info
#name
draw
#type
[Draw]{.ts-class}
#accessors
[get]{.ts-getter} 

#description
Gets object for a draw (Not recommended use this property directly)
::

::

<br>

## Methods

::list

::method-info
#method
clear
#overridings
(rect?: [TRect]{.ts-type-intf}) ⇨ [void]{.ts-base}
#description
Clears a surface
::

::method-info
#method
fill
#overridings
(color: [string]{.ts-base}) ⇨ [void]{.ts-base}
#description
Fills a surface a specified color
::

::method-info
#method
blit
#overridings
(surface: [ISurface]{.ts-type-intf}, rect: [TRect]{.ts-type-intf} | [TPoint]{.ts-type-intf}, srcRect?: [TRect]{.ts-type-intf}) ⇨ [void]{.ts-base}
#description
Copies a specified surface bitmap on the current surface in specified rect
::

::method-info
#method
blita
#overridings
(alpha: [number]{.ts-base}, surface: [ISurface]{.ts-type-intf}, rect: [TRect]{.ts-type-intf} | [TPoint]{.ts-type-intf}, srcRect?: [TRect]{.ts-type-intf}) ⇨ [void]{.ts-base}
#description
Copies a specified surface bitmap on the current surface in specified rect
::

::method-info
#method
extract
#overridings
(rect: [TRect]{.ts-type-intf}) ⇨ [void]{.ts-base}
#description
Creates new instance of the surface by extracted a specified rectangle from original surface
::

::method-info
#method
zoom
#overridings
(index: [number]{.ts-base}) ⇨ [void]{.ts-base}
#description
Scales the surface by both axises in a specified value
::

::method-info
#method
flip
#overridings
(position: 'x' | 'y' | 'xy') ⇨ [void]{.ts-base}
#description
Flips the surface in a specified position
::

::method-info
#method
rotate
#overridings
(deg: [number]{.ts-base}, pivote?: [TPivote]{.ts-type-intf}) ⇨ [void]{.ts-base}
#description
Rotates the surface in a specified angle
::

::method-info
#method
resize
#overridings
(width: [number]{.ts-base}, height: [number]{.ts-base}) ⇨ [void]{.ts-base}
#description
Resizes the surface in a specified width and height
::

::method-info
#method
setCanvasSize
#overridings
(width: [number]{.ts-base}, height: [number]{.ts-base}, shiftToCenter: [boolean]{.ts-base} = true) ⇨ [void]{.ts-base}
#description
Sets a canvas size of the surface a specified width and height
::

::method-info
#method
mix
#overridings
(method: [GlobalCompositeOperation]{.ts-type-intf}, surface: [ISurface]{.ts-type-intf}, rect: [TRect]{.ts-type-intf} | [TPoint]{.ts-type-intf}, srcRect?: [TRect]{.ts-type-intf}) ⇨ [void]{.ts-base}
#description
Does composite operation on the original surface
::

::method-info
#method
createImage
#overridings
(type: [string]{.ts-base}, quality: [any]{.ts-base}) ⇨ [Promise<HTMLImageElement>]{.ts-type-intf}
#description
Create a HTML image element from the surface
::

::method-info
#method
toDataURL
#overridings
(type: [string]{.ts-base}, quality: [any]{.ts-base}) ⇨ [string]{.ts-base}
#description
Create a data URL from the surface
::

::method-info
#method
toPattern
#overridings
(type: repetition: "repeat" | "repeat-x" | "repeat-y" | "no-repeat") ⇨ [CanvasPattern]{.ts-type-intf}
#description
Creates a pattern from the surface
::

::method-info
#method
toBitmap
#overridings
() ⇨ [Bitmap]{.ts-type-intf}
#description
Creates a bitmap from the surface
::

::method-info
#method
save
#overridings
(type: [string]{.ts-base}, quality: [any]{.ts-base}) ⇨ [Promise<Blob | null>]{.ts-type-intf}
#description
Creates a Blob object from the surface
::

::method-info
#method
createMask
#overridings
() ⇨ [PixelMask]{.ts-class}
#description
Creates a pixel mask object from the surface
::

::method-info
#method
clone
#overridings
() ⇨ [Surface]{.ts-class}
#description
Creates a copy of the original surface
::

::