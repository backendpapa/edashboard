<template>
  <div>
       <v-navigation-drawer style="height:90vh;border-radius:15px" class="ma-4 black shadow" width="100" permanent>
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title class="text-center text-h2 white--text font-weight-bold">
            B.
          </v-list-item-title>
          
        </v-list-item-content>
      </v-list-item>

      <v-divider class="mb-5"></v-divider>

      
      <div style="width:100%">
         <v-btn text block to="/" plain><p class="text-center "><v-icon size="35px" color="white">mdi-home-outline</v-icon></p></v-btn>
        <div class="mb-5"></div>
        <v-btn text block to="/hat" plain><p class="text-center"><v-icon size="35px" color="white">mdi-school-outline</v-icon></p></v-btn>
        <div class="mb-5"></div>
        <v-btn text block to="/hat" plain><p class="text-center"><v-icon size="35px" color="white">mdi-account-outline</v-icon></p></v-btn>
        <div class="mb-5"></div>
        <v-btn text block to="/hat" plain><p class="text-center"><v-icon size="35px" color="white">mdi-tooltip-text-outline</v-icon></p></v-btn>
        <div class="mb-5"></div>
        <v-btn text block to="/hat" plain><p class="text-center"><v-icon size="35px" color="white">mdi-cog-outline</v-icon></p></v-btn>
      </div>
       
      <div style="position:absolute;bottom:0;width:100%">
        <v-btn text block to="/hat" plain><p class="text-center"><v-icon size="35px" color="white">mdi-login</v-icon></p></v-btn>
      </div>
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.shadow{
   box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}
</style>