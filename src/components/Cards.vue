<template>
<v-row class="justify-space-around mb-8 mt-4">
        <v-card
          v-for="project in projects"
          :key="project.name"
          class="cards"
          max-width="300"
          
        >
          <v-img
            class="align-end"
            height="250px"
            :src="project.image"
          />
          <v-card-title>{{ project.name }}</v-card-title>

          <v-card-text>
            {{ project.description }}
          </v-card-text>

          <v-card-actions>
            <v-btn
              color="#F6AB58"
              text
             :href="project.github" target="_blank"
            
            >
              Dépot Github
            </v-btn>

          </v-card-actions>
        </v-card>
</v-row>
</template>

<script>

export default {
   props: ['name','description','image','github'],
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
          name: 'Autres projets',
          github: 'https://github.com/Sanitc?tab=repositories',
          description: "Dépot où l'on retrouve mes tps effectué lors de mon bac+3",
          image: 'https://raw.githubusercontent.com/Sanitc/website/main/src/assets/img/projet/portefolio-projet.png'
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

<style>

.v-image {
  border-bottom: 1px solid;
  border-start-start-radius: 10px;
}

.cards{
  border-radius: 15px;
  box-shadow: 10px 5px 5px #ADAFBC;
}

</style>