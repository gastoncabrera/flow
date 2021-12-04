<template>
  <div class="footer">
    <div class="footer__title">JOIN FLOW ON</div>

    <nav class="footer_nav">
      <ul class="footer_nav__list">
        <li class="footer_nav__item">
          <nuxt-link class="footer_nav__link" to="">TWITTER</nuxt-link>
        </li>

        <li class="footer_nav__item">
          <nuxt-link class="footer_nav__link" to="">DISCORD</nuxt-link>
        </li>

        <li class="footer_nav__item">
          <nuxt-link class="footer_nav__link" to="">ONFLOW.ORG</nuxt-link>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.footer {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100%;
  width: 100%;
  text-align: center;
  padding-top: 30px;
  padding-bottom: 90px;
  font-family: $font_2;
  font-size: 30px;
  font-weight: bold;

  @include breakpoint(sm) {
    background-image: url("https://assets.website-files.com/5f734f4dbd95382f4fdfa0ea/616a02f7ee582ff395518473_greeVector-170%20(1).jpg");
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    line-height: 35px;
  }

  @include breakpoint(md) {
    font-size: 48px;
    line-height: 55px;
  }

  @include breakpoint(lg) {
    font-size: 68px;
    line-height: 78px;
  }
}

.footer__title {
  font-size: 18px;

  @include breakpoint(md) {
    font-size: 38px;
  }

  @include breakpoint(lg) {
    font-size: 46px;
  }
}

.footer_nav__list {
  list-style: none;
  padding: 0;
}

.footer_nav__link {
  text-decoration: none;
  color: black;
  transition: all 300ms ease;

  &:hover {
    color: #00ef8b;
    text-decoration: underline;
  }
}
</style>