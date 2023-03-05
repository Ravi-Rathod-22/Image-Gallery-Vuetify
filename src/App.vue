<template>
  <v-app>
    <SideBar @selectOption="onSelectOptions" />
    <v-main>
      <!-- CARDS -->
      <ImageGallery :isWithColor="isWithColor"/>
    </v-main>
  </v-app>
</template>

<script>
import SideBar from "./components/SideBar.vue";
import ImageGallery from "./components/ImageGallery.vue";

export default {
  components:{
    SideBar,
    ImageGallery,
  },
  data() {
    return {
      isWithColor : true
    }
  },
  methods: {
    onSelectOptions  (isColor)  {
      this.isWithColor = isColor;
    }
  }
}

</script>
