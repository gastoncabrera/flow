<template>
  <div class="home">

    <Hero />

    <Main />

    <RaisedMoney />

    <FeaturedProjects />
    
    <TableSelect />
  </div>
</template>

<script>
import Hero from "@/components/Home/Hero";
import Main from "@/components/Home/Main";
import RaisedMoney from "@/components/Home/RaisedMoney";
import FeaturedProjects from "@/components/Home/FeaturedProjects";
import TableSelect from "@/components/Home/TableSelect";

export default {
  components: {
    Hero,
    Main,
    RaisedMoney,
    FeaturedProjects,
    TableSelect,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";
</style>
