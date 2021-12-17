<template>
  <div class="dao">
    <div class="dao__container custom_container custom_container--xl">
      <h2 class="dao__title">What is Title Dao</h2>

      <div class="dao__wrap">
        <div class="dao__list">
          <img src="icon-CheckList2.svg" alt="" class="dao__image" />

          <span class="dao__text">Give equity to contributors</span>
        </div>

        <div class="dao__list">
          <img src="icon-CheckList2.svg" alt="" class="dao__image" />

          <span class="dao__text">Raise funds with tokens & NFTs</span>
        </div>

        <div class="dao__list">
          <img src="icon-CheckList2.svg" alt="" class="dao__image" />

          <span class="dao__text">Make decisions together</span>
        </div>

        <div class="dao__list">
          <img src="icon-CheckList2.svg" alt="" class="dao__image" />

          <span class="dao__text">Operate globally</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.dao__container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  margin-top: 127px;
  margin-bottom: 127px;
}

.dao__title {
  font-size: 30px;
  font-weight: 400;
  line-height: 36px;
  margin-bottom: 39px;
}

.dao__list {
  display: flex;
  align-items: center;
  margin-top: 26px;
}

.dao__image {
  margin-right: 15px;
}

.dao__text {
  font-size: 18px;
  line-height: 22px;
  font-weight: 600;
}
</style>