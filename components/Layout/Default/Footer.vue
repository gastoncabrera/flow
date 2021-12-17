<template>
  <div class="footer">
    <div class="footer__container custom_container custom_container--xxxl">
      <div class="footer__left">
        Construido por
        <span class="footer___creator">Orlando</span> y
        <span class="footer___creator">Freddy</span>
      </div>
      <div class="footer__right">© Todos los derechos reservados | 2021</div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.footer__container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 60px;
  margin-bottom: 36px;
}

.footer__left,
.footer__right {
  font-size: 16px;
  line-height: 19px;
  font-weight: 400;
}

.footer___creator {
  text-decoration: underline;
}
</style>