<template>
  <div class="house">
    <div class="house__container custom_container custom_container--xl">
      <h2 class="house__title">¿Cómo es tener una casa en tu Wallet?</h2>

      <div class="house__wrap_top">
        <div class="left">
          <div class="title">Si me gano el premio</div>
          <div class="line"></div>
          <div class="apartment__wrap">
            <div class="apartment__list">
              <ListWrap />

              <ListWrap />

              <ListWrap />
            </div>
          </div>
        </div>
        <img src="Gray.jpg" alt="" class="right" />
      </div>

      <div class="house__wrap_bottom">
        <img src="Gray.jpg" alt="" class="bottom_left" />

        <div class="bottom_right">
          <div class="bottom_title">Otros beneficios del NFT's</div>
          <div class="bottom_line"></div>
          <div class="bottom__wrap">
            <div class="bottom__list">
              <ListWrap />

              <ListWrap />

              <ListWrap />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ListWrap from "@/components/Shared/ListWrap.vue";
export default {
  components: {
    ListWrap,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.house__container {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 172px;
  margin-bottom: 109px;
}

.house__title {
  margin-bottom: 77px;
}

.house__wrap_top {
  width: 100%;
  height: 639px;
  display: flex;
  justify-content: space-between;
}

.left {
  width: 459px;
  height: 100%;
}

.title {
  margin-bottom: 16px;
  font-size: 20px;
  line-height: 24px;
  font-weight: 600;
}

.line {
  border-bottom: 1px solid #979797;
  margin-bottom: 30px;
}

.apartment__wrap {
  display: flex;
  height: 450px;
  width: 441px;
}

.apartment__list {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.right {
  width: 593px;
  height: 100%;
}

// ----------------------

.house__wrap_bottom {
  margin-top: 100px;
  width: 100%;
  height: 639px;
  display: flex;
  justify-content: space-between;
}

.bottom_left {
  width: 593px;
  height: 100%;
}

.bottom_right {
  width: 459px;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.bottom_title {
  margin-bottom: 16px;
  font-size: 20px;
  line-height: 24px;
  font-weight: 600;
}

.bottom_line {
  border-bottom: 1px solid #979797;
  margin-bottom: 30px;
}

.bottom__wrap {
  display: flex;
  height: 450px;
  width: 441px;
}

.bottom__list {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
</style>