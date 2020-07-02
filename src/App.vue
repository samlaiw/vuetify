<template>
  <v-app>
    <div v-if="path">
      <Navbar />
    </div>
    <v-content>
      <router-view></router-view>
    </v-content>
  </v-app>
</template>

<script>
import Navbar from '@/components/Navbar'
export default {
  name: 'App',

  components: {
    Navbar
  },

  data: () => ({
    path: 'routes'
    
  }),
};
</script>
