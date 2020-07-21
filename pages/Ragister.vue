<template>
<center>
   <v-card color="#336699" >
     <v-card-title>
       <h1>สมัครสมาชิก</h1>
     </v-card-title>
     <v-card-text>
       <v-form>

        <v-text-field label="Name" 
        :counter="10"
        :rules="nameRules"
         prepend-icon="mdi-account-circle" />
        <v-text-field label="E-mail" prepend-icon="mdi-email" />

       <v-card-actions>
        <nuxt-link to="/Ragister" ><v-btn color="success"  dark >Ragister</v-btn> </nuxt-link>
         <v-spacer></v-spacer>
        <nuxt-link to="/Login" ><v-btn color="primary"  dark >Login</v-btn> </nuxt-link>
        </v-card-actions>

       </v-form>
     </v-card-text>
   </v-card>
   </center>
</template>
<script>
export default {
  name: 'App',
  data () {
    return {
      showPassword: false
    }
  }
}
</script>