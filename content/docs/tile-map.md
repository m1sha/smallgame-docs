---
title: "TileMap"
---

## Constructors

::list

::constructor-info
#name 
TileMap
#overridings
(tileWidth: [number]{.ts-base}, titleHight: [number]{.ts-base}, image: [HTMLImageElement]{.ts-class}, rect: [Rect]{.ts-class}, options?: [TileMapInitOptions]{.ts-class})
#description
Creates a new instance of the TileMap object
::

::

<br>

## Properties

::list

::property-info
#name
tileWidth
#type
[number]{.ts-base}
#accessors
[get]{.ts-getter}

#description
Gets the tile width
::

::property-info
#name
titleHight
#type
[number]{.ts-base}
#accessors
[get]{.ts-getter}

#description
Gets the tile hight
::

::property-info
#name
cols
#type
[number]{.ts-base}
#accessors
[get]{.ts-getter}

#description
Gets the number of columns
::

::property-info
#name
rows
#type
[number]{.ts-base}
#accessors
[get]{.ts-getter}

#description
Gets the number of rows
::

::

<br>

## Methods

::list

::method-info
#method
cell
#overridings
(col: [number]{.ts-base}) ⇨ [Surface]{.ts-class}<br>
(row: [number]{.ts-base}, col: [number]{.ts-base}) ⇨ [Surface]{.ts-class}
#description
Gets the tile image from the TileMap 
::

::