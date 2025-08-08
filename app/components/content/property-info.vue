<template>
<div class="property-info">
  <div class="prop-name">
    <span><slot name="name" /></span> 
    <span class="op-colon">:</span>
    <span><slot name="type" /></span> 
  </div>
  <div class="accessors">
    <slot name="accessors" />
    <!-- <div class="get">
      <span>get</span>
    </div>
    <div class="set" v-if="hasSetter">
      <span>set</span>
    </div> -->
  </div>
  <div>
    <slot name="description" />
  </div>

</div>
</template>

<style lang="sass" scoped>
.property-info
  display: flex
  gap: 12px
  padding: 8px
  border: 1px solid #555
  border-radius: 8px
  align-items: center

  .prop-name
    display: flex

  .accessors
    display: flex
    gap: 8px

</style>