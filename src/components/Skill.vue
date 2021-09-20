<template>
  <section id="compétences" class="skill-section">
    <v-container>
      <v-row>
        <v-col>
          <h1 class="text">Compétences informatique</h1>
        </v-col>
      </v-row>
      <v-row>
        <v-col sm="6" offset-sm="3" class="d-flex justify-space-around">
            <g-image alt="Example image" src="~/assets/img/informatique/html.png" class="img-lang"/>        
            <g-image alt="Example image" src="~/assets/img/informatique/php.png" class="img-lang"/>  
            <g-image alt="Example image" src="~/assets/img/informatique/sql.png" class="img-lang"/>  
            <g-image alt="Example image" src="~/assets/img/informatique/flutter.png" class="img-lang"/>  
        </v-col>
      </v-row>
       <v-col sm="6" offset-sm="3" class="d-flex justify-space-around">
            <g-image alt="Example image" src="~/assets/img/informatique/java.png" class="img-lang"/>  
            <g-image alt="Example image" src="~/assets/img/informatique/js.png" class="img-lang"/>  
            <g-image alt="Example image" src="~/assets/img/informatique/angular.png" class="img-lang"/>  
            <g-image alt="Example image" src="~/assets/img/informatique/vue.png" class="img-lang"/>  
        </v-col>
    </v-container>
        <v-container>
      <v-row>
        <v-col>
          <h1 class="text">Compétence linguistiques</h1>
        </v-col>
      </v-row>
      <v-row>
        <v-col sm="6" offset-sm="3" class="d-flex justify-space-around">
            <g-image alt="Example image" src="~/assets/img/langue/france.png" class="img-lang"/>        
            <g-image alt="Example image" src="~/assets/img/langue/uk.png" class="img-lang"/>  
            <g-image alt="Example image" src="~/assets/img/langue/spain.png" class="img-lang"/>   
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<style scoped>
.skill-section {
  background-color: #FFE58F ;
}
.contact-icon {
  height: 30px;
}
 
.text {
 text-align: left;
 margin-bottom: 20px;
 color: black;
} 

.img-lang {
    height: 75%;
    width: 25%;
    object-fit: contain ;
    margin-left: 50px;
    margin-right: 50px;
    margin-bottom: 20px;
}
</style>
