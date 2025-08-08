<template>
  <div class="constructor-info doc-article">
    <div class="constructor-signature">
      <div class="constructor-name"> 
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
  border: 2px solid #3f3f3f
  border-radius: 4px
  border-radius: 8px
  .constructor-signature
    display: flex
    gap: 4px
    width: 100%
    .constructor-name
      display: flex
  

</style>