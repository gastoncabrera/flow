<template>
  <v-carousel
    v-model="model"
    next-icon
    prev-icon
    class="carousel carousel--home"
    height="600"
  >
    <v-carousel-item v-for="slide in slider" :key="slide" class="carousel_item">
      <img :src="slide.title" alt="" class="carousel_item__title" />
      <div class="carousel_item__content">
        <img
          :src="slide.image"
          alt=""
          class="carousel_item__image_background"
        />
        <img
          :src="slide.image_background"
          alt=""
          class="carousel_item__image"
        />
      </div>
    </v-carousel-item>
  </v-carousel>
</template>
<script>
export default {
  data: () => ({
    model: 0,
    slider: [
      {
        title: "/title_genies.svg",
        image: "/Rectangle 1.png",
        image_background: "/jakeGroup.png",
      },
      {
        title: "/chainmonsters-logo-1.png",
        image: "/Rectangle 2.png",
        image_background: "/Group 793.png",
      },
      {
        title: "/top-shot_logo_Layer 2.svg",
        image: "/Rectangle 3.png",
        image_background: "/Group_145.png",
      },
    ],
  }),
};
</script>
<style lang="scss" >
.carousel--home {
  .carousel_item {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .carousel_item__title {
    height: 50px;
    width: 100%;
    max-width: 200px;
    object-fit: contain;
    display: flex;
    margin: 0 auto;
    margin-top: 42px;
    margin-bottom: 32px;
  }

  .carousel_item__content {
    position: relative;
    width: 300px;
    height: 100%;
    margin-bottom: 64px;
  }

  .carousel_item__image {
    max-width: 100%;
    position: absolute;
    top: 32px;
    z-index: 1;
  }

  .carousel_item__image_background {
    max-width: 100%;
    position: absolute;
    top: 0;
    padding-left: 24px;
    padding-right: 24px;
  }
}
</style>