<template>
    <nav>
        <v-app-bar
      app
      color="indigo darken-4"
      dark
      flat
      height="80px"
    >
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="../assets/pngegg.png"
          transition="scale-transition"
          width="40"
        />

        <v-text class="white--text text-h5" style="font-weight:bold;">BANK INDONESIA BALI</v-text>
      </div>

      <v-spacer></v-spacer>

      <Date/>
    </v-app-bar>
    </nav>
</template>

<script>
import Date from '@/components/Date.vue'
export default {
    components: {
        Date,
    }
}
</script>