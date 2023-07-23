<template>
  <v-app id="app">
    <v-container>
        <v-card id="content">
          <v-row>
            <v-col>
              <h2>Hi there! I'm</h2>
              <h1>Eoin Pinaqui</h1>
            </v-col>
          </v-row>
          <div class="space"></div>
          <v-row>
            <v-col>
              <p>I am a passionate software engineer with a relentless drive for technology, problem-solving, and innovation.</p>
              <v-btn
                  class="shadow"
                  color="#87CEFA"
                  @click.prevent="openResume"
              >
                See my Resume
              </v-btn>
            </v-col>
          </v-row>
          <div class="space"></div>
          <v-row>
            <v-col>
              <v-img
                  :src="require('./assets/selfie.jpg')"
                  class="image shadow"
              ></v-img>
            </v-col>
          </v-row>
        </v-card>
    </v-container>
  </v-app>
</template>

<script>
export default {
  name: 'App',
  methods: {
    openResume() {
      window.open("/Eoin Pinaqui - Resume.pdf", "_blank").focus();
    }
  }
};
</script>

<style>

#app {
  font-family: "Roboto", sans-serif;
  background-color: #87CEFA;
}

#content {
  margin: 10vh 5vw;
  padding: 10vh 5vw;
  text-align: center;
}

.space {
  margin: 3em;
}

.shadow {
  box-shadow: 10px 10px 20px #aaaaaa;
}

.image {
  border-radius: 50%;
  width: 50%;
  min-width: 250px;
  margin: 0 auto;
}

h1 {
  font-size: calc(3.5em + 0.5vw);
  font-weight: 900;
}

h2 {
  font-size: calc(2em + 0.5vw);
  font-weight: 300;
}

p {
  font-size: calc(1em + 0.5vw);
  font-weight: 300;
}
</style>
