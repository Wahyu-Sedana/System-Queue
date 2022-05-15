<template>
  <v-carousel
    cycle
    height="425"
    hide-delimiter-background
    :show-arrows="false"
  >
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    ></v-carousel-item>
  </v-carousel>
</template>
<script>
  export default {
    data () {
      return {
         items: [
          {
            src: 'https://www.bi.go.id/id/publikasi/ruang-media/news-release/PublishingImages/sp_2325421.jpg',
          },
          {
            src: 'https://www.bi.go.id/id/publikasi/ruang-media/news-release/PublishingImages/sp_2327021.jpg',
          },
          {
            src: 'https://tf.ugm.ac.id/wp-content/uploads/sites/589/2022/03/Untitled-720x510.png',
          },
          {
            src: 'https://www.porosbali.com/uploads/berita/berita_BankIndonesiaSerahkanBantuanPSBIMendukungProgramKemandirianYayasanKaumDifabel.jpg',
          },
        ]
      }
    },
  }
</script>