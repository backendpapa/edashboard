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
              <div class="mt-5 ">
                <p class="text-h5 font-weight-bold">Courses</p>
                <v-tabs class="mt-n4"  hide-slider  v-model="tab" color="black" background-color="transparent" >
                  <v-tab style="text-transform:none" v-for="item in item" :key="item.tab">
                    {{ item.tab }}
                  </v-tab>
                </v-tabs>
                <v-tabs-items style="height:40vh;overflow-y:scroll" class="mt-n4 my-scroll" v-model="tab">
                  <v-tab-item v-for="item in item" :key="item.tab">
                    <v-card flat>
                      <v-card-text>
                        <component v-bind:is="item.content"></component>
                      </v-card-text>
                    </v-card>
                  </v-tab-item>
                </v-tabs-items>
              </div>
            <div style="">
              <v-row>

              </v-row>
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
import AllCourses from '../components/Courses/AllCourses.vue'
  export default {
    name: 'Home',

    components: {
      Sidebar,
      Intro,
      AllCourses
    },
    data(){
      return {
        items: [
          { title: 'Dashboard', icon: 'mdi-view-dashboard' },
          { title: 'Photos', icon: 'mdi-image' },
          { title: 'About', icon: 'mdi-help-box' },
        ],
        tab: null,
      item: [
        { tab: 'All Courses', content: 'AllCourses' },
        { tab: 'The Newest', content: 'ComponentB' },
        { tab: 'Top Rated', content: 'ComponentB' },
        { tab: 'Most Popular', content: 'ComponentB' }
      ]
      }
    }
  }
</script>
<style>
.shadow{
   box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}

  .my-scroll::-webkit-scrollbar {
    width: 3px;
    }


</style>
