<template>
  <Layout>
    <About />
    <Projects/>
    <Skill/>
    <Education />
    <Contact />
  </Layout>
</template>

<script>
import About from '@/components/About.vue'
import Projects from '@/components/Projects.vue'
import Skill from '@/components/Skill.vue'
import Education from '@/components/Education.vue'
import Contact from '@/components/Contact.vue'

export default {
  metaInfo: {
    title: 'Portefolio'
  },
  components: {
    About,
    Projects,
    Skill,
    Education,
    Contact
  }
}
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
</style>
