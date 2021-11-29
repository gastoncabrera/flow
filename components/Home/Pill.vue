<template>
  <div class="pill">
    <nuxt-link
      to=""
      class="pill__container"
      v-for="pill in pills"
      :key="pill.title"
    >
      <img class="pill__image" :src="pill.image" alt="" />
      <span class="pill__title">{{ pill.title }}</span>
    </nuxt-link>
  </div>
</template>

<script>
export default {
  data() {
    return {
      pills: [
        {
          image:
            "https://assets.website-files.com/6166db1bcfba82a3b0a334d6/61675ced852fd3097d1a9eac_612cadda51366e013180df35_bng.jpeg",
          title: "Biscuits n Groovy",
        },
        {
          image: "/Binance.png",
          title: "Binance",
        },
        {
          image:
            "https://assets.website-files.com/6166db1bcfba82a3b0a334d6/61675c0b09f4d7287c9d8a8c_61600d14b05ba933f6e2deef_ballerz%20logo.jpeg",
          title: "Ballerz",
        },
        {
          image:
            "https://assets.website-files.com/6166db1bcfba82a3b0a334d6/61675c619dd742f44b6d832b_60f2afc1fb0e0ba46096446b_big%20dipper.jpeg",
          title: "Big Dipper",
        },
        {
          image:
            "https://assets.website-files.com/6166db1bcfba82a3b0a334d6/61675bdad1baaae3a823c9f5_6149ccacd3bf0e0431b2a427_Screen%20Shot%202021-09-21%20at%2010.14.31%20pm.png",
          title: "Athletes Unlimited",
        },
        {
          image:
            "https://assets.website-files.com/6166db1bcfba82a3b0a334d6/61675bdad1baaae3a823c9f5_6149ccacd3bf0e0431b2a427_Screen%20Shot%202021-09-21%20at%2010.14.31%20pm.png",
          title: "Athletes Unlimited",
        },
        {
          image:
            "https://assets.website-files.com/6166db1bcfba82a3b0a334d6/61675bdad1baaae3a823c9f5_6149ccacd3bf0e0431b2a427_Screen%20Shot%202021-09-21%20at%2010.14.31%20pm.png",
          title: "Athletes Unlimited",
        },
        {
          image:
            "https://assets.website-files.com/6166db1bcfba82a3b0a334d6/61675bdad1baaae3a823c9f5_6149ccacd3bf0e0431b2a427_Screen%20Shot%202021-09-21%20at%2010.14.31%20pm.png",
          title: "Athletes Unlimited",
        },
        {
          image:
            "https://assets.website-files.com/6166db1bcfba82a3b0a334d6/61675bdad1baaae3a823c9f5_6149ccacd3bf0e0431b2a427_Screen%20Shot%202021-09-21%20at%2010.14.31%20pm.png",
          title: "Athletes Unlimited",
        },
        {
          image:
            "https://assets.website-files.com/6166db1bcfba82a3b0a334d6/61675bdad1baaae3a823c9f5_6149ccacd3bf0e0431b2a427_Screen%20Shot%202021-09-21%20at%2010.14.31%20pm.png",
          title: "Athletes Unlimited",
        },
      ],
    };
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
  align-items: center;
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