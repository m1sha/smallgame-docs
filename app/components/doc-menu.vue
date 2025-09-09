<template>
  <menu class="doc-menu">
    <ul>
      <li>
        <div class="selector" />
        <NuxtLink to="/docs/">Introdution</NuxtLink>
      </li>
      <li>
        <div class="selector" />
        <NuxtLink to="/docs/installation">Installation</NuxtLink>
      </li>
      <li>
        <div class="selector" />
        <NuxtLink to="/docs/get-started">Get Started</NuxtLink>
      </li>
      <li>
        <div class="selector" />
        <NuxtLink to="/docs/animation">Animation</NuxtLink></li>
      <li>
        <div class="selector" />
        <NuxtLink to="/docs/animator">Animator</NuxtLink></li>
      <li>
        <div class="selector" /> 
        <NuxtLink to="/docs/transition">AnimationTransition</NuxtLink></li>
      <li>
        <div class="selector" />
        <NuxtLink to="/docs/assets">Assets</NuxtLink></li>
      <li>
        <div class="selector" />
        <NuxtLink to="/docs/game">Game</NuxtLink></li>
      <li>
        <div class="selector" />
        <NuxtLink to="/docs/game-events">GameEvents</NuxtLink></li>
      <li>
        <div class="selector" />
        <NuxtLink to="/docs/gameloop">gameloop</NuxtLink></li>
       <li>
        <div class="selector" /> 
        <NuxtLink to="/docs/group">Group</NuxtLink></li>
      <li>
        <div class="selector" /> 
        <NuxtLink to="/docs/keys">Keys</NuxtLink></li>
      <li>
        <div class="selector" /> 
        <NuxtLink to="/docs/pixel-mask">PixelMask</NuxtLink></li>
      <li>
        <div class="selector" /> 
        <NuxtLink to="/docs/point">Point</NuxtLink></li>
       <li>
        <div class="selector" /> 
        <NuxtLink to="/docs/rect">Rect</NuxtLink></li>
      <li>
        <div class="selector" /> 
        <NuxtLink to="/docs/shape-style">ShapeStyle</NuxtLink></li>
      <li>
        <div class="selector" /> 
        <NuxtLink to="/docs/size">Size</NuxtLink></li>
      <li>
        <div class="selector" /> 
        <NuxtLink to="/docs/sketch">Sketch</NuxtLink></li>
      <li>
        <div class="selector" /> 
        <NuxtLink to="/docs/sprite">Sprite</NuxtLink></li>
      <li>
        <div class="selector" /> 
        <NuxtLink to="/docs/surface">Surface</NuxtLink></li>
      <li>
        <div class="selector" /> 
        <NuxtLink to="/docs/text-style">TextStyle</NuxtLink></li>
      <li>
        <div class="selector" /> 
        <NuxtLink to="/docs/text">Text</NuxtLink></li>
      <li>
        <div class="selector" /> 
        <NuxtLink to="/docs/tile-map">TileMap</NuxtLink></li>
      <li>
        <div class="selector" /> 
        <NuxtLink to="/docs/time">Time</NuxtLink></li>
      
    </ul>
  </menu>
</template>

<style lang="sass" scoped>
.doc-menu
  overflow: auto
  @media screen and (width < 600px)
    &
      height: 10vh
  ul
    li
      display: flex
      gap: 2px
      padding: 4px
      a
        display: flex
        color: #ccc
        width: 100%
        padding-left: 4px
        font-size: 1.1em
      .selector
        width: 4px
        height: auto
      &:has(>.router-link-active)
        background-color: #383838
        border-radius: 3px
        a
          color: #fff
        .selector
          background-color: #119911
    
</style>