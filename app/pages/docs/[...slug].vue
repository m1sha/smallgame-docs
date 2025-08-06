<script lang="ts" setup>
const route = useRoute()
const { data: page } = await useAsyncData(route.path, () => {
  return queryCollection('content').path(route.path).first()
})
</script>

<template>
  <div>

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
    

    <ContentRenderer v-if="page" :value="page" />

    
  </div>
</template>
<style lang="sass">

.menu
  padding: 8px
  border: 1px solid #555
  width: 12vw
  a
    color: #ccc

  .router-link-active
    color: #559916

    
</style>