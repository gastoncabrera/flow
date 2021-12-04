<template>
  <v-carousel
    v-model="model"
    next-icon
    prev-icon
    hide-delimiter-background
    class="carousel carousel--home"
    height="600"
  >
    <v-carousel-item
      v-for="proyect in proyects"
      :key="proyect.title"
      class="carousel_item"
    >
      <img :src="proyect.title" alt="" class="carousel_item__title" />

      <div class="carousel_item__content">
        <img
          :src="proyect.img_bg"
          alt=""
          class="carousel_item__image_background"
        />

        <img :src="proyect.img" alt="" class="carousel_item__image" />
      </div>
    </v-carousel-item>
  </v-carousel>
</template>
<script>
export default {
  props: {
    proyects: {
      typeof: String,
      require: true,
    },
  },

  data: () => ({
    model: 0,
  }),
};
</script>
<style lang="scss" >
@import "@/assets/scss/utils";

.carousel--home {
  margin-bottom: 100px;
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

.carousel--home {
  .v-carousel__controls.v-btn__content.v-icon {
    font-size: 6px;
  }

  .v-icon {
    font-size: 10px;
  }

  .v-btn__content {
    color: rgb(126, 122, 122);
    font-size: 3px;
  }

  .v-btn--icon.v-size--small {
    margin: 0 4px;
    height: 15px;
    width: 15px;
    color: black;
  }

  .v-btn > .v-btn__content .v-icon {
    color: black;
  }

  .v-carousel__controls__item:hover {
    background: #7e7a7a;
  }

  .v-carousel__controls__item:hover {
    background: #7e7a7a;
  }

  .v-icon .notranslate .mdi .mdi-circle .theme--dark {
    font-size: 5px;
  }

  .v-carousel__controls__item {
    margin: 0;
  }

  .v-btn .v-item--active .v-btn--active {
    color: black;
  }
}
</style>