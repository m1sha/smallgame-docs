<template>
  <div class="constructor-info doc-article">
    <div class="constructor-signature">
      <div class="constructor-name"> 
        <span class="ts-class"> <slot name="class-name" /></span>
        <span class="op-dot">.</span>
        <span class="ts-method"> <slot name="method" /></span>
      </div>
      <div>
       <slot name="overridings" />
      </div>
    </div>

    <div>
      <slot name="description" />
    </div>
  </div>
</template>

<style lang="sass" scoped>
.constructor-info
  display: flex
  flex-direction: column
  gap: 12px
  padding: 8px
  border: 1px solid #555
  border-radius: 8px
  .constructor-signature
    display: flex
    gap: 4px
    width: 100%
    .constructor-name
      display: flex
  

</style>