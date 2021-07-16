<template>
<div id="app">
  
  <v-card
    color="grey lighten-4"
    flat
    height="200px"
    tile
  >
    <v-toolbar >
      

      <v-toolbar-title>
     <v-tab to="/"><h1 style="font-family: 'Titillium Web', sans-serif">Rehaan Rasheed</h1></v-tab>
     </v-toolbar-title>

      <v-spacer></v-spacer>

      <v-tab to="/">
        <h4 style="font-family: 'Titillium Web', sans-serif">Home</h4>
      </v-tab>

      <v-tab to="/Services">
        <h4 style="font-family: 'Titillium Web', sans-serif">Services</h4>
      </v-tab>

      <v-tab to="/About">
        <h4 style="font-family: 'Titillium Web', sans-serif">About</h4>
      </v-tab>

      <v-tab to="/Contact">
        <h4 style="font-family: 'Titillium Web', sans-serif">Contacts</h4>
      </v-tab>

      <v-app-bar-nav-icon>
        
      </v-app-bar-nav-icon>
    </v-toolbar>

  <router-view></router-view>


    <v-spacer></v-spacer>
      <v-card>
        <v-container>
        <v-row class="text-center">
          
        <v-btn
          v-for="icon in icons"
          :key="icon"
          icon
        >
          <v-icon size="24px">
            {{ icon }}
          </v-icon>
        </v-btn>
        </v-row>
        </v-container>
 
      </v-card>
    <v-card>
      
<v-footer
    centered
    padless
  >
  <v-container>
    <v-row class="text-center"> 
    <v-col cols="4">

      <v-card-text class="white--text pt-0">

        <u><h1  style="font-family: 'Titillium Web', sans-serif">Rehaan Rasheed</h1></u>
        <br>
        <p >
          A 21 year old speed cuber from India and is the 2021 National Champion (Redbull, Rescramble event).
        </p>
      </v-card-text>
      <br>
      <v-divider></v-divider>
      <v-card-text class="white--text">
        {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
      </v-card-text>
    
    </v-col>
    <v-col cols="4">

      <u><h1 style="font-family: 'Titillium Web', sans-serif">Gallery</h1></u>
      <br>
      <br>
      <v-row><v-img
      max-height="70"
      max-width="95"
      src="https://image.shutterstock.com/image-photo/this-aerial-photograph-sydney-taken-600w-1050318920.jpg">
      </v-img>
      <v-col cols="1">
        </v-col>
      <v-img
      max-height="70"
      max-width="95"
      src="https://image.shutterstock.com/image-photo/blue-morpho-peleides-big-butterfly-600w-407651284.jpg">
      </v-img>
      <v-col cols="1">
        </v-col>
      <v-img
      max-height="70"
      max-width="95"
      src="https://image.shutterstock.com/image-photo/wings-butterflies-high-magnification-natural-600w-611026832.jpg">
      </v-img>
      </v-row>
    </v-col>
    <v-col cols="4">
      <u><h1 style="font-family: 'Titillium Web', sans-serif">Contact</h1></u>
    
      <br>
      <h4 style="font-family: 'Titillium Web', sans-serif">EMAIL :</h4>
      <h5 style="font-family: 'Titillium Web', sans-serif">anirbanbanik0000@gmail.com</h5>
      <br>
      <h4 style="font-family: 'Titillium Web', sans-serif">DEVELOPED BY :</h4>
      <h5 style="font-family: 'Titillium Web', sans-serif">Anirban Banik</h5>
    </v-col>
    </v-row>
    </v-container>
  </v-footer>
  
  </v-card>
  </v-card>

  
 </div>
</template>


<script>
  export default {
    name: 'Home',
    data: () => ({ 
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
      
      }),
  }
</script>




<style>
@import url('https://fonts.googleapis.com/css2?family=Barlow:wght@100&family=Titillium+Web:wght@200&display=swap');

html, body {
  font-family:  sans-serif;
}

#app {
  font-family: 'Roboto', sans-serif;
   
}
</style>