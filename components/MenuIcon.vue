<template>
  <div class="icon_menu" @click="handleClick">
    <div class="barra barra--one"></div>
    <div class="barra barra--two"></div>
    <div class="barra barra--three"></div>
  </div>
</template>

<script>
export default {
  methods: {
    handleClick() {
      this.$emit("Click");
    },
  },
};
</script>

<style lang="scss" scoped>
.icon_menu {
  width: 30px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.barra {
  margin-top: 2px;
  margin-bottom: 2px;
  height: 2px;
  width: 100%;
  background-color: black;
}

.barra--one,
.barra--three {
  width: 75%;
}
</style>