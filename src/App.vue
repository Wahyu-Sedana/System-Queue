<template>
  <v-app>
    <Navbar/>
    <v-main class="indigo darken-3 mt-5">
      <Content/>
    </v-main>
    <Footer/>
  </v-app>
</template>

<script>
import Content from './components/Content';
import Navbar from './components/Navbar';
import Footer from './components/Footer';

export default {
  name: 'App',

  components: {
    Content,
    Navbar,
    Footer
  },

  data: () => ({
    //
  }),
};
</script>
