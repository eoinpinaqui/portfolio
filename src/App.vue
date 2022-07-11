<template>
  <v-app id="app">
    <div id="banner" class="bg">
      <v-container
          fill-height
      >
        <v-row
            justify="center"
            align="center"
        >       
          <h1>Eoin Pinaqui</h1>
        </v-row>
      </v-container>
    </div>
    <div id="content">
      <div class="bg-2">
        <v-container>
          <div style="text-align: center; margin: 15vh auto;">
            <h2>Who am I?</h2>
            <div>
                <h3>A Master's of Computer Science student passionate about software engineering.</h3>
                <v-btn
                  dark
                  x-large
                  color="#310049"
                  elevation="10" 
                  style="font-family: 'Heebo', sans-serif; font-weight: 900; margin: 3em 0;"
                >
                See my Resume
                </v-btn>
              </div>
          </div>  
        </v-container>
      </div>
      <div class="bg-3">
        <v-container>
        <div style="text-align: center; margin: 5em auto;">
          <v-container>
            <div>
              <h2>Education</h2>
              <div style="text-align: left;">
                <p>Due to academic success in my undergraduate degree, I was accepted into the integrated Master in Computer Science (MCS) programme at Trinity College Dublin.</p>
                <ul>
                  <li>Currently awaiting final results for my undergraduate degree.</li>
                  <li>3rd Year Grade: 1.1 (4.0 GPA Equivalent) - 86% overall and 1st out of 91 students</li>
                  <li>2nd Year Grade: 1.1 (4.0 GPA Equivalent) - 90% overall and 1st out of 96 students</li>
                  <li>1st Year Grade: 1.1 (3.98 GPA Equivalent) - 86% overall and 6th out of 100 students</li>
                </ul>
              </div>
              <v-img
                  :src="require('./assets/trinity.jpg')"
                  width="80%"
                  max-width="800px"
                  class="mx-auto mt-10 mb-10"
              ></v-img>
            </div>
            <div>
              <h2 style="margin: 1em 0 0 0">Experience</h2>
              <div style="text-align: left;">
                <div class="work">
                  <h3>Software Engineering Intern - Stripe</h3>
                  <h4>Jan 2022 - Jun 2022</h4>
                  <ul>
                    <li>Designed and built a new automatic onboarding process for the Klarna payment method.</li>
                    <li>Facilitated the rollout of Klarna disputes to over 50,000 connected accounts.</li>
                    <li>Created automatic alerts and mitigation tools for Klarna manual reconciliation issues.</li>
                    <li>Main programming languages: Ruby, Java.</li>
                  </ul>
                </div>
                <div class="work">
                  <h3>Part-time Software Developer - Trinity College Dublin Students Union</h3>
                  <h4>Jun 2021 - Jan 2022</h4>
                  <ul>
                    <li>Built a personnel and events management system with a team of three engineers.</li>
                    <li>Led the design and development of all backend services and the API.</li>
                    <li>Main programming languages: Golang, VueJS.</li>
                  </ul>
                </div>
                <div class="work">
                  <h3>Software Engineering Intern - Stripe</h3>
                  <h4>Jun 2021 - Sep 2022</h4>
                  <ul>
                    <li>Implemented an autoscaling solution for Stripe's cloud continuous integration (CI) infrastructure.</li>
                    <li>Beta tested a new internal framework by creating sample projects and providing feedback.</li>
                    <li>Main programming languages: Ruby.</li>
                  </ul>
                </div>
                <div class="work">
                  <h3>Programming Tutor - Trinity College Dublin & The Academy of Code</h3>
                  <h4>Sep 2020 - May 2021</h4>
                  <ul>
                    <li>Assisted in teaching ARM Assembly Language programming to first-year computer science students as part of the Introduction to Computing module.</li>
                    <li>Delivered lessons on object-oriented programming and web development to children aged 7 to 16 over Zoom.</li>
                    <li>Main programming languages: Processing, Java, HTML, CSS, Javascript, ARM Assembly Language.</li>
                  </ul>
                </div>
                <div class="work">
                  <h3>Software Development Engineering Intern - Amazon Web Services (AWS)</h3>
                  <h4>May 2020 - Sep 2020</h4>
                  <ul>
                    <li>Developed sample Lambda extensions in <a style="color: white;" href="https://github.com/aws-samples/aws-lambda-extensions">multiple programming languages</a>.</li>
                    <li>Main programming languages: Golang, Python, Java.</li>
                  </ul>
                </div>
                <div class="work">
                  <h3>Information Technology Summer Intern - Wexford County Council</h3>
                  <h4>Jun 2019 - Aug 2019</h4>
                  <ul>
                    <li>Managed the automatic patch process for over 700 work computers using SolarWinds Patch Manager.</li>
                    <li>Assisted in the development of an in-house mobile application for monitoring ring buoys.</li>
                    <li>Main programming languages: HTML, CSS, Javascript.</li>
                  </ul>
                </div>
                <div class="work">
                  <v-row>
                    <v-col>
                      <v-img
                        :src="require('./assets/stripe.png')"
                        width="80%"
                        max-width="800px"
                        class="mx-auto"
                      ></v-img>
                    </v-col>
                    <v-col>
                      <v-img
                        :src="require('./assets/aws.jpg')"
                        width="80%"
                        max-width="800px"
                        class="mx-auto"
                      ></v-img>
                    </v-col>
                  </v-row>
                </div>
              </div>
            </div>
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

* {
  color: white;
}

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

.bg {
  width: 100vw;
  height: 100vh;
  background: url('assets/background.svg') no-repeat center center;
  background-color: #5b0287;
  background-size: cover;
}
.bg-2 {
  width: 100vw;
  height: 100vh;
  background: url('assets/background-2.svg') no-repeat center center;
  background-color: #2a42ee;
  background-size: cover;
}

.bg-3 {
  width: 100vw;
  background-color: #2a42ee;
}

.work {
  margin: 0 0 3em 0;
}

</style>
