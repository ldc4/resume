<template>
  <div class="app">
    <div class="w-screen bg-gray-200 py-16">
      <A4 id="a4">
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

    onkeydown = function(e) {
      if (
        (e.ctrlKey && e.keyCode == 'P'.charCodeAt(0)) ||
        (e.metaKey && e.keyCode == 'P'.charCodeAt(0))
      ) {
        e.preventDefault();
        printA4();
      }
    }

    const printA4 = () => {
      console.log('打印')
      const a4DOM = document.getElementById('a4');
      const bodyInnerHTML = document.body.innerHTML;
      window.document.body.innerHTML = a4DOM.innerHTML;
      window.print();
      window.document.body.innerHTML = bodyInnerHTML;
      return false;
    }

    return {
      printA4
    }
  }
}
</script>

<style>

</style>
