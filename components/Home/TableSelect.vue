<template>
  <div class="table_select custom_container">
    <v-btn
      color="primary"
      rounded
      x-large
      class="table_select__primary black--text"
      block
      depressed
    >
      Primary Market</v-btn
    >
    <v-btn
      color="primary"
      rounded
      depressed
      x-large
      outlined
      class="table_select__secondary"
      block
    >
      Secondary Market</v-btn
    >
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.table_select {
  display: flex;
  flex-direction: column;
  margin-top: 48px;
  margin-bottom: 34px;
}

.table_select__primary .table_select__primary .table_select__primary {
  border: 1px solid #00ef8b;
  padding: 8px 16px;
  margin-bottom: 16px;
  color: red;
}

.table_select__secondary {
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 600px;
  border: 1px solid #00ef8b;
  padding: 8px 16px;
}
</style>