<template>
  <div class="grey lighten-5">
    <v-row no-gutters align="center" justify="center">
      <v-col cols="12" xs="12" md="12" sm="12" lg="2 " xl="2" >
        
          <Sidebar />
      </v-col>
      <v-col cols="12" xs="12" md="12" sm="12" xl="10" lg="10">
          <v-row no-gutters  justify="start" style="height:100%">
            <v-col cols="12" xs="12" sm="12" md="12" xl="7" lg="7">
              <Intro />
              <div class="mt-5 pa-2">
                <p class="text-h5 font-weight-bold">Courses</p>
                <v-tabs   class="mt-n4" centered  hide-slider  v-model="tab" color="black" background-color="transparent" >
                  <v-tab  style="text-transform:none" v-for="item in item" :key="item.tab">
                    {{ item.tab }}
                  </v-tab>
                </v-tabs>
                <v-tabs-items style="overflow-y:scroll" class="mt-n4 my-scroll mi-height" v-model="tab">
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
                <!--  -->
                <div class="pa-3">
                  <v-row class="d-none d-sm-flex" no-gutters >
                    <v-col cols="12" sm="12" md="12" xl="8" lg="8">
                        <v-text-field dense outlined prepend-inner-icon="mdi-magnify"></v-text-field>
                    </v-col>
                    <v-col cols="12" sm="12" md="12" xl="2" lg="2">
                        <p class="text-center"><v-btn icon><Icon  width="30" icon="mdi:bell-badge-outline" /></v-btn></p>
                    </v-col>
                    <v-col cols="12" sm="12" md="12" xl="2" lg="2">
                       <v-avatar
                          tile
                          size="40"
                          
                        >
                          <v-img style="border-radius:10px" src="https://images.unsplash.com/photo-1599041125553-a3b967646ca5?ixid=MnwxMjA3fDB8MHxzZWFyY2h8Mnx8dnVlanxlbnwwfHwwfHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60"></v-img>
                        </v-avatar>
                    </v-col>
                </v-row>
                <!-- add a v-divider -->
                <v-divider class=ma-4></v-divider>
                <v-row no-gutters   class=" pa-2">
                  <v-col cols="6" style="" class="" >
                    <div class="grey lighten-4 mr-2" style="width:100%;border-radius:15px;height:10vh">
                      <v-row class="pa-2" no-gutters align="center" justify="center">
                        <v-spacer></v-spacer>
                        <p class="text-h3 font-weight-bold"> 11</p>
                         <v-spacer></v-spacer>
                        <div>
                          <p class="font-weight-bold text-caption">Courses</p>
                          <p class="mt-n4 font-weight-bold text-caption">completed</p>
                        </div>
                        <v-spacer></v-spacer>
                       
                      </v-row>
                    </div>
                  </v-col>
                  <v-col cols="6" style="height:100%" class="" >
                    <div class="black white--text ml-2" style="width:100%;border-radius:15px;height:10vh">
                      <v-row style="height:10vh" class="pa-2" no-gutters align="center" justify="center">
                        <v-spacer></v-spacer>
                        <p class="text-h3 font-weight-bold"> 4</p>
                         <v-spacer></v-spacer>
                        <div>
                          <p class="font-weight-bold text-caption">Courses</p>
                          <p class="mt-n4 font-weight-bold text-caption">in progress</p>
                        </div>
                        <v-spacer></v-spacer>
                       
                      </v-row>
                    </div>
                  </v-col>
                </v-row>
                <!-- graph -->
                <div>
                 <v-sheet
      class=" mx-auto mt-2"
      color="grey"
      elevation="12"
      max-width="calc(100% - 32px)"
    >
      <v-sparkline
        :labels="labels"
        :value="value"
        color="white"
        line-width="2"
        padding="16"
          height="140"
      ></v-sparkline>
    </v-sheet>
        <div class="mt-5 ma-2 grey lighten-4" style="height:20vh;border-radius:15px" >
          <v-row no-gutters class="ma-2" style="height:20vh" justify="center" align="center">
            <div>
              <p class="font-weight-bold text-h6">Learn even more!</p>
              <p>Unlock Premium features<br> only for $9.99 per month</p>
            </div>
            <v-spacer></v-spacer>
            <img src="https://img.icons8.com/ios/50/000000/brain--v2.png"/>
            <v-spacer></v-spacer>
          </v-row>
        </div>
                </div>
                <br>
                <br>
                </div>
            </v-col>
          </v-row>
      </v-col>

    </v-row>
    
  </div>
</template>

<script>
import { Icon } from '@iconify/vue2'
import Sidebar from '../components/SideBar.vue'

import Intro from '../components/Home/Intro.vue'
import AllCourses from '../components/Courses/AllCourses.vue'
  export default {
    name: 'Home',

    components: {
      Sidebar,
      Intro,
      AllCourses,
      
      Icon
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
      ],
      labels: [
        '12am',
        '3am',
        '6am',
        '9am',
        '12pm',
        '3pm',
        '6pm',
        '9pm',
      ],
      value: [
        200,
        675,
        410,
        390,
        310,
        460,
        250,
        240,
      ],
      
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
  .mi-height{
    height: 40vh;
  }
  @media only screen and (max-width: 600px) {
    .mi-height{
    height: 50vh;
  }
  }
 .v-sheet--offset {
    top: -24px;
    position: relative;
  }

</style>
