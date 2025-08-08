<template>
  <div class="list-of-items">
    <slot />
  </div>
</template>

<style lang="sass" scoped>
.list-of-items
  display: flex
  flex-direction: column
  gap: 4px
</style>