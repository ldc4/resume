<template>
  <div class="app">
    <div class="w-screen bg-gray-200">
      <A4>
        <template v-slot:header>
          <PersonInfo />
        </template>
        <template v-slot:body>
          <div class="flex">
            <ExpList class="p-2 w-1/2" />
            <SkillList class="p-2 w-1/2" />
          </div>
          <ProjectList />
          <SelfEval />
        </template>
      </A4>
    </div>
  </div>
  
</template>

<script>
import A4 from './components/layout/A4.vue'
import PersonInfo from './components/business/PersonInfo.vue'
import SkillList from './components/business/SkillList.vue'
import ExpList from './components/business/ExpList.vue'
import ProjectList from './components/business/ProjectList.vue'
import SelfEval from './components/business/SelfEval.vue'

export default {
  components: {
    A4,
    PersonInfo,
    SkillList,
    ExpList,
    ProjectList,
    SelfEval,
  },
  setup() {

  }
}
</script>

<style>

</style>
