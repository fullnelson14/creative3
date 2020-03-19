<template>
  <div class="schedule">
    <h1>Upcoming Events</h1>

    <div id="about-text">
      <p>Check out our RV's on sale!</p>
    </div>
    <SaleList></SaleList>

    <router-link to="/" class="nav-link">Back to Home</router-link>
  </div>
</template>

<script>
// @ is an alias to /src
import SaleList from "../components/SaleList";

export default {
  name: "Schedule",
  components: { SaleList }
};
</script>

<style scoped>
.schedule {
  flex: 1;
  display: flex;
  flex-direction: column;
  padding: 45px;
}
#about-text p {
  padding: 20px 0;
}
#about-text {
  padding-top: 50px;
  width: 50%;
}
</style>
