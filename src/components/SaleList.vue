<template>
  <div class="sale-list">
    <SaleItem
      v-for="item in itemArr"
      :key="item.name"
      :itemData="item"
    ></SaleItem>
  </div>
</template>

<script>
// @ is an alias to /src
import data from "../utils/fakeData";
import SaleItem from "./SaleItem";

export default {
  name: "SaleList",
  data() {
    return {
      itemArr: data
    };
  },
  components: { SaleItem }
};
</script>

<style scoped>
.sale-list {
  display: flex;
  justify-content: space-around;
}
</style>
