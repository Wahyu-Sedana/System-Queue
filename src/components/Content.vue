<template>
  <v-container>
    <v-row>
      <v-col cols="12" sm="6">
        <v-card style="border: 1px solid white">
          <v-card-title class="indigo darken-4 white--text justify-center text-h3">NAMA COUNTER</v-card-title>
          <v-card-title class="indigo darken-4 white--text justify-center text-h2" style="font-weight:bold;">TELLER</v-card-title>
        </v-card>
        <br>
        <v-card style="border: 1px solid white" @keyup.enter="clickData()" @click="clickData()">
          <v-card-title class="indigo darken-4 white--text justify-center text-h3">NOMOR TERPANGGIL</v-card-title>
          <v-card-title class="indigo darken-4 yellow--text justify-center text-h1" style="font-weight:bold;">00{{antrian}}</v-card-title>
        </v-card>
        <br>
      </v-col>
      <v-col cols="12" sm="6">
      <Slider/>
      </v-col>
    </v-row>
    <br>
    <v-row>
      <v-col cols="12" lg="2">
        <v-card style="border: 1px solid white">
           <v-card-title class="indigo darken-4 white--text justify-center text-h4" style="height:130px;"><p>NOMOR</p><p>ANTRIAN</p></v-card-title>
        </v-card>
      </v-col>
       <v-col cols="12" lg="2">
        <v-card style="border: 1px solid white">
           <v-card-title class="indigo darken-4 yellow--text justify-center text-h1" style="height:130px; font-weight:bold;">002</v-card-title>
        </v-card>
      </v-col>
       <v-col cols="12" lg="2">
        <v-card style="border: 1px solid white">
            <v-card-title class="indigo darken-4 yellow--text justify-center text-h1" style="height:130px; font-weight:bold;">003</v-card-title>
        </v-card>
      </v-col>
       <v-col cols="12" lg="2">
        <v-card style="border: 1px solid white">
            <v-card-title class="indigo darken-4 yellow--text justify-center text-h1" style="height:130px; font-weight:bold;">004</v-card-title>
        </v-card>
      </v-col>
       <v-col cols="12" lg="2">
        <v-card style="border: 1px solid white">
            <v-card-title class="indigo darken-4 yellow--text justify-center text-h1" style="height:130px; font-weight:bold;">005</v-card-title>
        </v-card>
      </v-col>
       <v-col cols="12" lg="2">
        <v-card style="border: 1px solid white">
           <v-card-title class="indigo darken-4 yellow--text justify-center text-h1" style="height:130px;font-weight:bold;">006</v-card-title>
        </v-card>
      </v-col>
            <v-col cols="12" lg="2">
        <v-card style="border: 1px solid white">
           <v-card-title class="indigo darken-4 white--text justify-center text-h4" style="height:130px"><p>NAMA</p><p>COUNTER</p></v-card-title>
        </v-card>
      </v-col>
       <v-col cols="12" lg="2">
        <v-card style="border: 1px solid white">
            <v-card-title class="indigo darken-4 white--text justify-center text-h5" style="height:130px; font-weight:bold;">TELLER</v-card-title>
        </v-card>
      </v-col>
       <v-col cols="12" lg="2">
        <v-card style="border: 1px solid white">
            <v-card-title class="indigo darken-4 white--text justify-center text-h5" style="height:130px; font-weight:bold;">CS</v-card-title>
        </v-card>
      </v-col>
       <v-col cols="12" lg="2">
        <v-card style="border: 1px solid white">
            <v-card-title class="indigo darken-4 white--text justify-center text-h5" style="height:130px; font-weight:bold;">PAJAK</v-card-title>
        </v-card>
      </v-col>
       <v-col cols="12" lg="2">
        <v-card style="border: 1px solid white">
            <v-card-title class="indigo darken-4 white--text justify-center text-h5" style="height:130px; font-weight:bold;">KREDIT</v-card-title>
        </v-card>
      </v-col>
       <v-col cols="12" lg="2">
        <v-card style="border: 1px solid white">
            <v-card-title class="indigo darken-4 white--text justify-center text-h5" style="height:130px; font-weight:bold;">OVER BOOKING</v-card-title>
        </v-card>
      </v-col>        
    </v-row>
  </v-container>
</template>

<script>
import Slider from '@/components/Slider.vue'
  export default {
    name: 'Content',

    data: () => ({
    antrian : 1,
    }),
    components: {
      Slider
    },

    methods: {
      clickData: function(){
        this.antrian++;
      }
    },
  }
</script>
