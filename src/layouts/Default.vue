<template>
  <v-app>
    <v-navigation-drawer width="240px" permanent fixed>
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title class="title">
           Clément Le Saint
          </v-list-item-title>
          <v-list-item-subtitle>
            Développeur Junior
          </v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>

      <v-divider></v-divider>

      <v-list
        dense
        nav
      >
        <v-list-item
          v-for="item in items"
          :key="item.title"
          link
          :to="`#${item.title.toLowerCase().replace(' & ', '-')}`"
        >
          <v-list-item-icon>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-main>
      <slot/>
    </v-main>

    <section id="contact" class="contact-section footer">
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

  </v-app>
</template>

<script>
export default {
  data() {
    return {
      items: [
        { title: 'A-propos', icon: 'mdi-account-box-outline' },
        { title: 'Projets', icon: 'mdi-apps' },
        { title: 'Compétences', icon: 'mdi-laptop' },
        { title: 'Educations & Expériences', icon: 'mdi-school-outline' },
        { title: 'Contact', icon: 'mdi-message-text-outline' },
      ]
    }
  }
}
</script>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style>
html {
  scroll-behavior: smooth;
}
/*
.v-application--wrap {

  flex-direction: row;
}
*/
.contact-section {
  background-color: #FBF8E7;
  color: black;
}
.contact-icon {
  height: 50px;
}
.v-main {
  flex: 1 0;
  margin-left: 240px;
}

</style>