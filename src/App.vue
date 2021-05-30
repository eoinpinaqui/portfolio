<template>
  <v-app id="app" style="height:500px">
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
          <v-card>
            <h1>Hi there</h1>
          </v-card>
        </v-container>
      </v-row>
    </v-container>
  </v-app>
</template>

<script>
export default {
  name: 'App',

  components: {},

  data: () => ({
    //
  }),
};
</script>

<style>

.bg {
  width: 110%;
  height: 100%;
  position: absolute;
  top: 0;
  left: 0;
  background: url('assets/background.svg') no-repeat;
  background-size: cover;
}
</style>

