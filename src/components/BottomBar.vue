<template >
<div class="d-flex d-sm-none">
    <v-bottom-navigation
    v-model="value"
    background-color="grey"
    dark
    app
    shift
  >
    <v-btn>
      <span>Home</span>

      <v-icon>mdi-home</v-icon>
    </v-btn>

    <v-btn>
      <span>Certs</span>

      <v-icon>mdi-school-outline</v-icon>
    </v-btn>

    <v-btn>
      <span>Book</span>

      <v-icon>mdi-book</v-icon>
    </v-btn>

    <v-btn>
      <span>Profile</span>

      <v-icon>mdi-menu</v-icon>
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