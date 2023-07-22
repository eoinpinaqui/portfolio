<template>
  <v-app id="app">
    <v-container>
        <v-card id="content">
          <v-row>
            <v-col>
              <div class="greeting">
                <h2>Hi there! I'm</h2>
                <h1>Eoin Pinaqui</h1>
              </div>
            </v-col>
          </v-row>
          <v-row>
            <v-col>
              <div class="button">
                <p>I am a passionate software engineer with a relentless drive for technology, problem-solving, and innovation.</p>
                <v-btn
                    style="box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);"
                    color="#008BFF"
                    @click.prevent="openResume"
                >
                  See my Resume
                </v-btn>
              </div>
            </v-col>
          </v-row>
          <v-row>
            <v-col>
              <div class="image_div_circle">
                <v-img
                    :src="require('./assets/selfie.jpg')"
                    class="image_circle"
                ></v-img>
              </div>
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
  background-color: #008BFF;
}

#content {
  margin: 5em 0;
}

.greeting {
  text-align: center;
  margin: 5em 0 0 0;
}

h1 {
  font-size: 3.5em !important;
  font-weight: 900 !important;
}

h2 {
  font-size: 2em !important;
  font-weight: 300 !important;
}

.image_div_circle {
  width: 100%;
  max-width: 400px;
  text-align: center;
  margin: 0em auto 5em auto;
}

.image_circle {
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  border-radius: 50%;
}

p {
  font-size: 1.25em !important;
  font-weight: 300 !important;
}

.button {
  text-align: center;
  margin: 2em 0 ;
}

</style>
