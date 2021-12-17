<template>
  <div>
    <Hero />

    <PropertyImage />

    <Dao />

    <Apartment />

    <House />

    <hr />

    <Questions />
  </div>
</template>

<script>
import Hero from "@/components/Home/Hero";
import PropertyImage from "@/components/Home/PropertyImage";
import Dao from "@/components/Home/Dao";
import Apartment from "@/components/Home/Apartment";
import House from "@/components/Home/House";
import Questions from "@/components/Home/Questions";

export default {
  components: { Hero, PropertyImage, Dao, Apartment, House, Questions },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";
</style>
