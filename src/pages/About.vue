<template>
  <section id="a-propos" class="about-section">
    
    <v-container>
      <div class="center">
          <h1>Portefolio - Clément Le Saint</h1>
      </div>
      <div class="center-about">
      <v-row>
        <v-col sm="4">
          <g-image class="img" alt="Example image" src="~/assets/img/photo/clement.png" width="380"/>
        </v-col>
        <v-col sm="8" class="d-flex flex-column justify-center ">
          <div class="relief">
            <h1>Clément Le Saint</h1>
            <div>
              <p>Diplômée d’un Bachelor Développement Web » (Titre RNCP – Bac+3) de l’école MYDIGITALSCHOOL de Rennes,</p>
              <p>je souhaite poursuivre mon cursus à la rentrée 2021, avec l'établissement MyDigitalSchool Angers,</p>
              <p>qui propose une formation de Développeur web Full Stack (Bac+5 – Titre RNCP), en alternance.</p>
            </div>
            <h3>Hobbies</h3>
              <p>- Pratique l'athlétisme depuis 6 ans</p>
              <p>- Escalade</p>
              <p>- Cinéma</p>
              <p>- Photographie</p>
          </div>   
        </v-col>
      </v-row>
      </div>
    </v-container>
  </section>
</template>

<style scoped>
.about-section{
  background-color: #E7EAFB;
  padding-bottom: 12%;
}
.img{
  border-radius: 15px;
  box-shadow: 10px 5px 5px #ADAFBC
}

.relief{
  border: solid;
  border-radius: 15px ;
  background-color: #CACDDC;
  border-color:#CACDDC;
  margin-right:10% ;
  margin-left:10% ;
  box-shadow: 10px 5px 5px #ADAFBC;
  
}

.center-about{
  padding-top: 5%;
  padding-left: 10%
}
.center{
  padding-top: 5%;
  text-align: center;
  font-size: 150%;
}
</style>
