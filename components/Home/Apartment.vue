<template>
  <div class="apartment">
    <div class="apartment__container custom_container custom_container--xl">
      <div class="apartment__left">
        <img src="Gray.jpg" alt="" class="apartment__image_left" />
      </div>

      <div class="apartment__right">
        <h2 class="apartment__title">¿Cómo ganarse un apartamento en Miami?</h2>

        <div class="apartment__wrap">
          <img src="Gray.jpg" alt="" class="apartment__image_list" />

          <div class="apartment__list">
            <ListWrap />

            <ListWrap />

            <ListWrap />
          </div>
        </div>

        <div class="apartment__button_wrap">
          <v-btn class="apartment__button">Connect wallet</v-btn>
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
.apartment {
  display: flex;
  justify-content: center;
  align-items: center;
}

.apartment__container {
  display: flex;
  justify-content: space-between;
}

.apartment__left {
  width: 424px;
  height: 783px;
}

.apartment__image_left {
  width: 100%;
  height: 100%;
}

.apartment__right {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.apartment__title {
  margin-top: 40px;
}

.apartment__wrap {
  display: flex;
  height: 450px;
  width: 441px;
}

.apartment__image_list {
  margin-top: 12px;
  width: 84px;
  height: 366px;
}

.apartment__list {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  margin-left: 31px;
}

.apartment__item {
  display: flex;
}

.apartment__background_number {
  height: 48px;
  min-width: 48px;
  border-radius: 50%;
  background-color: #d8d8d8;
  position: relative;
}

.apartment__number {
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  font-size: 18px;
  line-height: 22px;
  font-weight: 600;
}

.apartment__item_wrap {
  display: flex;
  flex-direction: column;
  margin-left: 41px;
}

.apartment__item_title {
  font-size: 23px;
  line-height: 28px;
  font-weight: 600;
  margin-bottom: 15px;
}

.apartment__item_description {
  font-size: 18px;
  line-height: 27px;
  width: 352px;
}

.apartment__button_wrap {
  display: flex;
  justify-content: center;
}

.apartment__button.apartment__button.apartment__button {
  margin-bottom: 58px;
}
</style>