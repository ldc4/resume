<template>
  <div class="exp-list">
    <Container title="工作经历">
      <div class="my-4">
        <TagTimeTitle tag="工作" title="腾讯 / WXG / 微信支付研发部" time="2019.09 ~ 至今" />
        <DotContent content="负责需求管理系统2.0的web全栈开发" />
      </div>
      <div class="my-4">
        <TagTimeTitle tag="工作" title="腾讯 / CSIG / 云服务平台部" time="2018.10 ~ 2019.09" />
        <DotContent content="负责腾讯云控制台-云监控的web前端开发" />
      </div>
      <div class="my-4">
        <TagTimeTitle tag="工作" title="腾讯 / SNG / 社交网络运营部" time="2017.07 ~ 2018.09" />
        <DotContent content="负责织云（商业版）的框架、组件和部分业务的web前端开发" />
      </div>
    </Container>
  </div>
</template>

<script>
import DotContent from '../basic/DotContent.vue'
import TagTimeTitle from '../basic/TagTimeTitle.vue'
import Container from '../basic/Container.vue'

export default {
  components: {
    TagTimeTitle,
    DotContent,
    Container,
  },
  setup() {

  },
}
</script>
