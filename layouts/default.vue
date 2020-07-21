 <template>
 <!-- ส่วนบนสุด vuetifyjs -->
     <v-app>
         <v-card height="720px">
            <v-card-title class="Light purple white--text">
              <v-app-bar-nav-icon></v-app-bar-nav-icon>
                <v-toolbar-title>Page title</v-toolbar-title>
                <v-spacer></v-spacer>
                  <v-btn icon>
                   <nuxt-link to="/"> <v-icon>mdi-heart</v-icon></nuxt-link>
                  </v-btn>
                  <v-btn icon>
                    <v-icon>mdi-magnify</v-icon>
                  </v-btn>
                <v-icon>mdi-dots-vertical</v-icon>

            </v-card-title>
            <v-content>
              <nuxt/>
            </v-content>
         </v-card>
         <!-- ส่วนเนื้อหา -->
        
     </v-app>

 </template>