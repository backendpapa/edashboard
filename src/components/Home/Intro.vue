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
      <div class="mt-4 ma-2">
           <v-row no-gutters>
           <v-col cols="12" xs="12" sm="12" md="12" xl="12" lg="12">
               <div class="pa-2 grey lighten-4" style="border-radius:15px;height:10vh">
                   <v-row no-gutters style="height:100%" align="center" justify="center">
                     
                         <v-col cols="1">
                               <div class="pa-1 ml-2 mt-n2 white" style="border-radius:15px;height:40px;width:40px">
                        <v-img width="30" height="30" src="../../assets/spain.png">

                        </v-img>
                       </div>
                         </v-col>
                       
                      <v-col cols="5">
                           <div class="mt-2 ml-5">
                           <p class="font-weight-bold">Spanish B2</p>
                           <p class="text-caption  mt-n4">By Backend Papa</p>
                       </div>
                      </v-col>
                   
                        <v-col cols="1">
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
                        </v-col>
                        
                        <v-col cols="5" class="">
                            <v-btn class="mt-n2  text-caption d-none d-sm-flex" color="black" dark style="text-transform:none;">Continue</v-btn>
                             <p class="text-right"><v-btn icon class="mt-n2   d-flex d-sm-none" color="black"  rounded><v-icon>mdi-monitor-dashboard</v-icon></v-btn></p>
                        </v-col>
                   </v-row>
               </div>
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