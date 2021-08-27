<template>
  <div>
      <div style="position:relative" class="ma-2">
         
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
      <div class="mt-4">
           <v-row no-gutters>
           <v-col cols="10" xs="12" sm="12" md="12" xl="10" lg="10">
               <div class="pat-2 grey lighten-4" style="border-radius:15px;height:10vh">
                   <v-row no-gutters style="height:100%" align="center" justify="center">
                     
                           <div class="pa-1 ml-2 mt-n2 white" style="border-radius:15px;height:40px;width:40px">
                        <v-img width="30" height="30" src="../../assets/spain.png">

                        </v-img>
                       </div>
                       
                       <div class="mt-2 ml-2">
                           <p class="font-weight-bold">Spanish B2</p>
                           <p class="text-caption  mt-n4">By Backend Papa</p>
                       </div>
                       <v-spacer></v-spacer>
                        <v-progress-circular
                        :rotate="360"
                        :size="35"
                        :width="3"
                        :value="85"
                        color="black"
                        class="ml-5 mt-n3"
                        
                        >
                    <span style="font-size:12px" class="font-weight-bold">85%</span>
                        </v-progress-circular>
                        <v-spacer></v-spacer>
                        <v-btn class="mt-n2 mr-10 text-caption" color="black" dark style="text-transform:none;width:8rem">Continue</v-btn>
                   </v-row>
               </div>
           </v-col>
           <v-col cols="2">
               <v-row style="height:100%" no-gutters>
                   <v-icon class="ml-2" color="black" size="40px">mdi-arrow-left-circle-outline</v-icon>
                   <v-icon class="ml-2" color="black" size="40px">mdi-arrow-right-circle-outline</v-icon>
               </v-row>
           </v-col>
       </v-row>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>