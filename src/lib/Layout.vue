<template>
  <div class="layout" >
    <slot></slot>
  </div>
</template>
<script>
export default {}
</script>
<style lang="scss" scoped>
.layout{
  display: flex;
  flex-grow: 1;
  flex-direction: column;
  border: 1px solid red;
  &.hasSider {
    flex-direction: row;
  }
}
</style>