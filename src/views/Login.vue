<template>
  <div class="">
     <v-row no-gutters align="center" justify="center" style="height:100vh">
       <v-col cols="8" sm="10" md="10" xl="4" lg="4">
         <p>Welcome to E-Dashboard</p>
         <v-card style="height:50vh" >
           <v-subheader class="grey lighten-2">
             Login
           </v-subheader>
           <div class="ma-2">
             <p class="text-caption ">Username</p>
             <v-text-field outlined dense prepend-inner-icon="mdi-account" class="text-caption mt-n3" placeholder="Enter in your username"></v-text-field>

              <p class="text-caption ">Password</p>
             <v-text-field outlined dense prepend-inner-icon="mdi-lock" class="text-caption mt-n3" placeholder="Enter in your Password"></v-text-field>
             <v-btn block @click="login" style="text-transform:none" class="orange" dark> Login</v-btn>
           </div>
         </v-card>
       </v-col>
     </v-row>
  </div>
</template>

<script>
export default {
  data(){
    return {

    }
  },
  methods:{
    login(){
      this.$router.push('/course/overview')
    }
  }
}
</script>

<style>

</style>