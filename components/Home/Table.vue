<template>
  <v-data-table
    :headers="headers"
    :items="desserts"
    class="elevation-1 black--text prueba"
    hide-default-footer
    mobile-breakpoint="0"
  >
    <template v-slot:item.name="{ item }">
      {{ item.img }}{{ item.name }}
    </template>
  </v-data-table>
</template>
<script>
export default {
  data() {
    return {
      headers: [
        {
          text: "PROJECT",
          value: "name",
        },
        { text: "SALES", value: "calories" },
        { text: "NFTS", value: "fat" },
      ],
      desserts: [
        {
          name: "1 Frozen Yogurt",
          img: "algo",
          calories: 159,
          fat: 6.0,
        },
        {
          name: "2 Ice cream sandwich",
          calories: 237,
          fat: 9.0,
        },
        {
          name: "3 Eclair",
          calories: 262,
          fat: 16.0,
        },
      ],
    };
  },
};
</script>
<style lang="scss">
.prueba .prueba.prueba {
  font-size: 30px;
}
</style>