<template>
  <section id="compétences" class="skill-section">
    <v-container>
      <v-row>
        <v-col>
          <h1 class="space">Compétences informatiques</h1>
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
          <h1 class="space space2">Compétences linguistiques</h1>
        </v-col>
      </v-row>
      <v-row>
        <v-col sm="6" offset-sm="3" class="d-flex justify-space-around">
           
              <g-image alt="Example image" src="~/assets/img/langue/france.png" class="img-lang2 col-sm"/>   <br/>
              <v-rating class="col-sm"
                color="black"
                background-color="black"
                empty-icon: icons.iconempty
                full-icon: icons.iconfull
                half-icon: icons.iconhalf
                half-increments
                length="5"
                readonly
                size="40"
                value="4.5"
              ></v-rating> 
            
              <g-image alt="Example image" src="~/assets/img/langue/uk.png" class="img-lang2 col-sm"/>   <br/>
              <v-rating class="col-sm"
                color="black"
                background-color="black"
                empty-icon: icons.iconempty
                full-icon: icons.iconfull
                half-icon: icons.iconhalf
                half-increments
                length="5"
                readonly
                size="40"
                value="3"
              ></v-rating> 
                      
            
              <g-image alt="Example image" src="~/assets/img/langue/spain.png" class="img-lang2 col-sm"/>   <br/>
              <v-rating class="col-sm"
                color="black"
                background-color="black"
                empty-icon: icons.iconempty
                full-icon: icons.iconfull
                half-icon: icons.iconhalf
                half-increments
                length="5"
                readonly
                size="40"
                value="3"
              ></v-rating> 
            
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<style scoped>
.skill-section {
  background-color: #E7EAFB ;
  padding-bottom: 2%;
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
   
}

.space{
  padding-bottom: 5%;
}
.space2{
  padding-top: 2%;
}

.img-lang2 {
    height: 75%;
    width: 25%;
    object-fit: contain ;
    
}

.img-lang:hover{
 transform: scale(1.2); 
}

</style>

<script>
export default {
  data() {
    return {
      icons: [
        { iconfull: 'mdi-moon-full',iconhalf: 'mdi-moon-last-quarter', iconempty: "mdi-moon-new"},
      ]
    }
  }
}
</script>