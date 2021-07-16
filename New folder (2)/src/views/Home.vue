<template>
  <div class="home">

  <v-card>
<template>
  <v-carousel 
  cycle
  :show-arrows="false">
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      reverse-transition="fade-transition"
      transition="fade-transition"
    ></v-carousel-item>
  </v-carousel>
</template>

<br> <br> <br>



  <v-card>
    <v-container>
      <v-row>
      <v-col cols="12">

      <u><h1 style="font-family: 'Titillium Web', sans-serif">Gallery</h1></u>
      <br>
      <br>
      <v-row>
      <v-img cols="4"
      max-height="300"
      max-width="325"
      src="https://image.shutterstock.com/image-photo/this-aerial-photograph-sydney-taken-600w-1050318920.jpg">
      </v-img>
      <v-col cols="1">
        </v-col>
      <v-img cols="4"
      max-height="300"
      max-width="325"
      src="https://image.shutterstock.com/image-photo/blue-morpho-peleides-big-butterfly-600w-407651284.jpg">
      </v-img>
      <v-col cols="1">
        </v-col>
      <v-img cols="4"
      max-height="300"
      max-width="325"
      src="https://image.shutterstock.com/image-photo/wings-butterflies-high-magnification-natural-600w-611026832.jpg">
      </v-img>
      </v-row>
    <br><br>
      <v-row><v-img cols="4"
      max-height="300"
      max-width="325"
      src="https://image.shutterstock.com/image-photo/vibrant-velvet-green-copper-grey-600w-1785984722.jpg">
      </v-img>
      <v-col cols="1">
        </v-col>
      <v-img cols="4"
      max-height="300"
      max-width="325"
      src="https://image.shutterstock.com/image-photo/top-view-aerial-photo-amazingly-600w-1961439181.jpg">
      </v-img>
      <v-col cols="1">
        </v-col>
      <v-img cols="4"
      max-height="300"
      max-width="325"
      src="https://image.shutterstock.com/image-photo/03052021-latvia-fishing-boats-floating-600w-1970152138.jpg">
      </v-img>
      </v-row>
    <br><br>
      <v-row><v-img cols="4"
      max-height="300"
      max-width="325"
      src="https://image.shutterstock.com/image-photo/creative-layout-made-green-leaves-600w-770742391.jpg">
      </v-img>
      <v-col cols="1">
        </v-col>
      <v-img cols="4"
      max-height="300"
      max-width="325"
      src="https://image.shutterstock.com/image-photo/santiago-de-chile-6-november-600w-1557932828.jpg">
      </v-img>
      <v-col cols="1">
        </v-col>
      <v-img cols="4"
      max-height="300"
      max-width="325"
      src="https://image.shutterstock.com/image-photo/santiago-de-chile-29-october-600w-1556903228.jpg">
      </v-img>
      </v-row>
      <br><br><br><br>
    </v-col>
    </v-row>
    </v-container>
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
        items: [
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg',
          },
        ],

      }),
  }
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Barlow:wght@100&family=Titillium+Web:wght@200&display=swap');

</style>
