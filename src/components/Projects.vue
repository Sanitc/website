<template>
  <section id="projet" class="project-section">
    <v-container>
      <v-row>
        <v-col>
          <h1>Projet</h1>
        </v-col>
      </v-row>
      <v-row class="justify-space-around mb-8 mt-4">
        <v-card
          v-for="project in projects"
          :key="project.name"
          class=""
          max-width="300"
          
        >
          <v-img
            class="align-end"
            height="250px"
            :src="project.image"
          />
          <v-card-title>{{ project.name }}</v-card-title>

          <v-card-text>
            {{ truncate(project.description) }}
          </v-card-text>

          <v-card-actions>
            <v-btn
              color="black"
              text
              :href="project.github" target="_blank"
            >
              Dépot Github
            </v-btn>

          </v-card-actions>
        </v-card>
      </v-row>
    </v-container>
  </section>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        {
          name: 'Phoïkos',
          github: 'https://github.com/Sanitc/phoikos',
          description: "Cette application permettra de retrouver des magasins éco-responsable dans Rennes, et donnera des conseils afin de reduire son impact écologique.",
          image: 'https://raw.githubusercontent.com/Sanitc/phoikos/master/assets/images/logo/%C3%A9t%C3%A9.png'
        },
        {
          name: 'Portefolio',
          github: 'https://github.com/Sanitc/phoikos',
          description: "Portefolio réalisé en Vue.js afin d'apprendre ce framework",
          image: 'https://raw.githubusercontent.com/Sanitc/phoikos/master/assets/images/logo/%C3%A9t%C3%A9.png'
        },
      ]
    }
  },
  methods: {
    truncate(str) {
      if (str.length > 145) {
        return str.slice(0, 79) + '...'
      }
      return str
    }
  }
}
</script>

<style scoped>
.project-section {
  background-color: #FFE58F;
}
.v-image {
  border-bottom: 1px solid;
}
.font{
  color:#ffe58f
}
</style>
