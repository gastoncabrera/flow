<template>
  <div class="card_hero" :style="{ 'background-image': `/flow/${background}` }">
    <span class="card_hero__title">{{ title }}</span>
    <p class="card_hero__subtitle">{{ subtitle }}</p>
  </div>
</template>

<script>
export default {
  props: {
    background: {
      type: String,
      default: "url(/card/Frame_4.png)",
    },

    title: {
      type: String,
      require: true,
    },

    subtitle: {
      type: String,
      require: true,
    },
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.card_hero {
  height: 200px;
  width: 100%;
  background-position: center;
  background-size: cover;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 40px;
  padding-right: 20px;
  padding-left: 20px;
  border-radius: 10px;
  overflow: hidden;
  margin-top: 16px;
  margin-bottom: 16px;

  @include breakpoint(sm) {
    height: 300px;
  }

  @include breakpoint(md) {
    margin: 0;
    height: 310px;
  }
}

.card_hero__title {
  font-family: $font_2;
  font-size: 48px;
  font-weight: 900;
  color: black;
  text-align: center;
  line-height: 54px;

  @include breakpoint(sm) {
    font-size: 62px;
    letter-spacing: 3px;
  }

  @include breakpoint(md) {
    font-size: 48px;
    line-height: 48px;
  }

  @include breakpoint(lg) {
    font-size: 62px;
  }
}

.card_hero__subtitle {
  font-family: $font_1;
  font-size: 16px;
  font-weight: 500;
  color: black;
  text-align: center;

  @include breakpoint(sm) {
    font-size: 19px;
  }

  @include breakpoint(lg) {
    margin-top: 16px;
    font-size: 24px;
  }
}
</style>