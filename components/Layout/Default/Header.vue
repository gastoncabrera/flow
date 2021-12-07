<template>
  <div class="header">
    <div class="header__background">
      <div class="header__container custom_container">
        <nuxt-link to="/" class="header__image_link">
          <img
            src="~/static/logo_Flow_Wordmark.svg"
            alt=""
            class="header__image"
          />
        </nuxt-link>

        <MenuIcon class="header__menu" @Click="handleClick" />

        <nav class="navbar">
          <ul class="navbar__list">
            <li class="navbar__item">
              <nuxt-link class="navbar__link" to="">Getting Started</nuxt-link>
            </li>

            <li class="navbar__item">
              <nuxt-link class="navbar__link" to="">Documentation</nuxt-link>
            </li>

            <li class="navbar__item">
              <nuxt-link class="navbar__link" to="">Flowverse</nuxt-link>
            </li>
          </ul>
        </nav>
      </div>
    </div>

    <nav
      class="menu custom_container"
      :class="menu ? 'menu__open' : 'menu__close'"
    >
      <ul class="menu__list">
        <li class="menu__item">
          <nuxt-link class="menu__link" to="">Getting Started</nuxt-link>
        </li>

        <li class="menu__item">
          <nuxt-link class="menu__link" to="">Documentation</nuxt-link>
        </li>

        <li class="menu__item">
          <nuxt-link class="menu__link" to="">Flowverse</nuxt-link>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
import MenuIcon from "@/components/MenuIcon";
export default {
  components: {
    MenuIcon,
  },
  data() {
    return {
      menu: false,
    };
  },
  methods: {
    handleClick() {
      this.menu = !this.menu;
    },
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.header__background {
  height: 100px;
  width: 100%;
  position: fixed;
  top: 0;
  background-color: white;
  z-index: 100;
}

.header__container {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-top: 24px;
  margin-bottom: 24px;
}

.header__image_link {
  max-width: 120px;
  cursor: pointer;

  @include breakpoint(lg) {
    max-width: 130px;
  }
}

.header__image {
  width: 100%;
}

.header__menu.header__menu.header__menu {
  display: flex;
  cursor: pointer;

  @include breakpoint(lg) {
    display: none;
  }
}

.navbar {
  display: none;

  @include breakpoint(lg) {
    display: flex;
  }
}

.navbar__list {
  display: flex;
  list-style: none;
  align-items: center;
  justify-content: center;
}

.navbar__item {
  margin-left: 32px;
}

.navbar__link {
  text-decoration: none;
  color: black;
  font-family: $font_2;
  font-size: 16px;
  font-weight: 700;
  letter-spacing: 1px;
}

.menu {
  position: fixed;
  transition: 300ms ease;
  left: 0;
  z-index: 2;
  background-color: white;
  border-top: 1px solid #eaeaea;

  @include breakpoint(lg) {
    display: none;
  }
}

.menu__list {
  list-style: none;
}

.menu__item {
  margin: 24px 0;
}

.menu__link {
  text-decoration: none;
  color: black;
  font-family: $font_2;
  font-size: 16px;
  font-weight: 700;
  letter-spacing: 1px;
}

.menu__open {
  top: 100px;
}

.menu__close {
  top: -70px;
}
</style>