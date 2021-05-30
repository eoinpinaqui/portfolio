<template>
  <v-app id="app">
    <div id="banner" style="height: 100vh">
      <span class="bg"></span>
      <v-container
          fill-height
          fluid
      >
        <v-row
            justify="center"
            align="center"
        >
          <v-container>
            <v-card class="mx-auto" max-width="1000px">
              <v-container>
                <v-row
                    justify="center"
                    align="center"
                >
                  <v-col sm="6">
                    <div class="ml-10">
                      <h2>Hi there! I'm</h2>
                      <h1>Eoin Pinaqui.</h1>
                    </div>
                  </v-col>
                  <v-col sm="6">
                    <v-img
                        :src="require('./assets/IMG_1834.jpg')"
                        width="80%"
                        style="border-radius: 50%"
                        max-width="600px"
                        class="mx-auto mt-lg-10 mb-lg-10"
                    >
                    </v-img>
                  </v-col>
                </v-row>
              </v-container>
            </v-card>
          </v-container>
        </v-row>
      </v-container>
    </div>
    <div id="content" style="background-color: #00ff7f">
      <v-container
          fill-height
          fluid
      >
        <v-row
            justify="center"
            align="center"

        >
          <v-container>
            <div class="text-center" data-aos="fade-up">
              <h1>Who am I?</h1>
              <p style="font-size: 1.25em">I am a final year Computer Science student at Trinity College Dublin with a
                passion for software
                engineering.</p>
              <v-btn class="mt-5 mb-10"
                     style="box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19)">See my Resume
              </v-btn>
              <v-img elevation="10" :src="require('./assets/trinity.jpg')" max-width="1180px" class="mx-auto mb-10"
                     style="box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19)"></v-img>
            </div>
          </v-container>
        </v-row>
      </v-container>
      <v-container
          fill-height
          fluid
      >
        <v-row
            justify="center"
            align="center"
        >
          <v-container>
            <v-card class="mx-auto" style="margin-top: 100px">
              <v-container>
                <v-row
                    justify="center"
                    align="center"
                >
                  <div style="width: 100%; text-align: center">
                    <h1 class="mt-10">Work Experience</h1>
                  </div>
                  <v-timeline style="margin: 1em 3em 3em 3em">
                    <v-timeline-item
                        v-for="(year, i) in years"
                        :key="i"
                        :color="year.color"
                        small
                    >
                      <template v-slot:opposite>
                        <span
                            :class="`headline font-weight-bold`"
                            v-text="year.year"
                        ></span>
                      </template>
                      <div class="py-4">
                        <h2 :class="`headline font-weight-light mb-4`">
                          {{ year.title }}
                        </h2>
                        <div>
                          {{ year.description }}
                        </div>
                      </div>
                    </v-timeline-item>
                  </v-timeline>
                </v-row>
              </v-container>
            </v-card>
          </v-container>
        </v-row>
      </v-container>
    </div>
  </v-app>
</template>

<script>
import AOS from 'aos';
import 'aos/dist/aos.css';

export default {


  name: 'App',

  components: {},

  data: () => ({
    years: [
      {
        color: '#00ffff',
        title: 'Software Engineering Intern at Stripe',
        year: 'Summer 2021',
        description: 'Who knows what the future may hold?!',
      },
      {
        color: '#00ffff',
        title: 'Laboratory Demonstrator at Trinity College Dublin',
        year: '2020/21 Academic Year',
        description: 'Assisted with the running of online lab sessions, the marking of assignments and the ' +
            'teaching of ARM assembly language to first-year students.',
      },
      {
        color: '#00ffff',
        title: 'Programming Tutor at The Academy of Code',
        year: 'Winter 2020',
        description: 'Taught object-oriented programming to primary and secondary school students using the ' +
            'Processing programming language over Zoom.',
      },
      {
        color: '#00ffff',
        title: 'Software Development Engineering Intern at Amazon Web Services (AWS)',
        year: 'Summer 2020',
        description: 'Made the debugging process simpler for AWS Lambda customers and operators by creating ' +
            'a Golang Lambda extension that watches for core dumps and uploads them into an S3 bucket for ' +
            'later inspection and troubleshooting.',
      },
      {
        color: '#00ffff',
        title: 'IT Intern at Wexford County Council',
        year: 'Summer 2019',
        description: 'Protected over 700 work computers from security threats by managing the automated patch management process, using SolarWinds Patch Manager.',
      },
    ],
  }),

  created() {
    AOS.init();
  }
};
</script>

<style>

#app {
  font-family: "Roboto", sans-serif;
}

h1 {
  font-size: 3.5em !important;
  font-weight: 900 !important;
}

h2 {
  font-size: 1.5em !important;
  font-weight: 300 !important;
}

#banner {
  color: black;
}

#content {
  color: white;
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
</style>
