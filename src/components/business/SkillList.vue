<template>
  <div class="skill-list">
    <Container title="专业技能">
      <DotContent class="my-4" content="掌握Web全栈开发的相关技能，重视用户体验与代码可维护性，有4年多的前端开发工作经验。" />
      <DotContent class="my-4" content="对MV*框架，例如Vue、React、Angular有着较熟练的实践和较深刻的感悟。" />
      <DotContent class="my-4" content="对ES6、NodeJS、前端工程化、性能优化、模块加载、构建平台框架、UI组件等有一定的了解和思考。" />
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