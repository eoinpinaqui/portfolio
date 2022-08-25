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
                    <div class="greeting">
                      <h2 id="subtitle">Hi there! I'm</h2>
                      <h1 id="title">Eoin Pinaqui</h1>
                    </div>
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
                  style="box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);"
                  color="#00ff7f"
                  @click.prevent="openResume"
                >
                  See my Resume
                </v-btn>
              <v-img
                :src="require('./assets/eoin.jpg')" 
                elevation="10"
                width="50%"
                style="box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19); margin: 0 auto;"
                class="mb-10 mt-10"
              ></v-img>
            </div>
          </v-container>
        </v-card>
      </v-container>
    </div>
    <v-footer class="mt-3" style="background-color: #00ff7f; padding-bottom: 50px">
      <v-container class="text-center">
        <h2 class="mb-5" style="color: white; font-weight: 900 !important;">Get in touch</h2>
          <v-row class="text-center">
          <div class="mx-auto text-center">
            <a href="mailto: pinaquie@tcd.ie" target="_blank">
              <v-icon
                x-large
                color="white"
                class="mr-10"
              >
                mdi-email
              </v-icon>
            </a>
            <a href="https://www.linkedin.com/in/eoin-pinaqui/" target="_blank">
              <v-icon
                x-large
                color="white"
                class="mr-10 ml-10"
              >
                mdi-linkedin
              </v-icon>
            </a>
            <a href="https://github.com/eoinpinaqui" target="_blank">
              <v-icon
                x-large
                color="white"
                class="ml-10"
              >
                mdi-github
              </v-icon>
            </a>
          </div>
        </v-row>
      </v-container>
    </v-footer>
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
}

#banner {
  max-width: 1000px; 
  margin: 5em auto 5em auto;
}

#intro {
  margin: 100em 0 0 0;
  max-width: 1200px;
  margin: 0 auto;
  text-align: center;
}

@media (max-width: 700px) {
  .greeting {
    text-align: center;
  }
}

#title {
  font-size: 4em !important;
  font-weight: 900 !important;
}

#subtitle {
  font-size: 2.5em !important;
  font-weight: 300 !important;
}

h1 {
  font-size: 2em !important;
  font-weight: 900 !important;
}

h2 {
  font-size: 1.25em !important;
  font-weight: 300 !important;
}

p {
  font-size: 1.25em !important;
  font-weight: 300 !important;
}

a {
  text-decoration: none;
}

</style>
