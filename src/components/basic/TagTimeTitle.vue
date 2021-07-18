<template>
  <div class="tag-time-title">
    <div class="flex items-center justify-between my-2">
      <div class="flex items-center">
        <div class="text-xs border px-1 rounded border-blue-500 text-blue-500 hover:text-white hover:bg-blue-500 cursor-pointer">{{tag}}</div>
        <div class="text-sm ml-2">{{title}}</div>
      </div>
      <div class="text-sm">{{time}}</div>
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
    title: {
      type: String,
      default: '',
    },
    time: {
      type: String,
      default: '',
    },
  },
  components: {},
  setup() {
    
  },
}
</script>
