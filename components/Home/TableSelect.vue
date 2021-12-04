<template>
  <div class="table_select">
    <div class="table_select__container table_select--home custom_container">
      <v-hover color="secondary" v-slot="{ hover }">
        <v-btn
          color="primary"
          rounded
          :outlined="selected !== 'primary'"
          :class="selected === 'primary' && 'black--text'"
          class="table_select__button table_select__button--primary"
          depressed
          @click="handleSelect('primary')"
        >
          Primary Market
        </v-btn>
      </v-hover>

      <v-btn
        color="primary"
        rounded
        depressed
        :outlined="selected !== 'secondary'"
        :class="selected === 'secondary' && 'black--text'"
        class="table_select__button table_select__button--secondary"
        @click="handleSelect('secondary')"
      >
        Secondary Market
      </v-btn>
    </div>

    <div class="table_container custom_container">
      <div class="table_container__content">
        <span v-show="selected === 'primary'" class="table_container__title">
          <img src="/pm.png" alt="" class="table_container__image" />
          Powered by Flowverse.co - discoverability platform for Flow Blockchain
          projects
        </span>

        <div v-show="selected === 'secondary'">
          <span class="table_container__title">
            <img
              src="/graffle_logo.png"
              alt=""
              class="table_container__image"
            />
            Powered by Graffle - read, write, and query Flow blockchain using
            any language
          </span>

          <div
            class="buttons_days__container buttons_days--home custom_container"
          >
            <v-btn
              color="primary"
              rounded
              :outlined="selectDays !== 'seven'"
              :class="selectDays === 'seven' && 'black--text'"
              class="buttons_days__select buttons_days__select--seven"
              depressed
              @click="handleSelectDay('seven')"
            >
              7 days
            </v-btn>

            <v-btn
              color="primary"
              rounded
              :outlined="selectDays !== 'thirty'"
              :class="selectDays === 'thirty' && 'black--text'"
              class="buttons_days__select buttons_days__select--thirty"
              depressed
              @click="handleSelectDay('thirty')"
            >
              30 days
            </v-btn>

            <v-btn
              color="primary"
              rounded
              :outlined="selectDays !== 'sixty'"
              :class="selectDays === 'sixty' && 'black--text'"
              class="buttons_days__select buttons_days__select--sixty"
              depressed
              @click="handleSelectDay('sixty')"
            >
              60 days
            </v-btn>
          </div>
        </div>
      </div>
    </div>

    <Table
      v-show="selected === 'primary'"
      :header="headerPrimary"
      :body="bodyPrimary"
    />

    <Table
      v-show="selected === 'secondary'"
      :header="headerSecondary"
      :body="bodySecondary"
    />
  </div>
</template>

<script>
import Table from "@/components/Home/Table";

export default {
  components: {
    Table,
  },
  data() {
    return {
      selected: "primary",
      selectDays: "seven",

      headerPrimary: [
        {
          text: "PROJECT",
          value: "name",
          class: "title black--text ",
        },

        { text: "SALES", value: "sales", class: "black--text title" },

        { text: "NFTS", value: "nft", class: "black--text title" },
      ],

      bodyPrimary: [
        {
          id: 1,
          name: "NBA Top Shot",
          img: "NBA_Top_Shot.png",
          sales: "90.0M",
          nft: "15.0M",
        },

        {
          id: 2,
          name: "Matrix World",
          img: "Matrix_World.jpeg",
          sales: "4.1M",
          nft: "5.0K",
        },

        {
          id: 3,
          name: "misa.art",
          img: "misa.art.png",
          sales: "2.3M",
          nft: "2.1K",
        },

        {
          id: 4,
          name: "Evolution",
          img: "Evolution.png",
          sales: "2.1M",
          nft: "10.6K",
        },

        {
          id: 5,
          name: "BALLERZ",
          img: "ballerz.jpeg",
          sales: "1.8M",
          nft: "8.8K",
        },

        {
          id: 6,
          name: "Chainmonsters",
          img: "chainmonsters.jpeg",
          sales: "1.4M",
          nft: "10.0K",
        },

        {
          id: 7,
          name: "nWayPlay",
          img: "nWayPlay.png",
          sales: "1.1M",
          nft: "131.2K",
        },

        {
          id: 8,
          name: "Energy Metal",
          img: "Enemy_Metal.png",
          sales: "800.0K",
          nft: "15.0K",
        },

        {
          id: 9,
          name: "RCRDSHP",
          img: "RCRDSHP.jpeg",
          sales: "636.2K",
          nft: "208.0K",
        },

        {
          id: 10,
          name: "STARLY",
          img: "starly.jpeg",
          sales: "582.1K",
          nft: "25.6K",
        },

        {
          id: 11,
          name: "Hoodlums",
          img: "Hoodlums.jpeg",
          sales: "516.9K",
          nft: "5.0K",
        },

        {
          id: 12,
          name: "RacingTime",
          img: "RacingTime.jpeg",
          sales: "384.0K",
          nft: "1.7K",
        },

        {
          id: 13,
          name: "versus",
          img: "versus.jpg",
          sales: "305.3K",
          nft: "362",
        },

        {
          id: 14,
          name: "Muger ARt",
          img: "Mugen_ARt.jpeg",
          sales: "254.9K",
          nft: "3.6K",
        },

        {
          id: 15,
          name: "Eternal",
          img: "Eternal.jpeg",
          sales: "204.2K",
          nft: "104.7K",
        },

        {
          id: 16,
          name: "MotoGP™ Ignition",
          img: "MotoGp_Ignition.jpeg",
          sales: "176.9K",
          nft: "51.4K",
        },

        {
          id: 17,
          name: "Vault by CNN",
          img: "cnn.png",
          sales: "160.5K",
          nft: "3.6K",
        },

        {
          id: 18,
          name: "OVO NFT platform",
          img: "ovo.jpeg",
          sales: "158.3K",
          nft: "1.3K",
        },

        {
          id: 19,
          name: "THiNG.FUND",
          img: "thingfund.png",
          sales: "138.2K",
          nft: "1.9K",
        },

        {
          id: 20,
          name: "Canes Vault",
          img: "Canes_Vault.jpeg",
          sales: "101.1K",
          nft: "1.7K",
        },

        {
          id: 21,
          name: "Tical Universe",
          img: "tical.jpeg",
          sales: "86.7K",
          nft: "602",
        },

        {
          id: 22,
          name: "Mynft",
          img: "Mynft.jpeg",
          sales: "65.2K",
          nft: "902",
        },

        {
          id: 23,
          name: "RareRooms",
          img: "RareRooms.png",
          sales: "54.6K",
          nft: "613",
        },

        {
          id: 24,
          name: "Flowns",
          img: "Flowns.png",
          sales: "40.4K",
          nft: "30.5K",
        },

        {
          id: 25,
          name: "Klktn",
          img: "Klktn.jpeg",
          sales: "39.1K",
          nft: "894",
        },

        {
          id: 26,
          name: "Basic Beasts",
          img: "basicbeast.png",
          sales: "35.7K",
          nft: "317",
        },

        {
          id: 27,
          name: "xtingles",
          img: "xtingles.jpeg",
          sales: "27.8K",
          nft: "809",
        },

        {
          id: 28,
          name: "Raceday NFT",
          img: "RACEDAY.jpeg",
          sales: "25.1K",
          nft: "31.7K",
        },

        {
          id: 29,
          name: "The Next Cartel",
          img: "nextCartel.png",
          sales: "5.6K",
          nft: "36",
        },
      ],

      headerSecondary: [
        {
          text: "PROJECT",
          value: "name",
          class: "title black--text ",
        },

        { text: "SALES", value: "sales", class: "black--text title" },

        { text: "CHANGE", value: "change", class: "black--text title" },

        { text: "USERS", value: "users", class: "black--text title" },

        { text: "TXNS", value: "txns", class: "black--text title" },
      ],

      bodySecondary: [
        {
          id: 1,
          name: "NBA Top Shot",
          img: "NBA_Top_Shot.png",
          sales: "5,225,727",
          change: -21,
          users: "77,952",
          txns: "406,357",
        },

        {
          id: 2,
          name: "Chain Monsters",
          img: "chainmonsters.jpeg",
          sales: "32,608",
          change: 0,
          users: "415",
          txns: "566",
        },

        {
          id: 3,
          name: "Olympic Pins",
          img: "nWayPlay.png",
          sales: "17,628",
          change: -48,
          users: "260",
          txns: "522",
        },

        {
          id: 4,
          name: "Eternal",
          img: "Eternal.jpeg",
          sales: "5,595",
          change: -73,
          users: "288",
          txns: "910",
        },

        {
          id: 5,
          name: "Starly",
          img: "starly.jpeg",
          sales: "4,678",
          change: -32,
          users: "301",
          txns: "292",
        },

        {
          id: 6,
          name: "CNN",
          img: "cnn.png",
          sales: "3,839",
          change: -46,
          users: "15",
          txns: "12",
        },

        {
          id: 7,
          name: "Dark Country",
          img: "Dark_Country.jpeg",
          sales: "1,097",
          change: 1180,
          users: "14",
          txns: "20",
        },

        {
          id: 8,
          name: "Versus",
          img: "versus.jpg",
          sales: "1,026",
          change: -79,
          users: "2",
          txns: "1",
        },

        {
          id: 9,
          name: "MotoGP",
          img: "MotoGp_Ignition.jpeg",
          sales: "673",
          change: -9,
          users: "30",
          txns: "26",
        },

        {
          id: 10,
          name: "Evolution",
          img: "Evolution.png",
          sales: "386",
          change: -91,
          users: "9",
          txns: "6",
        },

        {
          id: 11,
          name: "Canes",
          img: "Canes_Vault.jpeg",
          sales: "87",
          change: 0,
          users: "2",
          txns: "1",
        },

        {
          id: 12,
          name: "xtingles",
          img: "xtingles.jpeg",
          sales: "1",
          change: 84,
          users: "4",
          txns: "4",
        },
      ],
    };
  },
  methods: {
    handleSelect(selected) {
      this.selected = selected;
    },
    handleSelectDay(day) {
      this.selectDays = day;
    },
  },
};
</script>

<style lang="scss">
@import "@/assets/scss/utils";

.table_select--home {
  @include breakpoint(md) {
    display: flex;
    justify-content: center;
    align-items: center;
    padding-top: 50px;
  }

  @include breakpoint(lg) {
    padding-top: 100px;
  }

  @include breakpoint(xl) {
    padding-top: 170px;
  }

  @include breakpoint(xxl) {
    padding-top: 190px;
  }

  .v-btn:hover {
    background-color: #00ef8b;
  }

  .v-btn:hover .v-btn__content {
    color: black;
  }

  .v-btn:not(.v-btn--round).v-size--default {
    padding: 24px 40px;
  }

  .table_select {
    margin-bottom: 34px;

    @include breakpoint(md) {
      width: 100%;
      display: flex;
      flex-direction: row;
      justify-content: center;
      align-items: center;
      margin: 0 auto;
      padding-top: 100px;
    }

    @include breakpoint(lg) {
      padding-top: 250px;
    }
  }

  .table_select__button {
    width: 100%;
    border: 1px solid #00ef8b;
    margin-bottom: 16px;
    text-transform: capitalize;
    font-family: $font_2;
    font-size: 16px;
    font-weight: bold;

    @include breakpoint(md) {
      width: auto;
    }
  }

  .table_select__button--primary {
    @include breakpoint(md) {
      margin-right: 12px;
    }
  }

  .table_select__button--secondary {
    @include breakpoint(md) {
      margin-left: 12px;
    }
  }
}

.buttons_days--home {
  .buttons_days__select {
    margin: 0 16px;
    width: 100%;
    border: 1px solid #00ef8b;
    margin-bottom: 16px;
    text-transform: capitalize;
    font-family: $font_2;
    font-size: 16px;
    font-weight: 900;

    @include breakpoint(md) {
      width: auto;
    }
  }

  .v-btn:hover {
    background-color: #00ef8b;
  }

  .v-btn:hover .v-btn__content {
    color: black;
  }

  .v-btn:not(.v-btn--round).v-size--default {
    padding: 24px 40px;
  }
}
</style>
<style lang="scss" scoped>
@import "@/assets/scss/utils";

.table_container {
  display: flex;
  flex-direction: column;
  margin-bottom: 16px;
}

.table_container__content {
  display: flex;
  justify-content: center;
  text-align: center;
}

.table_container__title {
  display: flex;
  align-items: flex-start;
  font-family: $font_1;
  font-weight: 400;
  font-size: 10px;
  color: black;

  @include breakpoint(sm) {
    font-size: 14px;
  }
}

.buttons_days__container {
  display: flex;
  flex-direction: row;
  margin-top: 30px;
}

.table_container__image {
  display: none;

  @include breakpoint(md) {
    display: block;
    margin-right: 8px;
    width: 20px;
    height: 20px;
  }
}
</style>