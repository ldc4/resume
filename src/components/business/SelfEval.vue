<template>
  <div class="self-eval">
    <Container title="自我评价">
      <DotContent class="my-4" content="有着良好的工作心态和友善的性格，能够快速融入各项工作与团队中。" />
      <DotContent class="my-4" content="能够很好的理解和沟通产品需求，并按时按质的落地；及时处理各类现网问题，保障产品稳定运行。" />
      <DotContent class="my-4" content="涉猎的技术范围广，对新技术保持着主动学习的热情；对技术原理和实现保持钻研、精益求精的开发精神。" />
    </Container>
  </div>
</template>

<script>
import DotContent from '../basic/DotContent.vue'
import Container from '../basic/Container.vue'

export default {
  components: {
    DotContent,
    Container,
  },
  setup() {
    
  },
}
</script>