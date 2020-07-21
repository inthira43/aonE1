<template>
<v-card color="#DAA520">
  <v-container fluid class="pa-0" > 
    <v-row align="center">
      <v-col cols="12" sm="6">
        <div class="text-center">
          <div class="my-2">
            <nuxt-link to="/activity/line"><v-btn x-small color="secondary" dark>กิจกรรมเข้าเเถว</v-btn> </nuxt-link>
          </div>
          <div class="my-2">
            <nuxt-link to="/activity/homeroom"> <v-btn small color="primary" dark>กิจกรรม Homeroom</v-btn> </nuxt-link>
          </div>
          <div class="my-2">
           <nuxt-link to="/activity/special"> <v-btn color="warning" dark>กิจกรรมพิเศษ</v-btn> </nuxt-link>
          </div>
          <div class="my-2">
             <nuxt-link to="/activity/flag"> <v-btn color="error" dark large>กิจกรรมวิชาชีพ</v-btn> </nuxt-link>
          </div>
          <div class="my-2">
            <nuxt-link to="/"> <v-btn x-large color="success" dark>กลับหน้าหลัก</v-btn> </nuxt-link>
          </div>
        </div>
      </v-col>
      <v-col cols="12" sm="6">
        <div class="text-center">
          
          <div class="my-2">
             <nuxt-link to="/Login"><v-btn color="primary" fab x-large dark>
               <h4>Login</h4>
            </v-btn></nuxt-link>
          </div>
        </div>
      </v-col>
    </v-row>
  </v-container>
</v-card>
</template>