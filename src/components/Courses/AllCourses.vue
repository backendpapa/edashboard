<template>
  <div>
      <v-row no-gutters align="center" justify="center" class="grey lighten-4 pa-1  mb-2" v-for="i in  courses" :key="i.i" style="border-radius:15px">
          <v-col cols="2" xl="1" lg="1" sm="2" md="2" >
              <div class="white ml-2" style="width:40px;height:40px;border-radius:15px">
              <v-row no-gutters style="height:100%" align="center" justify="center">
                  <v-img class="ma-1" :src="i.img"></v-img>
              </v-row>
          </div>
          </v-col>
          <v-col cols="5" xl="4" md="5" sm="5" lg="4">
              <div class=" mt-3">
              <p class="font-weight-bold text-caption">{{i.title}}</p>
              <p class="mt-n5 text-caption">By Backendpapa</p>
          </div>
          </v-col>
         
         <v-col cols="4" xl="4" lg="4" md="4" sm="4">
              <div class="mt-3">
            <p><v-icon size="17px">mdi-clock</v-icon><span class="text-caption font-weight-bold ml-1">{{i.time}}</span></p>
          </div>
         </v-col>
         
         <v-col cols="1" xl="3" md="1" sm="1" lg="3">
              
               <p class="text-right mt-4"><v-btn icon right  plain color="black"  rounded><v-icon size="40px">mdi-menu-right-outline</v-icon></v-btn></p>
          
         </v-col>
      
        
      </v-row>
  </div>
</template>

<script>
export default {
    data(){
        return {
            courses:[
                {img:require('../../assets/figma.svg'),title:'Learn Figma',time:'6hr 30min',rating:'4.9'},
                {img:require('../../assets/shutter.png'),title:'Analog Photography',time:'3hr 15min',rating:'4.7'},
                {img:require('../../assets/insta.png'),title:'Master Instagram',time:'7hr 45min',rating:'4.6'},
                {img:require('../../assets/pen.png'),title:'Basics of Drawing',time:'11hr 30min',rating:'4.8'},
                {img:require('../../assets/photoshop.png'),title:'Photoshop Essence',time:'5hr 35min',rating:'4.7'}
            ]
        }
    }
}
</script>

<style>

</style>