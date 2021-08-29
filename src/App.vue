<template>
  <v-app>
   

   <v-content>

      <router-view/>
    <BottomBar v-if="$route.path!='/'" />
   </v-content>
  </v-app>
</template>

<script>
import BottomBar from './components/BottomBar.vue'
export default {
  name: 'App',
  components:{
    BottomBar
  },
  data: () => ({
    //
  }),
};
</script>
