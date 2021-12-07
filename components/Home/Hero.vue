<template>
  <div class="hero">
    <div class="hero__container custom_container">
      <h1 class="hero__left">A new world awaits #onflow</h1>

      <nuxt-link to="" class="hero__center">
        <img class="hero__center_image" src="~/static/play.svg" alt="" />
      </nuxt-link>

      <img
        src="~/static//FlowLogo_Horizontal_Green.svg"
        alt=""
        class="hero__right"
      />
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.hero {
  margin-top: 100px;
  background-position: center;
  background-size: cover;
  background-image: url("~/static/heroimage_mobile.jpg");

  @include breakpoint(md) {
    background-image: url("~/static/bg.jpg");
    min-height: 550px;
  }

  @include breakpoint(lg) {
    column-gap: 50px;
    min-height: 750px;
  }
}

.hero__container {
  min-height: 405px;
  width: 100%;
  height: 100%;
  padding-bottom: 32px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding-top: 54px;

  @include breakpoint(md) {
    min-height: 550px;
    display: grid;
    justify-items: center;
    grid-template-columns: minmax(0, 1fr) minmax(0, 150px) minmax(0, 1fr);
    grid-template-areas: "left center right";
  }

  @include breakpoint(lg) {
    column-gap: 150px;
    min-height: 750px;
  }
}

.hero__left {
  font-family: $font_2;
  font-size: 64px;
  line-height: 58px;
  font-weight: 800;
  text-align: center;
  margin: 0 16px;

  @include breakpoint(md) {
    grid-area: left;
    text-align: left;
    line-height: 50px;
    margin: 0;
  }
}

.hero__center_image {
  margin-top: 54px;
  width: 100%;
  max-width: 100px;

  @include breakpoint(md) {
    grid-area: center;
  }

  @include breakpoint(lg) {
    max-width: 130px;
  }
}

.hero__right {
  display: none;

  @include breakpoint(md) {
    grid-area: right;
    display: block;
    width: 100%;
  }
}
</style>