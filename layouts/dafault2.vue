<template>
    <v-app>
        <v-system-bar
          color="indigo accent-2"
          :height="height"
          :lights-out="lightsOut"
          :window="window"
        >
        
        
          <v-spacer></v-spacer>
          <v-icon>mdi-wifi-strength-4</v-icon>
          <v-icon>mdi-signal-cellular-outline</v-icon>
          <v-icon>mdi-battery</v-icon>
          <span>12:30</span>
        </v-system-bar>
  <v-navigation-drawer app>
    <!-- -->
  </v-navigation-drawer>

  <div>
    <v-app-bar
      color="indigo darken-3"
      dense
      dark
      
    >
      <v-app-bar-nav-icon></v-app-bar-nav-icon>

      <v-toolbar-title>Title</v-toolbar-title>
      
    <!-- ยืดออก --> <v-spacer></v-spacer>
     
      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-heart</v-icon>
      </v-btn>
      <v-menu
        left
        bottom
      >
        <template v-slot:activator="{ on, attrs }">
          <v-btn
            icon
            v-bind="attrs"
            v-on="on"
          >
            <v-icon>mdi-dots-vertical</v-icon>
          </v-btn>
        </template>

        <v-list>
          <v-list-item
            v-for="n in 5"
            :key="n"
            @click="() => {}"
          >
            <v-list-item-title>Option {{ n }}</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
    </v-app-bar>
  </div>
  

  <!-- Sizes your content based upon application components -->
  <v-main>

    <!-- Provides the application the proper gutter -->
    <v-container fluid>

 
      <!-- If using vue-router -->
      <router-view></router-view>
    </v-container>
  </v-main>
    
  <v-footer
    color="indigo darken-3"
    padless
  >
    <v-row
      justify="center"
      no-gutters
    >
      <v-btn
        v-for="link in links"
        :key="link"
        color="white"
        text
        rounded
        class="my-2"
      >
        {{ link }}
      </v-btn>
      <v-col
        class="indigo accent-2 text-center white--text"
        cols="12"
      >
        {{ new Date().getFullYear() }} — <strong>อินทิรา ภูผาทอง</strong>
      </v-col>
    </v-row>
  </v-footer>
</v-app>
</template>
<script>
  export default {
    data: () => ({
      links: [
        'Home',
        'Profile',
        'Team',
      
      ],
    }),
  }
</script>