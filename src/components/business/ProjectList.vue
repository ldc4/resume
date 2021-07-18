<template>
  <div class="project-list">
    <Container title="主要工作项目">
      <TimeLine>
        <TimeLineItem>
          <template v-slot:header>
            <LinkTimeTitle
              title="需求管理系统2.0"
              linkTitle="内网"
              linkHref="https://weedust.com/"
              time="2019.09 - 至今"
            />
          </template>
          <template v-slot>
            <Card>
              <TagContent tag="项目描述">
                需求管理系统是微信支付的业务架构师团队为了实现需求的结构化输出，核心实现逻辑沉淀、支持UAT自动化测试保证支付业务质量的需求管理平台。涵盖了微信支付的商业支付、用户支付、业务增值等一系列业务的需求逻辑描述。
                在微信支付复杂的业务需求和多团队协作中，大家共同维护自助查阅，减少沟通成本和对系统不了解带来的研发质量风险。同时结构化需求对接自动化UAT测试平台，生成自动化测试脚本，在开发测试和定时批跑执行时使用，保障支付业务的稳定性。
              </TagContent>
              <TagContent class="pt-2" tag="主要职责">
                <DotContent>
                  该项目团队结构：1个项目负责人，2个产品，4个全栈开发，2个外包。
                </DotContent>
                <DotContent>
                  负责需求管理系统的Web全栈开发，掌握每一个开发环节（DB、Dao层、Node应用层express、前端Vue2、前端组件element-ui、构建部署、自动化测试、运营系统、定时任务等）
                </DotContent>
                <DotContent>
                  负责系统中高频使用的子模块（补充约束-业务规则）和其他公共模块的迭代开发、维护、CR、运营等
                </DotContent>
                <DotContent>
                  团队内实行精益迭代（按双周），除了交付需求之外，还涉及一些其他技术事项：技术债务清理（重构）、前端后端性能优化、排查内存溢出、微服务拆分等
                </DotContent>
              </TagContent>
            </Card>
          </template>
        </TimeLineItem>
        <TimeLineItem>
          <template v-slot:header>
            <LinkTimeTitle
              title="腾讯云控制台 - 云监控"
              linkTitle="console.cloud.tencent.com/monitor"
              linkHref="https://console.cloud.tencent.com/monitor"
              time="2018.10 - 2019.09"
            />
          </template>
          <template v-slot>
            <Card>
              <TagContent tag="项目描述">
                云监控为用户提供了统一监控云服务器、云数据库等所有云产品的平台。可以通过使用云监控全面了解云产品资源使用率、应用程序性能和云产品运行状况，云监控还支持多指标监控、自定义告警、跨地域和跨项目实例分组、自定义监控、可视化Dashboard等功能。
              </TagContent>
              <TagContent class="pt-2" tag="主要职责">
                <DotContent>
                  负责云监控web前端的迭代需求开发
                </DotContent>
                <DotContent>
                  保障现网的稳定运行，及时处理Web页面相关问题
                </DotContent>
                <DotContent>
                  负责前端页面接入（SDK形式），支撑好其他云产品接入云监控的相关工作
                </DotContent>
              </TagContent>
            </Card>
          </template>
        </TimeLineItem>
        <TimeLineItem>
          <template v-slot:header>
            <LinkTimeTitle
              title="织云（商业版）"
              linkTitle="私有云部署"
              linkHref="https://cloud.tencent.com/developer/column/1056"
              time="2017.07 - 2018.09"
            />
          </template>
          <template v-slot>
            <Card>
              <TagContent tag="项目描述">
                织云是SNG内部运营多年的运维自动化能力，进行toB市场化的推广的产物，是一站式的运维平台。经历几个大版本迭代，同时孵化出uweb平台框架、应用框架和UI组件库。
              </TagContent>
              <TagContent class="pt-2" tag="主要职责">
                <DotContent>
                  负责织云的平台框架 ( uweb-platform ) 开发，版本迭代管理，公共能力建设
                </DotContent>
                <DotContent>
                  负责织云的应用框架 ( uweb-app ) 开发，部分业务模块开发
                </DotContent>
                <DotContent>
                  辅导新的前端成员及其技术指导，并帮助中心同学的更多项目实践与接入平台
                </DotContent>
              </TagContent>
            </Card>
          </template>
        </TimeLineItem>
      </TimeLine>
    </Container>
  </div>
</template>

<script>
import Container from '../basic/Container.vue'
import TimeLine from '../basic/TimeLine.vue'
import TimeLineItem from '../basic/TimeLineItem.vue'
import Card from '../basic/Card.vue'
import LinkTimeTitle from '../basic/LinkTimeTitle.vue'
import TagContent from '../basic/TagContent.vue'
import DotContent from '../basic/DotContent.vue'

export default {
  components: {
    Container,
    TimeLine,
    TimeLineItem,
    Card,
    LinkTimeTitle,
    TagContent,
    DotContent,
  },
  setup() {
    
  },
}
</script>