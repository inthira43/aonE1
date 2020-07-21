<template>
<center>
   <v-card color="#663399" >
     <v-card-title>
       <h1>Login</h1>
     </v-card-title>
     <v-card-text>
       <v-form>
         <v-text-field label="Username" prepend-icon="mdi-account-circle" />
         <v-text-field 
            :type="showPassword ? 'text' : 'password'" 
            label="Password"
            prepend-icon="mdi-lock"
            :append-icon="showPassword ? 'mdi-eye' : 'mdi-eye-off'"
            @click:append="showPassword = !showPassword"
          />

       <v-card-actions>
        <nuxt-link to="/Ragister" ><v-btn color="success"  dark >Ragister</v-btn> </nuxt-link>
         <v-spacer></v-spacer>
        <nuxt-link to="" ><v-btn color="primary"  dark >Login</v-btn> </nuxt-link>
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