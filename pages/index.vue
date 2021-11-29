<template>
  <div>
    <Hero />
    <Main />
    <!-- <Pill /> -->
    <RaisedMoney />
    <!-- <FeaturedProjects />
    <TableSelect />
    <TableContainer /> -->
  </div>
</template>

<script>
import Hero from "@/components/Home/Hero";
import Main from "@/components/Home/Main";
import Pill from "@/components/Home/Pill";
import RaisedMoney from "@/components/Home/RaisedMoney";
import FeaturedProjects from "@/components/Home/FeaturedProjects";
import TableSelect from "@/components/Home/TableSelect";
import TableContainer from "@/components/Home/TableContainer";

export default {
  components: {
    Hero,
    Main,
    Pill,
    RaisedMoney,
    FeaturedProjects,
    TableSelect,
    TableContainer,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";
</style>
