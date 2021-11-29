<template>
  <div class="raised_money">
    <div class="raised_money__container_pills">
      <Pill />
      <Pill />
      <Pill />
    </div>
    <div class="raised_money__container_money custom_container">
      <img class="raised_money__image_mobile" src="J-Balvin_media.png" alt="" />
      <img class="raised_money__image_destock" src="j-balvin.png" alt="" />
      <div class="raised_money__million">
        <span class="raised_money__number">$800</span> MILLION
      </div>
      <div class="raised_money__description">
        RAISED ACROSS ECOSYSTEM PROJECTS
      </div>
    </div>
  </div>
</template>

<script>
import Pill from "@/components/Home/Pill";

export default {
  components: { Pill },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.raised_money {
  position: relative;
  margin-bottom: 300px;
  display: flex;
  align-items: center;
  flex-direction: column;
  background-image: url("/greeVector.jpg");
  background-position: center;
  background-size: cover;

  @include breakpoint(sm) {
    padding-bottom: 100px;
  }
}

.raised_money__container_money {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-top: 30px;

  @include breakpoint(sm) {
    margin-top: 100px;
  }
}

.raised_money__image_mobile {
  max-width: 200px;

  @include breakpoint(sm) {
    display: none;
  }
}

.raised_money__image_destock {
  display: none;

  @include breakpoint(sm) {
    display: block;
    position: absolute;
    right: 0;
    bottom: 0;
    max-height: 390px;
  }
}

.raised_money__million {
  display: flex;
  flex-direction: column;
  text-align: center;
  width: 100%;
  height: 100%;
  max-width: 1000px;
  font-family: $font_2;
  font-size: 48px;
  line-height: 64px;
  font-weight: 800;
  color: white;
  background-image: linear-gradient(180deg, #16ff99, #02d87e);
  border-radius: 600px;
  padding: 24px 30px;

  @include breakpoint(sm) {
    font-size: 70px;
    line-height: 78px;
    padding: 70px 38px;
  }
}

.raised_money__number {
  font-size: 80px;
}

.raised_money__description {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  font-family: $font_2;
  line-height: 38px;
  font-weight: 700;
  font-size: 28px;
  color: #16ff99;
  margin-top: 24px;
  padding-left: 16px;
  padding-right: 16px;
}
</style>