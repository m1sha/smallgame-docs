---
title: "Text"
---

## Constructors

::list

::constructor-info
#name 
Text
#overridings
(content: [string]{.ts-base}, pos: [TextPosition]{.ts-type-intf}, style: [TTextStyle]{.ts-type-intf})
#description
Creates a new instance of the Text object
::

::

<br>

## Properties

::list

::property-info
#name
pos
#type
[Readonly]{.ts-class}<[TTextStyle]{.ts-type-intf}>
#accessors
[get]{.ts-getter}

#description
Gets the position of the Text object
::

::property-info
#name
style
#type
[TextStyle]{.ts-class}
#accessors
[get]{.ts-getter}

#description
Gets the style of the Text object
::

::

<br>

## Methods

::list

::method-info
#method
draw
#overridings
(suface: [Surface]{.ts-class}) ⇨ [void]{.ts-base}

#description
Draws the text on a suface
::

::