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
           <v-row align="center" no-gutters justify="center" class="grey lighten-4 pa-1" style="border-radius:15px;height:10vh" >
                    <div class="white" style="border-radius:15px;height:8vh;">
                     <v-img src="../../assets/spain.png">
                     </v-img>
                     </div>
                   
                           <div class="">
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
                        
                        
                        >
                    <span style="font-size:12px" class="font-weight-bold">85%</span>
                        </v-progress-circular>
                        
                        
                       
                            <v-btn class="  text-caption d-none d-sm-flex" color="black" dark style="text-transform:none;">Continue</v-btn>
                             <p class="text-right"><v-btn icon class="   d-flex d-sm-none" color="black"  rounded><v-icon>mdi-monitor-dashboard</v-icon></v-btn></p>
                       
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