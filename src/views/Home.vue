<template>
  <div>
    <v-row no-gutters align="center" justify="center">
      <v-col cols="12" xs="12" md="12" sm="12" lg="2 " xl="2" >
        
          <Sidebar />
      </v-col>
      <v-col cols="12" xs="12" md="12" sm="12" xl="10" lg="10">
          <v-row align="start" justify="start" style="height:100%">
            <v-col cols="12" xs="12" sm="12" md="12" xl="7" lg="7">
              <Intro />
            <div style="height:40vh">

            </div>
            </v-col>
            <v-col cols="12" xs="12" sm="12" md="12" xl="5" lg="5">
              
            </v-col>
          </v-row>
      </v-col>
    </v-row>
  </div>
</template>

<script>
import Sidebar from '../components/SideBar.vue'
import Intro from '../components/Home/Intro.vue'
  export default {
    name: 'Home',

    components: {
      Sidebar,
      Intro
    },
    data(){
      return {
        items: [
          { title: 'Dashboard', icon: 'mdi-view-dashboard' },
          { title: 'Photos', icon: 'mdi-image' },
          { title: 'About', icon: 'mdi-help-box' },
        ],
      }
    }
  }
</script>
<style>
.shadow{
   box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}
</style>
