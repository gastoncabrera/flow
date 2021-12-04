<template>
  <div class="carousel_desktop">
    <div
      class="carousel_desktop__container"
      v-for="proyect in proyects"
      :key="proyect.title"
    >
      <img :src="proyect.title" alt="" class="carousel_desktop__title" />

      <div class="carousel_desktop__content">
        <img
          :src="proyect.img_bg"
          alt=""
          class="carousel_desktop__image_background"
        />

        <img :src="proyect.img" alt="" class="carousel_desktop__image" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    proyects: {
      typeof: String,
      require: true,
    },
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.carousel_desktop {
  display: flex;
  width: 100%;
  height: 100%;
  padding-bottom: 300px;
}

.carousel_desktop__container {
  position: relative;
  height: 100%;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin: 0 20px;
}

.carousel_desktop__title {
  height: 50px;
  width: 100%;
  max-width: 200px;
  object-fit: contain;
  display: flex;
  margin: 0 auto;
  margin-top: 42px;
  margin-bottom: 32px;
}

.carousel_desktop__content {
  position: relative;
  width: 100%;
  height: 100%;
  margin-bottom: 64px;
}

.carousel_desktop__image_background {
  max-width: 100%;
  position: absolute;
  top: 0;
  padding-left: 24px;
  padding-right: 24px;
}

.carousel_desktop__image {
  max-width: 100%;
  position: absolute;
  top: 32px;
  z-index: 1;
}
</style>