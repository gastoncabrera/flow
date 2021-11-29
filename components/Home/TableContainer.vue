<template>
  <section class="table_container custom_container">
    <div class="table_container__content">
      <img src="/pm.png" alt="" class="table_container__image" />
      <p class="table_container__title">
        Powered by Flowverse.co - discoverability platform for Flow Blockchain
        projects
      </p>
    </div>
    <Table />
  </section>
</template>

<script>
import Table from "@/components/Home/Table";

export default {
  components: {
    Table,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.table_container {
  display: flex;
  flex-direction: column;
  margin-bottom: 16px;
}

.table_container__content {
  display: flex;
}

.table_container__title {
  font-family: $font_1;
  font-weight: 400;
  font-size: 10px;
  color: black;
  text-align: center;
}

.table_container__image {
  display: none;
}
</style>