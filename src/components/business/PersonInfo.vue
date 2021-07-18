<template>
  <div class="basic-info">
    <div class="shadow-lg rounded-t-lg bg-blue-500 px-10 py-8 text-white">
      <div class="flex justify-between py-2 border-b border-blue-600 border-opacity-30">
        <div class="flex items-end">
          <div class="text-5xl tracking-wider">赵青松</div>
          <div class="text-2xl pl-2">Weedustzhao</div>
        </div>
        <div class="flex items-end">
          <div class="text-3xl">Web前端开发</div>
        </div>
      </div>
      <div class="flex justify-between py-2">
        <div class="flex flex-col justify-around">
          <div class="">男 / 1994.12</div>
          <div class="">重庆邮电大学 / 信息安全</div>
          <div class="">本科 / 2017年毕业</div>
        </div>
        <div class="flex flex-col justify-around items-end">
          <div>
            <a class="text-sm mr-2 text-white" href="https://weedust.com">https://weedust.com</a>
            <HomeIcon class="inline-block" />
          </div>
          <div>
            <a class="text-sm mr-2 text-white" href="https://github.com/ldc4">https://github.com/ldc4</a>
            <GithubIcon class="inline-block" />
          </div>
          <div>
            <sapn class="text-sm mr-2">ldc4#vip.qq.com</sapn>
            <EmailIcon class="inline-block" />
          </div>
          <div>
            <sapn class="text-sm mr-2">186****1335</sapn>
            <PhoneIcon class="inline-block" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import HomeIcon from '../icons/HomeIcon.vue'
import EmailIcon from '../icons/EmailIcon.vue'
import PhoneIcon from '../icons/PhoneIcon.vue'
import GithubIcon from '../icons/GithubIcon.vue'

export default {
  components: {
    HomeIcon,
    EmailIcon,
    PhoneIcon,
    GithubIcon,
  },
  setup() {
    
  },
}
</script>
