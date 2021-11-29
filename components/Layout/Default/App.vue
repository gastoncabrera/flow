<template>
  <v-app class="debugger">
    <!-- <div class="layout custom_container">
      <img src="/logo_Flow_Wordmark.svg" alt="" class="layout__image" />
      <v-icon x-large class="header__btn_menu" @click="getClick"
        >mdi-menu</v-icon
      >
    </div> -->
    <slot />
    <!-- <div class="footer">
      <div>JOIN FLOW ON</div>
      <nuxt-link to="#">TWITTER</nuxt-link>
      <nuxt-link to="#">DISCORD</nuxt-link>
      <nuxt-link to="#">ONFLOW.ORG</nuxt-link>
    </div> -->
  </v-app>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.layout {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-top: 24px;
  margin-bottom: 24px;
}

.layout__image {
  max-width: 120px;
}

.footer {
  display: flex;
  flex-direction: column;
  background-image: url("https://assets.website-files.com/5f734f4dbd95382f4fdfa0ea/616a02f7ee582ff395518473_greeVector-170%20(1).jpg");
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  height: 100%;
  width: 100%;
  text-align: center;
  padding-top: 30px;
  padding-bottom: 90px;
}
</style>
