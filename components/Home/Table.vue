<template>
  <div class="custom_container">
    <v-data-table
      :headers="header"
      :items="body"
      class="table table--home"
      hide-default-footer
      mobile-breakpoint="0"
      disable-sort
      items-per-page="100"
    >
      <template v-slot:item.name="{ item }">
        <div class="table__body">
          {{ item.id }}

          <img
            :src="`~/static/pills/${item.img}`"
            alt=""
            class="table__body_image"
          />
          {{ item.name }}
        </div>
      </template>

      <template v-slot:item.sales="{ item }">
        <div class="table__body">${{ item.sales }}</div>
      </template>

      <template v-slot:item.nft="{ item }">
        <div class="table__body">
          {{ item.nft }}
        </div>
      </template>

      <template v-slot:item.change="{ item }">
        <div
          :class="item.change < 0 ? 'table__up' : 'table__down'"
          class="table__body"
        >
          {{ item.change }}%
        </div>
      </template>

      <template v-slot:item.users="{ item }">
        <div class="table__body">
          {{ item.users }}
        </div>
      </template>

      <template v-slot:item.txns="{ item }">
        <div class="table__body">
          {{ item.txns }}
        </div>
      </template>
    </v-data-table>
  </div>
</template>
<script>
export default {
  props: {
    header: {
      typeof: String,
      require: true,
    },

    body: {
      typeof: String,
      require: true,
    },
  },
};
</script>
<style lang="scss">
@import "@/assets/scss/utils";

.table--home {
  display: flex;
  align-items: center;
  margin-bottom: 50px;
  margin-top: 24px;

  .v-data-table__wrapper {
    height: 100%;
    width: 100%;
  }

  .table__body_image {
    height: 20px;
    width: 20px;
    border-radius: 50%;
    overflow: hidden;
    object-fit: cover;
    margin-left: 10px;
    margin-right: 16px;

    @include breakpoint(md) {
      height: 40px;
      width: 40px;
    }
  }

  .title.title.title {
    border-bottom: 4px solid black !important;
    font-family: $font_1;
    font-size: 20px;
    font-weight: 700;
  }

  .table__body.table__body.table__body {
    display: flex;
    align-items: center;
    font-family: $font_2;
    font-size: 15px;
    font-weight: 900;
    margin-top: 25px;
    margin-bottom: 25px;
    color: black;
  }

  .table__up.table__up.table__up {
    color: #02d87e;
  }

  .table__down.table__down.table__down {
    color: red;
  }
}
</style>