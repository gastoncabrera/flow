<template>
  <div class="raised_money">
    <div class="raised_money__pills">
      <Pill :pills="pills1" />
      <Pill :pills="pills2" />
      <Pill :pills="pills3" />
    </div>

    <div class="raised_money__container_money custom_container">
      <img
        class="raised_money__image_mobile"
        src="~/static/J-Balvin_media.png"
        alt=""
      />
      <img
        class="raised_money__image_desktop"
        src="~/static/j-balvin.png"
        alt=""
      />

      <div class="raised_money__million_wrapper">
        <div class="raised_money__million">
          <span class="raised_money__number">$800 </span> MILLION
        </div>
      </div>

      <div class="raised_money__description">
        RAISED ACROSS ECOSYSTEM PROJECTS
      </div>
    </div>
  </div>
</template>

<script>
import Pill from "@/components/Home/Pill";

export default {
  components: { Pill },
  data() {
    return {
      pills1: [
        {
          image: "ballerz_logo.jpeg",
          title: "Ballerz",
        },
        {
          image: "biscuit.jpeg",
          title: "Biscuits n Groovy",
        },
        {
          image: "Binance.png",
          title: "Binance",
        },
        {
          image: "big_dipper.jpeg",
          title: "Big Dipper",
        },
        {
          image: "Athletic_Unlimited.png",
          title: "Athletes Unlimited",
        },
        {
          image: "Async_art.jpeg",
          title: "Async Art",
        },
        {
          image: "Anchorage.png",
          title: "Anchorage Digital",
        },
        {
          image: "Alchemy.png",
          title: "Alchemy",
        },
        {
          image: "AMF.jpeg",
          title: "Add More Funds",
        },
        {
          image: "Blockanime.jpeg",
          title: "Blockanime",
        },
        {
          image: "Blocklete_Games.jpeg",
          title: "Blocklete",
        },
        {
          image: "Blockparty.jpeg",
          title: "Blockparty",
        },
        {
          image: "Blocto.jpeg",
          title: "Blocto",
        },
        {
          image: "BloctoBay.jpeg",
          title: "BloctoBay",
        },
        {
          image: "BloctoSwap.png",
          title: "BloctoSwap",
        },
        {
          image: "brud.jpeg",
          title: "Brud",
        },
        {
          image: "Canes_Vault.jpeg",
          title: "Canes Vault",
        },
        {
          image: "chainmonsters.png",
          title: "Chainmonsters",
        },
        {
          image: "Cheeze.jpeg",
          title: "Cheeze",
        },
        {
          image: "Chicago_Bulls.jpeg",
          title: "Chicago Bulls",
        },
        {
          image: "CoinList.jpeg",
          title: "CoinList",
        },
        {
          image: "CoinSpot.jpeg",
          title: "CoinSpot",
        },
        {
          image: "Crave_Critics.jpeg",
          title: "Crave Critics",
        },
        {
          image: "CryptoKitties.jpeg",
          title: "CryptoKitties",
        },
        {
          image: "Cryptoys.jpeg",
          title: "Cryptoys",
        },
      ],

      pills2: [
        {
          image: "Dapper.png",
          title: "Dapper",
        },
        {
          image: "Dark_Country.jpeg",
          title: "Dark Country",
        },
        {
          image: "Decentology.jpeg",
          title: "Decentology",
        },
        {
          image: "Enemy_Metal.png",
          title: "Enemy Metal",
        },
        {
          image: "Eternal.jpeg",
          title: "Eternal",
        },
        {
          image: "Evaluate.market.jpeg",
          title: "Evaluate.market",
        },
        {
          image: "Everbloom.jpeg",
          title: "Everbloom",
        },
        {
          image: "Evolution.png",
          title: "Evolution",
        },
        {
          image: "Fantastec_Swap.jpeg",
          title: "Fantastec",
        },
        {
          image: "Filecoin.png",
          title: "Filecoin",
        },
        {
          image: "Flowns.png",
          title: "Flowns",
        },
        {
          image: "Flowscan.jpeg",
          title: "Flowscan",
        },
        {
          image: "Flowty.jpeg",
          title: "Flowty",
        },
        {
          image: "Fright_Club.jpeg",
          title: "Fright Club",
        },
        {
          image: "Gaia_Marketplace.jpeg",
          title: "Gaia Marketplace",
        },
        {
          image: "Geniace.jpeg",
          title: "Geniace.jpeg",
        },
        {
          image: "GigLabs.jpeg",
          title: "GigLabs",
        },
        {
          image: "Gigr.jpeg",
          title: "Gigr",
        },
        {
          image: "Graffle.jpeg",
          title: "Graffle",
        },
        {
          image: "Hoodlums.jpeg",
          title: "Hoodlums",
        },
        {
          image: "In_RIFT.jpeg",
          title: "In|RIFT",
        },
        {
          image: "Infinite_Objects.jpeg",
          title: "Infinite Objects",
        },
        {
          image: "Jambb.png",
          title: "Jambb",
        },
        {
          image: "Klktn.jpeg",
          title: "Klktn",
        },
        {
          image: "König_Galerie.jpeg",
          title: "König Galerie",
        },
      ],

      pills3: [
        {
          image: "KOTD_x_Niftory.png",
          title: "KOTD x Niftory",
        },
        {
          image: "Kraken.jpeg",
          title: "Kraken",
        },
        {
          image: "LaLiga.jpeg",
          title: "LaLiga",
        },
        {
          image: "Lazy.com.jpeg",
          title: "Lazy.com",
        },
        {
          image: "Legaci.png",
          title: "Legaci",
        },
        {
          image: "LiveToken.jpeg",
          title: "LiveToken",
        },
        {
          image: "Matrix_World.jpeg",
          title: "Matrix World",
        },
        {
          image: "Melos.jpeg",
          title: "Melos",
        },
        {
          image: "Metagood.jpeg",
          title: "Metagood",
        },
        {
          image: "Mint.jpeg",
          title: "Mint NFT",
        },
        {
          image: "misa.art.png",
          title: "MISA.ART",
        },
        {
          image: "Moment_Nerd.png",
          title: "Moment Nerd",
        },
        {
          image: "MomentRanks.jpeg",
          title: "MomentRanks",
        },
        {
          image: "MoonPay.jpeg",
          title: "MoonPay",
        },
        {
          image: "MotoGp_Ignition.jpeg",
          title: "MotoGP™ Ignition",
        },
        {
          image: "Mugen_ARt.jpeg",
          title: "Mugen ARt",
        },
        {
          image: "Mynft.jpeg",
          title: "Mynft",
        },
        {
          image: "Nanobash.jpeg",
          title: "Nanobash",
        },
        {
          image: "NBA_GLeague_NFTs.jpeg",
          title: "NBA GLeague NFTs",
        },
        {
          image: "NBA_Top_Shot.png",
          title: "NBA Top Shot",
        },
        {
          image: "NFLxDapper_Labs.jpeg",
          title: "NFL x Dapper Labs",
        },
        {
          image: "NFT_Genius.jpeg",
          title: "NFT Genius",
        },
        {
          image: "NFT_TopExpo.jpeg",
          title: "NFT TopExpo",
        },
        {
          image: "NFTfi.jpeg",
          title: "NFTfi",
        },
        {
          image: "Nifted.jpeg",
          title: "Nifted",
        },
        {
          image: "Niftory.png",
          title: "Niftory",
        },
        {
          image: "nWayPlay.png",
          title: "nWayPlay",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.raised_money {
  position: relative;
  display: flex;
  align-items: center;
  flex-direction: column;
  background-image: url("/greeVector.jpg");
  background-position: 100% 100%;
  background-size: contain;
  padding-bottom: 74px;

  @include breakpoint(sm) {
    padding-bottom: 100px;
  }

  @include breakpoint(md) {
    padding-bottom: 200px;
  }
}

.raised_money__pills {
  width: 100%;
}

.raised_money__container_money {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-top: 30px;

  @include breakpoint(sm) {
    margin-top: 100px;
  }

  @include breakpoint(lg) {
    margin-top: 150px;
  }
}

.raised_money__image_mobile {
  width: 200px;

  @include breakpoint(sm) {
    display: none;
  }
}

.raised_money__image_desktop {
  display: none;

  @include breakpoint(sm) {
    display: block;
    position: absolute;
    right: 0;
    bottom: 0;
    height: 390px;
  }

  @include breakpoint(md) {
    height: 540px;
  }

  @include breakpoint(lg) {
    width: 302px;
    height: 732px;
    object-fit: contain;
    object-position: center;
  }
}

.raised_money__million_wrapper {
  display: flex;
  justify-content: center;
  text-align: center;
  width: 100%;
  height: 100%;
  max-width: 1144px;
  font-family: $font_2;
  font-size: 48px;
  line-height: 64px;
  font-weight: 800;
  color: white;
  background-image: linear-gradient(180deg, #16ff99, #02d87e);
  border-radius: 600px;
  padding: 24px 30px;

  @include breakpoint(sm) {
    font-size: 70px;
    line-height: 78px;
    padding: 70px 38px;
  }

  @include breakpoint(md) {
    font-size: 120px;
    line-height: 120px;
  }

  @include breakpoint(lg) {
    font-size: 150px;
    line-height: 150px;
  }
}

.raised_money__number {
  font-size: 80px;

  @include breakpoint(md) {
    font-size: 120px;
  }

  @include breakpoint(lg) {
    font-size: 160px;
  }
}

.raised_money__description {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  font-family: $font_2;
  line-height: 38px;
  font-weight: 700;
  font-size: 28px;
  color: #16ff99;
  margin-top: 24px;
  padding-left: 16px;
  padding-right: 16px;

  @include breakpoint(sm) {
    line-height: 26px;
    font-size: 25px;
  }

  @include breakpoint(lg) {
    font-size: 35px;
    margin-top: 63px;
  }
}
</style>