<template>
  <div id="nav-container">
    <div id="logo">Super RV Park</div>

    <div id="links">
      <router-link to="/" class="nav-link">Home</router-link>
      <router-link to="/about" class="nav-link">About</router-link>
      <router-link to="/schedule" class="nav-link">Schedule</router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "NavBox"
};
</script>

<style  scoped>
#nav-container {
  border-radius: 3px;
  background-color: #808080b0;
  height: 50px;
  width: 450px;
  margin: 30px;
  margin-left: 50px;
  display: flex;
  align-items: center;
  justify-content: space-around;
}

.nav-link {
  display: inline-block;
  margin: 4px;
  padding: 4px;
  text-decoration: none;
  color: black;
  transition-duration: 200ms;
  border-radius: 3px;
}
.nav-link:hover {
  color: grey;
  background-color: lightgoldenrodyellow;
}
</style>