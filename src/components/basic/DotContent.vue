<template>
  <div class="dot-content">
    <div class="flex">
      <div class="mx-1 my-2 h-0 w-0 border-2 border-blue-400"></div>
      <template v-if="content">
        <div class="text-sm">{{ content }}</div>
      </template>
      <slot v-else></slot>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    content: {
      type: String,
      default: '',
    },
  },
  components: {},
  setup() {
    
  },
}
</script>
