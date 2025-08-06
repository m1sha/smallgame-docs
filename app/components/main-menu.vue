<script lang="ts" setup>
const route = useRoute()
const imActive = computed(() => route.path.indexOf('/docs') > -1)
</script>

<template>
  <menu class="main-menu">
    <ul>
      <li>
        <NuxtLink to="/">Home</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/docs/" :class="{'router-link-active': imActive }">Docs</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/">Tutorial</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/">Examples</NuxtLink>
      </li>
    </ul>
  </menu>
</template>

<style lang="sass">
.main-menu
  display: flex
  justify-content: center
  width: 100%
  ul
    display: flex
    padding: 0
    gap: 4px
    li
      a
        padding: 6px 12px
        color: #ccc
        text-decoration: none
        font-size: 1.2em
        border-bottom: 2px solid #595959
        border-radius: 1px
        &:is(.router-link-active)
          border-color: #18b338
</style>