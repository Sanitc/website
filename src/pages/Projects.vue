<template>
  <section id="projets" class="project-section">
    <v-container>
      <v-row>
        <v-col>
          <h1 class="space">Projets</h1>
        </v-col>
      </v-row>
      <v-row class="justify-space-around mb-8 mt-4">
        <Cards/>       
      </v-row>
    </v-container>
  </section>
</template>

<script>

import Cards from '@/components/Cards.vue'

export default {
   components: {
    Cards,
  },
}
</script>

<style scoped>
.project-section {
  background-color: #E7EAFB;
  padding-bottom: 17%;
}

.space{
  padding-bottom: 5%;
}
</style>
