<template>
  <v-app>
    <Header />

    <slot />

    <Footer />
  </v-app>
</template>

<script>
import Header from "@/components/Layout/Default/Header";
import Footer from "@/components/Layout/Default/Footer";

export default {
  components: {
    Header,
    Footer,
  },
};
</script>

<style lang="scss" scoped>
.debugger {
  position: relative;
}
</style>
