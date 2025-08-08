<script setup lang="ts" >
defineProps<{type: 'get' | 'set'}>()
</script>

<template>
  <div class="circle" :class="{ 'get': type === 'get', 'set': type === 'set' }">
    <slot />
  </div>
</template>

<style lang="sass" scoped>
.circle
  display: flex
  align-items: center
  justify-content: center
  padding: 4px
  border-radius: 50%
  &.get
    background-color: #005511
  &.set
    background-color: #001581
  span
    font-size: 10px
    color: #ccc
</style>