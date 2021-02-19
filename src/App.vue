<template>
  <v-app id="main-app-yo">
    <v-app-bar app color="#f0cee1">
          <v-img
            alt="logo"
            class="shrink mt-1 logo-class"
            contain
            src="/assets/cAndJBetter.png"
            style="cursor: pointer;"
            width="90"
          />
      <v-toolbar-title class="white--text"><h4>March 15, 2021</h4></v-toolbar-title>
      <!-- <div class="d-flex align-center">
        <router-link to="/resume">
          <v-img
            alt="logo"
            class="shrink mt-1 logo-class"
            contain
            src="/assets/logo.svg"
            style="cursor: pointer"
            width="50"
          />
        </router-link>
      </div>

      <v-spacer></v-spacer>

      <v-btn @click="dialogOpen = true" text>
        <v-icon>mdi-information-outline</v-icon>
      </v-btn>
      <v-btn
        href="https://www.linkedin.com/in/connor-moynahan-0a568698/"
        target="_blank"
        rel="noopener noreferrer"
        text
      >
        <v-icon>fa-linkedin-square</v-icon>
      </v-btn>
      <v-btn link to="/contact" text>
        <v-icon>fa-id-card-o</v-icon>
      </v-btn> -->
      <!--<router-link class="router-options" to="/">About</router-link> |
      <router-link class="router-options" to="/searchbgg">Search BGG</router-link>-->
    </v-app-bar>

    <!-- <v-dialog v-model="dialogOpen" width="500">
      <v-card>
        <v-card-title class="headline lighten-2 dialog-class" primary-title
          >About this site</v-card-title
        >

        <v-card-text>{{ aboutThisSite }}</v-card-text>

        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn color="primary" text @click="dialogOpen = false">Neat!</v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog> -->

    <v-content>
      <router-view />
      <!-- <HelloWorld/> -->
    </v-content>
    <v-footer class="justify-center" color="#FFF8DC" padless>
      <!-- <v-card
        flat
        tile
        width="100%"
        class="red lighten-1 text-center"
      >
        <v-card-text class="white--text">
          {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
        </v-card-text>
      </v-card> -->
      <h6>🚀🚀🚀🚀🚀: {{ timeRemaining }}</h6>
    </v-footer>
  </v-app>
</template>

<script>
// import HelloWorld from './components/HelloWorld';
// import siteText from './text/site-text';

// const countDownDate = new Date('May 15, 2021 18:00:00').getTime();
// const countdownFunction = () => {
// const now = new Date().getTime();
// const distance = countDownDate - now;
// const days = Math.floor(distance / (1000 * 60 * 60 * 24));
// const hours = Math.floor(
//   (distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60),
// );
// const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
// const seconds = Math.floor((distance % (1000 * 60)) / 1000);
// this.timeRemaining = `${days}d ${hours}h ${minutes}m ${seconds}s `;
//   // If the count down is finished, write some text
// if (distance < 0) {
//   clearInterval(x);
//   document.getElementById("demo").innerHTML = 'EXPIRED';
// }
// };
// const x = setInterval(countdownFunction, 1000);
// setInterval(countdownFunction, 1000);

export default {
  name: 'App',

  components: {
    // HelloWorld,
  },

  data: () => ({
    timeRemaining: '',
    dateOfCeremony: new Date('May 15, 2021 18:00:00').getTime(),
    // showDrawer: false,
    // dialogOpen: false,
    // aboutThisSite: siteText.aboutThisSite,
    //     items: [
    //   { title: 'Home', icon: 'dashboard' },
    //   { title: 'About', icon: 'question_answer' },
    // ],
  }),
  mounted() {
    this.countdownMethod();
  },
  methods: {
    countdownMethod() {
      this.timeRemaining = setInterval(() => {
        const now = new Date().getTime();
        const distance = this.dateOfCeremony - now;
        const days = Math.floor(distance / (1000 * 60 * 60 * 24));
        const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
        const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
        const seconds = Math.floor((distance % (1000 * 60)) / 1000);

        //   // Display the result in the element with id="demo"
        // document.getElementById('countdown').innerHTML =
        this.timeRemaining = `${days}d ${hours}h ${minutes}m ${seconds}s `;
      }, 1000);
    },
  },
};
</script>

<style scoped>
html,
body,
h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: "Roboto", sans-serif;
}

.router-options {
  color: white;
  margin: 10px;
}

.headshot-navbar {
  border-radius: 50%;
  height: 40px;
  width: 40px;
}

.dialog-class {
  background-color: #4682b4;
  color: white;
  margin-bottom: 5px;
}

#main-nav-bar {
  position: fixed;
  top: 0;
  left: 0;
  overflow-y: scroll;
}

#main-app-yo{
    background-image: url('/assets/watercolor.png');
    background-repeat: repeat;
  }
</style>
