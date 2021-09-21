<template>
  <section id="contact" class="contact-section">
    <v-container>
      <v-row>
        <v-col>
          <h1 class="text-center">Contact</h1>
        </v-col>
      </v-row>
      <v-row>
        <v-col sm="6" offset-sm="3" class="d-flex justify-space-around">
          <a href="https://github.com/Sanitc" target="_blank">
            <img
              class="contact-icon"
              src="https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/github.svg"
              
            >
          </a>
          <h3>lesaint.c.dev@gmail.com</h3>
          <a href="https://www.linkedin.com/in/cl%C3%A9ment-le-saint-1a8083154/" target="_blank">
            <img
              class="contact-icon"
              src="https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/linkedin.svg"
            >
          </a>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<style scoped>
.contact-section {
  background-color: #000;
  color: #FFE58F;
}
.contact-icon {
  height: 50px;
  background-color: #FFE58F;
  border-radius: 25px;
}
</style>
