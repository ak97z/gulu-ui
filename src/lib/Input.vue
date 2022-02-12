<template>
  <input :value="value" type="text" :disabled="disabled" :readonly="readonly"/>
  <template v-if="error">
    <Icon icon="error" class="gulu-icon-error"/>
    <span class="gulu-errorMessage">{{error}}</span>
  </template>
</template>

<script>
import Icon from "../components/Icon.vue";

export default {
  components: {Icon},
  props: {
    value:{
      type:String
    },
    disabled:{
      type:Boolean,
      default:false,
    },
    readonly:{
      type:Boolean,
      default:false,
    },
    error: {
      type: String,
    },
  }
}
</script>