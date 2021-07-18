<template>
  <div class="time-line-item">
    <div class="relative">
      <div class="absolute top-2 left-2 h-full w-0 border border-gray-200"></div>
      <div class="absolute bg-gray-200 rounded-full">
        <slot v-if="$slots.dot" name="dot"></slot>
        <ProjectIcon v-else />
      </div>
      <div class="relative -top-0.5 ml-6">
        <div>
          <slot name="header"></slot>
        </div>
        <div class="my-2">
          <slot></slot>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ProjectIcon from '../icons/ProjectIcon.vue'
export default {
  components: { ProjectIcon },
  setup() {
    
  },
}
</script>