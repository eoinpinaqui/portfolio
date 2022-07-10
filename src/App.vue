<template>
  <v-app id="app">
    <div id="banner" class="bg">
      <v-container
          fill-height
          fluid
      >
        <v-row
            justify="center"
            align="center"
            style="z-index: 1"
        >       
          <h1>Eoin Pinaqui</h1>
        </v-row>
      </v-container>
    </div>
    <div id="content">
      <div class="bg-2">
        <v-container>
          <div style="text-align: center; margin: 5em;">
            <h2>Who am I?</h2>
            <v-row
              justify="center"
              align="center"
              style="margin: 0 0 5em 0;"
            >
              <v-col sm="6">
                <div>
                  <h3>A Master's of Computer Science student passionate about software engineering.</h3>
                  <v-btn
                    dark
                    x-large
                    color="#310049"
                    elevation="10" 
                    style="font-family: 'Heebo', sans-serif; font-weight: 900; margin: 5em 0 2em 0;"
                  >
                  See my Resume
                  </v-btn>
                </div>
              </v-col>
              <v-col sm="6">
                <v-img
                  :src="require('./assets/me.jpg')"
                  width="50%"
                  style="border-radius: 50%"
                  max-width="400px"
                  class="mx-auto mt-lg-10 mb-lg-10"
                ></v-img>
              </v-col>
            </v-row>
          </div>  
        </v-container>
      </div>
      <div class="bg-3">
        <v-container id="intro" style="width: 100vw;">
        <div style="text-align: center; margin: 5em auto;">
          <h2>My Experience</h2>
          <v-container>
            <v-row>
              <v-col sm="6">
                <div style="text-align: left">
                <h3>Software Engineering Intern - Stripe</h3>
                <h4>Jan 2022 - Jun 2022</h4>
                <ul>
                  <li>Designed and built a new automatic onboarding process for the Klarna payment method.</li>
                  <li>Facilitated the rollout of Klarna disputes to over 50,000 connected accounts.</li>
                  <li>Created automatic alerts and mitigation tools for Klarna manual reconciliation issues.</li>
                  <li>Main programming languages used: Ruby, Java.</li>
                </ul>
              </div>
              </v-col>
              <v-col sm="6">
                <v-img
                  :src="require('./assets/stripe.png')"
                  width="80%"
                  max-width="400px"
                  class="mx-auto mt-lg-10 mb-lg-10"
                ></v-img>
              </v-col>
            </v-row>
            <v-row>
              <v-col sm="6">
                <div style="text-align: left">
                <h3>Software Developer - Trinity College Dublin Students Union</h3>
                <h4>Jun 2021 - Jan 2022</h4>
                <ul>
                  <li>Built a personnel and events management system with a team of three engineers.</li>
                  <li>Led the design and development of all backend services and the API.</li>
                  <li>Main programming languages used: Golang, VueJS.</li>
                </ul>
              </div>
              </v-col>
              <v-col sm="6">
                <v-img
                  :src="require('./assets/tcdsu.svg')"
                  width="20%"
                  min-width="100px"
                  class="mx-auto mt-lg-10 mb-lg-10"
                ></v-img>
              </v-col>
            </v-row>
          </v-container>
        </div>   
      </v-container>
      </div>
    </div>
  </v-app>
</template>

<script>
import 'aos/dist/aos.css';

export default {
  name: 'App',
  components: {},
};
</script>

<style>

h1 {
  font-family: 'Old Standard TT', serif;
  font-size: calc(100px + 5vw) !important;
}

h2 {
  font-family: 'Old Standard TT', serif;
  font-size: calc(60px + 2vw) !important;
}

h3 {
  font-family: 'Heebo', sans-serif;
  font-size: calc(25px + 0.5vw) !important;
  font-weight: 300;
}

h4 {
  font-family: 'Heebo', sans-serif;
  font-size: calc(20px + 0.25vw) !important;
  font-weight: 300;
}

p, li {
  font-family: 'Heebo', sans-serif;
  font-size: calc(15px + 0.25vw) !important;
}

#banner {
  color: white;
}

#content {
  color: white;
}

.bg {
  width: 100%;
  height: 100vh;
  top: 0;
  left: 0;
  background: url('assets/background.svg') no-repeat center center;
  background-color: #5b0287;
  background-size: cover;
}
.bg-2 {
  width: 100vw;
  height: 100vh;
  top: 0;
  left: 0;
  background: url('assets/background-2.svg') no-repeat center center;
  background-color: #2a42ee;
  background-size: cover;
}

.bg-3 {
    background-color: #2a42ee;
}

</style>
