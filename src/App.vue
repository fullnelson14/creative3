<template>
  <div id="app">
    <AppBox>
      <router-view />
    </AppBox>
  </div>
</template>

<script>
import AppBox from "./components/AppBox.vue";

export default {
  name: "Home",
  components: { AppBox }
};
</script>


<style>
* {
  margin: 0;
  font-family: "Open Sans", sans-serif;
}
</style>
