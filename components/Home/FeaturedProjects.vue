<template>
  <div class="featured_projects">
    <h1 class="featured_projects__title">PROJECT SPOTLIGHT</h1>
    <Carousel />
  </div>
</template>

<script>
import Carousel from "@/components/Home/Carousel";

export default {
  components: { Carousel },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";
.featured_projects__title {
  text-align: center;
  font-family: $font_2;
  font-size: 48px;
  font-weight: 900;
  line-height: 42px;
  color: black;
  margin-left: 16px;
  margin-right: 16px;
}
</style>