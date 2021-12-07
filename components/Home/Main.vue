<template>
  <div class="main custom_container">
    <CardHero
      background="url(~/static/card/Frame_1.png)"
      title="2.6 MILLION"
      subtitle="Total Wallet Accounts"
      class="main__one"
    />
    <CardHero
      background="url(~/static/card/Frame_2.png)"
      title="175,000"
      subtitle="Monthly Active Users"
      class="main__two"
    />
    <CardHero
      background="url(~/static/card/Frame_3.png)"
      title="5,000+"
      subtitle="Developers Building on Flow"
      class="main__three"
    />
    <CardHero
      background="url(~/static/card/Frame_4.png)"
      title="675+"
      subtitle="Active Projects"
      class="main__four"
    />
    <CardHero
      background="url(~/static/card/Frame_5.png)"
      title="350+"
      subtitle="Network Nodes"
      class="main__five"
    />
  </div>
</template>

<script>
import CardHero from "@/components/Home/CardHero";
export default {
  components: {
    CardHero,
  },
  data() {
    return {
      cards: [
        {
          title: "2.6 MILLION",
          subtitle: "Total Wallet Accounts",
          img: "url(~/static/card/Frame_1.png)",
        },

        {
          title: "175,000",
          subtitle: "Monthly Active Users",
          img: "url(~/static/card/Frame_2.png)",
        },

        {
          title: "5,000+",
          subtitle: "Developers Building on Flow",
          img: "url(~/static/card/Frame_3.png)",
        },

        {
          title: "675+",
          subtitle: "Active Projects",
          img: "url(~/static/card/Frame_4.png)",
        },

        {
          title: "350+",
          subtitle: "Network Nodes",
          img: "url(~/static/card/Frame_5.png)",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.main {
  margin-top: 50px;
  margin-bottom: 50px;

  @include breakpoint(md) {
    display: grid;
    grid-template-columns: repeat(6, 1fr);
    grid-template-rows: repeat(2, 1fr);
    grid-template-areas:
      "card__one card__one card__one card__two card__two card__two"
      "card__three card__three card__four card__four card__five card__five";
    row-gap: 20px;
    column-gap: 20px;
    margin-top: 74px;
    margin-bottom: 74px;
  }

  @include breakpoint(lg) {
    row-gap: 32px;
    column-gap: 32px;
  }
}

.main__one {
  grid-area: card__one;
}

.main__two {
  grid-area: card__two;
}

.main__three {
  grid-area: card__three;
}

.main__four {
  grid-area: card__four;
}

.main__five {
  grid-area: card__five;
}
</style>
