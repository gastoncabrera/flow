<template>
  <div class="pill">
    <nuxt-link
      to=""
      class="pill__container"
      v-for="pill in pills"
      :key="pill.title"
    >
      <img class="pill__image" :src="`/pills/${pill.image}`" alt="" />
      <span class="pill__title">{{ pill.title }}</span>
    </nuxt-link>
  </div>
</template>

<script>
export default {
  props: {
    pills: {
      typeof: Array,
      require: true,
    },
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.pill {
  display: flex;
  box-sizing: border-box;
  vertical-align: middle;
  overflow: hidden;
  padding: 15px 0;
  height: 90px;
}

.pill__container {
  width: 100%;
  flex-wrap: nowrap;
  align-items: center;
  letter-spacing: 0.4px;
  display: flex;
  border: 1px solid silver;
  border-radius: 600px;
  margin-left: 16px;
  margin-right: 16px;
  padding: 12px 20px;
  white-space: nowrap;
  text-decoration: none;
  color: black;

  @include breakpoint(sm) {
    margin-right: 30px;
  }

  @include breakpoint(md) {
    padding: 21px 34px;
  }
}

.pill__image {
  height: 30px;
  margin-right: 10px;
}

.pill__title {
  font-family: $font_2;
  font-size: 16px;
  font-weight: 700;

  @include breakpoint(sm) {
    font-size: 20px;
  }

  @include breakpoint(md) {
    font-size: 24px;
  }
}
</style>