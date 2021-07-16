<template>
<div class="contact">
    <v-form v-model="valid">
    <v-container>
    <v-row>
      <v-col cols="3"></v-col>
      <v-col cols="6">
      <br><br><br>
      <center><h1 style="font-family: 'Titillium Web', sans-serif">Contact</h1></center>

      <br><br><br>
        
          <v-text-field
            v-model="firstname"
            :rules="nameRules"
            :counter="10"
            label="First name"
            required
          ></v-text-field>
        
          <v-text-field
            v-model="lastname"
            :rules="nameRules"
            :counter="10"
            label="Last name"
            required
          ></v-text-field>
        
          <v-text-field
            v-model="email"
            :rules="emailRules"
            label="E-mail"
            required
          ></v-text-field>

          <br><br><br>
          <center>
            <v-btn
            depressed
            outlined
            small
          >SUBMIT</v-btn>
          </center>

          <br><br><br>
          <br><br><br>
        
      
      </v-col>
      <v-col cols="3"></v-col>
    </v-row>
    </v-container>
  </v-form>

</div>
</template>

<script>
  export default {
    data: () => ({
      valid: false,
      firstname: '',
      lastname: '',
      nameRules: [
        v => !!v || 'Name is required',
        v => v.length <= 10 || 'Name must be less than 10 characters',
      ],
      email: '',
      emailRules: [
        v => !!v || 'E-mail is required',
        v => /.+@.+/.test(v) || 'E-mail must be valid',
      ],
    }),
  }
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Barlow:wght@100&family=Titillium+Web:wght@200&display=swap');

</style>