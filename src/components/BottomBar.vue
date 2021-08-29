<template >
<div class="d-flex d-sm-none">
    <v-bottom-navigation
    v-model="value"
    background-color="grey"
    dark
    app
    
    
    shift
    
  >

    <v-btn style="height:100%" plain to="/overview">
      <span>Overview</span>

      <v-icon>mdi-motion-play</v-icon>
    </v-btn>

    <v-btn plain style="height:100%" to="/courses">
      <span>Courses</span>

      <v-icon>mdi-school-outline</v-icon>
    </v-btn>

    <v-btn plain style="height:100%" to="/ti">
      <span>Messages</span>

      <v-icon>mdi-tooltip-text-outline</v-icon>
    </v-btn>

    <v-btn plain style="height:100%" to="/na">
      <span>Profile</span>

      <v-icon>mdi-account</v-icon>
    </v-btn>
    <v-btn style="height:100%"  to="tooo" plain>
      <span>Home</span>

      <v-icon >mdi-arrow-right-bold-box-outline</v-icon>
    </v-btn>
  </v-bottom-navigation>
</div>
</template>

<script>
  export default {
    data: () => ({ value: 'black' }),

    computed: {
      color () {
        switch (this.value) {
          case 0: return 'blue-grey'
          case 1: return 'teal'
          case 2: return 'brown'
          case 3: return 'indigo'
          default: return 'blue-grey'
        }
      },
    },
  }
</script>

<style>

</style>