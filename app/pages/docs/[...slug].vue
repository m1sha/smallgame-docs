<script lang="ts" setup>
const route = useRoute()
const { data: page } = await useAsyncData(route.path, () => {
  return queryCollection('content').path(route.path).first()
})
</script>

<template>
  <div class="page-content">

    <div class="menu">
      <h1>Documentation</h1>
      <menu>
        <ul>
          <li>
            <NuxtLink to="/docs/">Introdution</NuxtLink>
          </li>
          <li>
            <NuxtLink to="/docs/installation">Installation</NuxtLink>
          </li>
          <li>
            <NuxtLink to="/docs/get-started">Get Started</NuxtLink>
          </li>
          <li><NuxtLink to="/docs/game">Game</NuxtLink></li>
          <li><NuxtLink to="/docs/surface">Surface</NuxtLink></li>
          <li><NuxtLink to="/docs/sprite">Sprite</NuxtLink></li>
          <li><NuxtLink to="/docs/sketch">Sketch</NuxtLink></li>
          <li><NuxtLink to="/docs/rect">Rect</NuxtLink></li>
          <li><NuxtLink to="/docs/point">Point</NuxtLink></li>
        </ul>
      </menu>
    </div>
    
    <article>
      <h1 v-if="page">{{ page.title }}</h1>
    <ContentRenderer v-if="page" :value="page" />
    </article>

    
  </div>
</template>
<style lang="sass">
.page-content
  display: flex
  gap: 1.2em
  padding: 2em 1.2em
  padding-right: .6em
  width: 100%

  article
    overflow: auto
    height: calc-size(auto, size) //calc( 100vh -  10em)
    flex: 1
    padding-right: .6em
    scroll-padding-bottom: 20px
    h1, h2
      position: sticky
      top: 0
      background-color: #333
      margin: 0
      padding: 8px 0
    h1
      z-index: 1
    h2
      top: calc( 1.6em + 8px )
      z-index: 2

.menu
  padding: 8px
  border: 2px solid #3f3f3f
  border-radius: 4px
  width: clamp(8vw, 12vw, 12vw)
  a
    color: #ccc

  .router-link-active
    color: #559916

    
</style>