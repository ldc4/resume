<template>
  <div class="basic-container">
    <div class="container">
      <div class="flex items-center">
        <div class="flex-grow">
          <div class="h-0 border-b mr-2"></div>
        </div>
        <div class="bg-gray-200 px-8 py-0.5 rounded-full font-medium">{{title}}</div>
        <div class="flex-grow">
          <div class="h-0 border-b ml-2"></div>
        </div>
      </div>
      <div class="my-4">
        <slot></slot>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: {
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
