---
title: "Size"
---

## Constructors

::list

::constructor-info
#name 
Size
#overridings
(value: [number]{.ts-base})<br>
(size: [TSize]{.ts-type-intf})<br>
(width: [number]{.ts-base}, height: [number]{.ts-base})
#description
Creates a new instance of the Size object
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
[get]{.ts-getter} [set]{.ts-setter}

#description
Gets or sets a width of the size object 
::

::property-info
#name
height
#type
[number]{.ts-base}
#accessors
[get]{.ts-getter} [set]{.ts-setter}

#description
Gets or sets a height of the size object 
::

::

<br>

## Methods

::list

::method-info
#method
scale [Self]{.ts-self}
#overridings
(value: [number]{.ts-base}) ⇨ [Size]{.ts-class}<br>
(size: [TSize]{.ts-type-intf}) ⇨ [Size]{.ts-class}<br>
(width: [number]{.ts-base}, height: [number]{.ts-base}) ⇨ [Size]{.ts-class}

#description
Scales the size object (size * value)
::

::method-info
#method
expand [Self]{.ts-self}
#overridings
(value: [number]{.ts-base}) ⇨ [Size]{.ts-class}<br>
(size: [TSize]{.ts-type-intf}) ⇨ [Size]{.ts-class}<br>
(width: [number]{.ts-base}, height: [number]{.ts-base}) ⇨ [Size]{.ts-class}

#description
Expands the size object (size + value)
::

::method-info
#method
inverse [Self]{.ts-self}
#overridings
() ⇨ [Size]{.ts-class}
(value: [number]{.ts-base}) ⇨ [Size]{.ts-class}<br>
(size: [TSize]{.ts-type-intf}) ⇨ [Size]{.ts-class}<br>
(width: [number]{.ts-base}, height: [number]{.ts-base}) ⇨ [Size]{.ts-class}

#description
Divides the transmitted value by the current value (value / size). If call without arguments (1 / size)
::

::method-info
#method
reset
#overridings
(value: [number]{.ts-base}) ⇨ [void]{.ts-base}<br>
(size: [TSize]{.ts-type-intf}) ⇨ [void]{.ts-base}<br>
(width: [number]{.ts-base}, height: [number]{.ts-base}) ⇨ [void]{.ts-base}

#description
Sets new values for the width and the height
::

::method-info
#method
equals
#overridings
(value: [number]{.ts-base}) ⇨ [boolean]{.ts-base}<br>
(size: [TSize]{.ts-type-intf}) ⇨ [boolean]{.ts-base}<br>
(width: [number]{.ts-base}, height: [number]{.ts-base}) ⇨ [boolean]{.ts-base}

#description
Checks if two sizes are equal
::

::method-info
#method
neg [Self]{.ts-self}
#overridings
() ⇨ [Size]{.ts-class}
(value: [number]{.ts-base}) ⇨ [Size]{.ts-class}<br>
(size: [TSize]{.ts-type-intf}) ⇨ [Size]{.ts-class}<br>
(width: [number]{.ts-base}, height: [number]{.ts-base}) ⇨ [Size]{.ts-class}

#description
Multiplies the size by minus one (size * -1)
::

::method-info
#method
negW [Self]{.ts-self}
#overridings
() ⇨ [Size]{.ts-class}
(value: [number]{.ts-base}) ⇨ [Size]{.ts-class}<br>
(size: [TSize]{.ts-type-intf}) ⇨ [Size]{.ts-class}<br>
(width: [number]{.ts-base}, height: [number]{.ts-base}) ⇨ [Size]{.ts-class}

#description
Multiplies the width by minus one (size.width * -1)
::

::method-info
#method
negH [Self]{.ts-self}
#overridings
() ⇨ [Size]{.ts-class}
(value: [number]{.ts-base}) ⇨ [Size]{.ts-class}<br>
(size: [TSize]{.ts-type-intf}) ⇨ [Size]{.ts-class}<br>
(width: [number]{.ts-base}, height: [number]{.ts-base}) ⇨ [Size]{.ts-class}

#description
Multiplies the height by minus one (size.height * -1)
::

::