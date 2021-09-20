<template>
  <section id="a-propos" class="about-section">
    <v-container>
      <v-row>
        <v-col sm="4">
          <g-image class="img" alt="Example image" src="~/assets/img/photo/clement.png" width="380"/>
        </v-col>
        <v-col sm="8" class="d-flex flex-column justify-center align">
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
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<style scoped>
.about-section{
  background-color: rgb(0, 0, 0);
  color: #FFE58F;
}
.align {
  margin-right: 0px;
}

</style>
