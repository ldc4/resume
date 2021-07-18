<template>
  <div class="tag-time-title">
    <div class="flex items-center justify-between my-2">
      <div class="flex items-center">
        <div class="text-base mr-2 font-medium">{{title}}</div>
        <div class="text-xs cursor-pointer">
          <a
            v-if="linkHref"
            :href="linkHref"
            target="_blank"
            class="border rounded border-blue-500 text-blue-500 hover:text-white hover:bg-blue-500 px-1"
          >{{linkTitle}}</a>
          <template v-else>{{linkTitle}}</template>
        </div>
      </div>
      <div class="text-sm">{{time}}</div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    linkTitle: {
      type: String,
      default: '',
    },
    linkHref: {
      type: String,
      default: ''
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
