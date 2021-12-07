<template>
  <div class="featured_projects custom_container">
    <h1 class="featured_projects__title">PROJECT SPOTLIGHT</h1>

    <CarouselMobile
      class="featured_projects__carousel_mobile"
      :proyects="proyects"
    />

    <CarouselDesktop
      class="featured_projects__carousel_desktop"
      :proyects="proyects"
    />
  </div>
</template>

<script>
import CarouselMobile from "@/components/Home/CarouselMobile";
import CarouselDesktop from "@/components/Home/CarouselDesktop";

export default {
  components: { CarouselDesktop, CarouselMobile },
  data() {
    return {
      proyects: [
        {
          title: "~/static/title_genies.svg",
          img_bg: "~/static/Rectangle 1.png",
          img: "~/static/jakeGroup.png",
        },

        {
          title: "chainmonsters-logo-1.png",
          img_bg: "Rectangle 2.png",
          img: "Group 793.png",
        },

        {
          title: "top-shot_logo_Layer 2.svg",
          img_bg: "Rectangle 3.png",
          img: "Group_145.png",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.featured_projects__title {
  text-align: center;
  font-family: $font_2;
  font-size: 48px;
  line-height: 48px;
  font-weight: 900;
  color: black;
  margin-bottom: 40px;

  @include breakpoint(md) {
    font-size: 62px;
    margin-bottom: 50px;
  }
}

.featured_projects__carousel_mobile {
  @include breakpoint(md) {
    display: none;
  }
}

.featured_projects__carousel_desktop {
  display: none;

  @include breakpoint(md) {
    display: flex;
  }
}
</style>