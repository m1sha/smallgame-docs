---
title: "AnimationTransition"
---

## Properties

::list

::property-info
#name
from
#type
[string]{.ts-base}
#accessors
[get]{.ts-getter} [set]{.ts-setter}

#description
The name of the start animation
::

::property-info
#name
to
#type
[string]{.ts-base}
#accessors
[get]{.ts-getter} [set]{.ts-setter}

#description
The name of the transition animation
::

::property-info
#name
trigger
#type
[AnimationTriggerCallback]{.ts-type-intf}
#accessors
[get]{.ts-getter} [set]{.ts-setter}

#description
The function that determines the transition to the next animation
::

::property-info
#name
flipX
#type
[AnimationTriggerCallback]{.ts-type-intf}
#accessors
[get]{.ts-getter} [set]{.ts-setter}

#description
The function that determines the need for an x-axis flip
::

::property-info
#name
flipY
#type
[AnimationTriggerCallback]{.ts-type-intf}
#accessors
[get]{.ts-getter} [set]{.ts-setter}

#description
The function that determines the need for an y-axis flip
::

::

<br>An Example:
<br>In the code below show how to add a [Transition]{.ts-type-intf} to an [Animator]{.ts-class} in the method **create** in the [Hero]{.ts-class} class

```ts
class Hero extends Sprite { 
  ...

  async create () {
    ...
    animator.addTransition({
      from: 'idle',
      to: 'dead',
      trigger: () => this.health <= 0,
      flipX: () => this.isFlipped
    })
  }
}
```