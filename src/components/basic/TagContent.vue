<template>
  <div class="tag-content">
    <div class="flex items-start">
      <div class="flex-shrink-0 text-sm border px-1 rounded bg-gray-100">{{tag}}</div>
      <div class="flex-shrink-0 text-sm">：</div>
      <div class="text-sm">
        <template v-if="content">
          <div>{{ content }}</div>
        </template>
        <slot v-else></slot>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    tag: {
      type: String,
      default: '',
    },
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
