<template>
  <div>
      <v-row no-gutters align="center" justify="center" class="grey lighten-4 pa-1  mb-2" v-for="i in  courses" :key="i.i" style="border-radius:15px">
          <v-col cols="1">
              <div class="white ml-2" style="width:40px;height:40px;border-radius:15px">
              <v-row no-gutters style="height:100%" align="center" justify="center">
                  <v-img class="ma-1" :src="i.img"></v-img>
              </v-row>
          </div>
          </v-col>
          <v-col cols="4">
              <div class=" mt-3">
              <p class="font-weight-bold text-caption">{{i.title}}</p>
              <p class="mt-n5 text-caption">By Backendpapa</p>
          </div>
          </v-col>
         
         <v-col cols="3">
              <div class="mt-3">
            <p><v-icon size="17px">mdi-clock</v-icon><span class="text-caption font-weight-bold ml-1">{{i.time}}</span></p>
          </div>
         </v-col>
         
         <v-col cols="2">
              <div class="mt-3">
              <p class="mt-2"><v-icon class="mt-n2 mr-2">mdi-fire</v-icon> <span class="font-weight-bold ">{{i.rating}}</span></p>
          </div>
         </v-col>
      
         <v-col cols="2" >
              <v-btn  color="black" dark style="text-transform:none" class="text-caption pr-2">View Course</v-btn>
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