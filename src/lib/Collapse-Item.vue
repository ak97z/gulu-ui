<template>
  <div class="collapseItem">
    <div class="title" @click=toggle>
      {{ title }}
    </div>
    <div class="content" v-if="open">
      <slot></slot>
    </div>
  </div>
</template>
<script>
export default {
  props: {
    title: String,
  },
  data() {
    return {
      open: false,
    }
  },

  methods: {
    toggle () {
      this.open = !this.open;
    },
    close () {
      this.open = false
    }
  },
}
</script>
<style lang="scss" scoped>
$grey: #ddd;
$border-radius: 4px;
.collapseItem {
  > .title {
    border: 1px solid $grey;
    margin-top: -1px;
    margin-left: -1px;
    margin-right: -1px;
    min-height: 32px;
    display: flex;
    align-items: center;
    padding: 0 8px;
  }
  &:first-child {
    > .title {
      border-top-left-radius: $border-radius;
      border-top-right-radius: $border-radius;
    }
  }
  &:last-child {
    > .title:last-child {
      border-bottom-left-radius: $border-radius;
      border-bottom-right-radius: $border-radius;
    }
  }
  > .content {
    padding: 8px;
  }
}
</style>