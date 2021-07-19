<template>
  <div class="a4-paper">
    <div class="mx-auto" :style="{ width, height }">
      <div class="h-1/6">
        <slot name="header"></slot>
      </div>
      <div class="h-5/6 shadow-lg rounded-b-lg bg-gray-50 p-6">
        <slot name="body"></slot>
      </div>
    </div>
  </div>
</template>

<script>
import { reactive, ref, computed } from 'vue'

const paperSizeMap = {
  'A4': {
    height: `${Math.SQRT2 * 1024}px`,
    width: '1024px',
  }
}

export default {
  setup() {
    const type = ref('A4');

    const width = computed(() => {
      return paperSizeMap[type.value].width;
    });
    const height = computed(() => {
      return paperSizeMap[type.value].height;
    })

    return reactive({
      width,
      height
    })
  },
}
</script>