<template>
  <Layout>
    <About/>
    <Projects/>
    <Skill/>
    <Education />
  </Layout>
</template>

<script>
import About from '@/pages/About.vue'
import Projects from '@/pages/Projects.vue'
import Skill from '@/pages/Skill.vue'
import Education from '@/pages/Education.vue'


export default {
  metaInfo: {
    title: 'Portefolio'
  },
  components: {
    About,
    Projects,
    Skill,
    Education,
  }
}
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
</style>
