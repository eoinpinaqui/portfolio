<template>
  <v-app id="app">
    <span class="bg" style="z-index: 0"></span>
    <div id="content">
      <v-container>
        <v-card>
          <v-container>
            <div id="banner">
              <v-row
                justify="center"
                align="center"
                >
                  <v-col sm="6">
                    <h2 id="subtitle">Hi there! I'm</h2>
                    <h1 id="title">Eoin Pinaqui</h1>
                  </v-col>
                  <v-col sm="6">
                    <v-img
                      :src="require('./assets/IMG_1834.jpg')"
                      width="80%"
                      style="border-radius: 50%; box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19)"
                      max-width="600px"
                      class="mx-auto mt-lg-10 mb-lg-10"
                    ></v-img>
                  </v-col>
                </v-row>
            </div>
            <div id="intro">
              <h1>About Me</h1>
              <p>Studying computer science has allowed me to marry my interests in technology, problem-solving and innovation. 
                  I am particularly interested in pursuing a software engineering career and have significant internship experience in this field.
              </p>
              <v-btn
                style="box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19)"
                color="#00ff7f"
              >
                See my Resume
              </v-btn>
              <v-img
                :src="require('./assets/trinity.jpg')" 
                elevation="10"
                max-width="1180px"
                style="box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19)"
                class="mb-10 mt-10"
              ></v-img>
            </div>
          </v-container>
        </v-card>
      </v-container>
    </div>
    <v-footer class="mt-3" style="background-color: #00ff7f; padding-bottom: 50px">
      <v-container class="text-center">
        <h1 class="mb-5" style="color: white">Get in touch</h1>
          <v-row class="text-center">
          <div class="mx-auto text-center">
            <v-icon
              size="5em"
              color="white"
              class="mr-10"
            >
              mdi-email
            </v-icon>
            <v-icon
              size="5em"
              color="white"
              class="mr-10 ml-10"
            >
              mdi-linkedin
            </v-icon>
            <v-icon
              size="5em"
              color="white"
              class="ml-10"
            >
              mdi-github
            </v-icon>
          </div>
        </v-row>
      </v-container>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: 'App',
};
</script>

<style>

#app {
  font-family: "Roboto", sans-serif;
  background-color: #00ff7f;
}

.bg {
  width: 100%;
  height: 100vh;
  position: absolute;
  top: 0;
  left: 0;
  background: url('assets/background.svg') no-repeat center center;
  background-size: cover;
}

#content {
  color: black;
  background-color: #00ff7f;
  margin: 20em 0 0 0;
}

#banner {
  max-width: 1000px; 
  margin: 5em auto 15em auto;
}

#intro {
  margin: 100em 0 0 0;
  max-width: 1200px;
  margin: 0 auto;
  text-align: center;
}

#title {
  font-size: 5em !important;
  font-weight: 900 !important;
}

#subtitle {
  font-size: 2.5em !important;
  font-weight: 300 !important;
}

h1 {
  font-size: 3.5em !important;
  font-weight: 900 !important;
}

h2 {
  font-size: 1.5em !important;
  font-weight: 300 !important;
}

p {
  font-size: 1.25em !important;
  font-weight: 300 !important;
}

</style>
