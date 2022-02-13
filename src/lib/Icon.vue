<template>
 <svg class="icon">
  <use :xlink:href="`#icon-${icon}`"></use>
</svg>
</template>

<script>
export default {
  props:{
    icon:{
      type:String,
    }
  }
}
</script>