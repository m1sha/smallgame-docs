<script lang="ts" setup>
const route = useRoute()
const { data: page } = await useAsyncData(route.path, () => {
  return queryCollection('content').path(route.path).first()
})
</script>

<template>
  <div class="page-content">

    <div class="doc-menu-content">
      <h1>Documentation</h1>
      <DocMenu />
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

  .doc-menu-content
    padding: 8px
    border: 2px solid #3f3f3f
    border-radius: 4px
    width: clamp(170px, 10vw, 10vw)
    display: flex
    flex-direction: column
    h1
      align-self: center

  @media screen and (width < 600px) 
    &
      flex-direction: column
  

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
    
</style>