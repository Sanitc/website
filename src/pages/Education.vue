<template>
  <section id="educations-expériences" class="education-section">
    <v-container>
      <v-row>
        <v-col>
          <h1>Education</h1>
        </v-col>
      </v-row>
      <v-row>
        <v-col>
          <v-timeline>
            <v-timeline-item
              v-for="(year, i) in years"
              :key="i"
              :color="year.color"
              small
            >
              <template v-slot:opposite>
                <span
                  :class="`headline font-weight-bold--text`"
                  v-text="year.year"
                ></span>
              </template>
              <div class="py-4 relief">
                <h2 :class="`headline font-weight-light mb-4 ${year.color}--text`"><span :class="`headline font-weight ${year.title}--text`" v-text="year.title"></span></h2>
                <div>
                  <span :class="`headline font-weight-light ${year.text}--text`" v-text="year.text"></span>
                </div>
              </div>
            </v-timeline-item>
          </v-timeline>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<script>
export default {
  data() {
    return {
      years: [
        {
          color: '#FF7FC6',
          title: 'BTS SIO | Lycée de la Salle',
          year: 'Septembre 2017 - Juin 2019',
          text: 'Obtention du BTS SIO (Services Informatiques aux Organisations) option solutions logicielles et applications métiers',
        },
        {
          color: '#FF7FC6',
          title: "Stage d'étude de BTS1 à Pricer - Guyancourt",
          year: 'Mai - Juin 2018',
          text: "Création de la maquette du site web via un mockup ainsi que la conception Base de données sql, puis conception de l'intranet en HTML, PHP, JS."
        },
        {
          color: '#FF7FC6',
          title: "Stage d'étude de BTS2 à Alkante - Noyal sur Vilaine",
          year: 'Janvier - Février 2019',
          text: "Continuer la conception de l'intranet d'un chercheur de l'université de Rennes 2 avec le framework Phalcon",
        },
        {
          color: '#C6FF7F',
          title: 'Bachelor développement web | My Digital School Rennes',
          year: 'Octobre 2019 - Juillet 2020',
          text: 'Obtention du Bachelor Developpeur Web',
        },
        {
          color: '#C6FF7F',
          title: 'Développeur Junior alternant | ADB INFO Saint Brice en Coglès',
          year: 'Octobre 2019 - Juillet 2020',
          text: "Création de site web en HTML, PHP, JS ainsi que la maintenance d'une application mobile avec le framework Ionic",
        },
      ]
    }
  }
}
</script>

<style>
.education-section{
  background-color: #E7EAFB;
  /*height: 35%;*/
}

.relief{
  border: solid;
  border-radius: 15px ;
  background-color: #CACDDC;
  border-color:#CACDDC;
  box-shadow: 10px 5px 5px #ADAFBC;
  padding: 25px;
  
  
}
</style>