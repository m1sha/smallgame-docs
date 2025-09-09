---
title: "Group"
---

The class Group need for storing sprites

## Constructors

::list

::constructor-info
#name 
Group 
#overridings
\<T [extends]{.keyword} [Sprite]{.ts-class}> ()
#description
Creates a new instance of the sprite group
::

::

<br>

## Properties

::list

::property-info
#name
sprites
#type
[number]{.ts-base}
#accessors
[get]{.ts-getter} 

#description
Gets all sprites of the group
::

::property-info
#name
useCollisionHashmap
#type
[number]{.ts-base}
#accessors
[get]{.ts-getter} 

#description
Uses hashmap algorithm for collide operations
::

::property-info
#name
useSpriteCollideRect
#type
[number]{.ts-base}
#accessors
[get]{.ts-getter} 

#description
Uses a sprite collider instead sprite rect for collide operations
::

::

<br>

## Methods

::list

::method-info
#method
add
#overridings
(sprite: T) ⇨ [void]{.ts-base}
#description
Adds a sprite to the group
::

::method-info
#method
remove
#overridings
(sprite: T) ⇨ [void]{.ts-base}
#description
Removes a sprite from the group
::

::method-info
#method
has
#overridings
(sprite: T) ⇨ [boolean]{.ts-base}
#description
Checks for existing a sprite in the group
::

::method-info
#method
find
#overridings
(predicate: (sprite: T) ⇨ [boolean]{.ts-base}) ⇨ T | [undefined]{.ts-base}
#description
Finds a sprite in the group
::

::method-info
#method
collidePoint
#overridings
(point: [TPoint]{.ts-type-intf}, callback: (sprite: T) ⇨ [void]{.ts-base}) ⇨ [void]{.ts-base}
#description
Checks collide any sprite a point in the group
::

::method-info
#method
collideSprite
#overridings
\<R [extends]{.keyword} [Sprite]{.ts-class}> (sprite: R, callback: (sprite: T) ⇨ [void]{.ts-base}) ⇨ [void]{.ts-base}
#description
Checks collide a sprite any sprite in the group
#example
<br>Example:
```ts
const enemies = new Group<Enemy>()
const hero = new Hero()

enemies.collideSprite(hero, enemy => {
  // an enemy is colliding the hero
})

```
::

::method-info
#method
collideGroup
#overridings
\<R [extends]{.keyword} [Sprite]{.ts-class}> (group: [Group]{.ts-class}\<R>, callback: (sprite1: T, sprite2: R) ⇨ [void]{.ts-base}) ⇨ [void]{.ts-base}
#description
Checks collide a sprite group any sprite in the group
#example
<br>Example:
```ts
const balls = new Group<Ball>()
const bricks = new Group<Brick>()

balls.collideGroup(bricks, (ball, brick) => {
  // a ball is colliding a brick
})

```
::

::method-info
#method
outsideRect
#overridings
(rect: [TRect]{.ts-type-intf}, callback: (sprite: T) ⇨ [void]{.ts-base}) ⇨ [void]{.ts-base}
#description
Checks any sprite in the group is outside of the rectangle
::

::method-info
#method
draw
#overridings
()
#description
Draws all sprites in the group
::

::method-info
#method
[protected]{.keyword} update
#overridings
()
#description
The update method calls before the draw method in children classes
::

::