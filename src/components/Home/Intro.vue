<template>
  <div class="">
      <v-container>
      <div style="position:relative" class="">
         
      <div style="min-height:10vh;height:20vh;border-radius:15px;" class="grey lighten-4 ">
         <v-row no-gutters align="center" justify="center" style="z-index:0;height:100%">
             <div class="pa-5">
                 <p class="font-weight-bold text-h4">Hello Josh!</p>
                <p class="font-weight-bold mt-n4">It's good to see you again.</p>
             </div>
             <v-spacer></v-spacer>
              <v-img style="position:absolute;bottom:0;right:0;z-index:2;margin-right:6rem" class="" max-width="135" max-height="220" src="../../assets/2.png"></v-img>
         </v-row>
        
      </div>
      
      </div>
      <!-- Info 2 -->
      <div class="mt-4 pa-2">
          <v-row align="center" style="border-radius:15px"  class="grey lighten-4 pa-1">
              <v-col cols="3" sm="3" md="3" xl="1" lg="1" >  
                  <div class="white pa-1" style="border-radius:15px;height:8vh;width:8vh">
                     <v-img src="../../assets/spain.png">
                     </v-img>
                     </div>
              </v-col>
              <v-col style="height:100%;"   cols="5" xl="4" lg="4" sm="5" md="5" class=" pt-6">
                  <p style="margin:auto" class="font-weight-bold">Spanish B2</p>
                  <p class="text-caption  ">By Backend Papa</p>
              </v-col>
              <v-col cols="2" sm="2" md="2" xl="1" lg="1" class="">
                   <v-progress-circular
                        :rotate="360"
                        :size="35"
                        :width="3"
                        :value="85"
                        color="black"
                        
                        
                        >
                    <span style="font-size:12px" class="font-weight-bold">85%</span>
                        </v-progress-circular>
              </v-col>
              <v-col cols="2" xl="6" lg="6" sm="2" md="2"  style="width:100%">
                    <p  class="text-center d-none d-sm-flex"><v-btn  class="  text-caption " color="black" dark style="text-transform:none;">Continue</v-btn></p>
                           <v-btn icon  plain class="   d-flex d-sm-none" color="black"  rounded><v-icon size="40px">mdi-menu-right-outline</v-icon></v-btn>  
              </v-col>
          </v-row>
      </div>


     
      </v-container>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>