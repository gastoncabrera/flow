<template>
  <div class="header">
    <div class="header__container custom_container custom_container--xxxl">
      <div class="Header__logo">Logo</div>
      <nav class="navbar">
        <ul class="navbar__list">
          <li class="navbar__item">
            <nuxt-link to="" class="navbar__link">Qué es Title Dao</nuxt-link>
          </li>
          <li class="navbar__item">
            <nuxt-link to="" class="navbar__link">Cómo funciona</nuxt-link>
          </li>
          <li class="navbar__item">
            <nuxt-link to="" class="navbar__link">Las ganancias</nuxt-link>
          </li>
          <li class="navbar__item">
            <nuxt-link to="" class="navbar__link">FAQ</nuxt-link>
          </li>
        </ul>
      </nav>
      <v-btn>Connect wallet</v-btn>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.header__container {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-top: 30px;
}

.navbar__list {
  display: flex;
  align-items: center;
  list-style: none;
}

.navbar__item {
  margin: 0 43px;
}

.navbar__link {
  text-decoration: none;
  font-size: 16px;
  font-weight: 400;
  line-height: 19px;
  color: black;
}
</style>