<template>
  <div class="sale-item">
    <div class="info">
      <p>Name of RV: {{ itemData.name }}</p>
      <p>Manufactured Year: {{ itemData.year }}</p>
      <p>RV Color: {{ itemData.color }}</p>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "SaleItem",
  components: {},
  props: ["itemData"]
};
</script>

<style scoped>
.sale-item {
  background-color: #fffe93;
  padding: 30px;
  border-radius: 4px;
}
.info {
  padding-left: 100px;
}
</style>
