<template>
  <v-app>
    <v-container>
    <v-row>
      <v-col>
<!-- <Header/> -->
      </v-col>
      <v-col>
<IndexPage/>
      </v-col>


    </v-row>
    </v-container>

    
  </v-app>
</template>

<script>
import Login from '../components/user/Login.vue'
import Header from '../layout/Header'
import IndexPage from '../pages/Home'

export default {
  name: 'App',
  // data() {
  //   return {
  //     //
  //   }
  // },
 components: {
  Login,
  Header,
  IndexPage
  }
}
</script>
