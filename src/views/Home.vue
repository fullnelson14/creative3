<template>
  <div class="home">
    <h1>Welcome to Super RV!</h1>
    <p>Let's get you settled in.</p>
    <div class="box-container">
      <LinkBox boxTitle="Home" :imgNumber="1"></LinkBox>
      <LinkBox boxTitle="About" :imgNumber="2"></LinkBox>
      <LinkBox boxTitle="Schedule" :imgNumber="3"></LinkBox>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import LinkBox from "../components/LinkBox";

export default {
  name: "Home",
  components: { LinkBox }
};
</script>

<style scoped>
.home {
  flex: 1;
  display: flex;
  flex-direction: column;
  padding: 45px;
}
.box-container {
  padding: 20px;
  padding-left: 0;
  display: flex;
  justify-content: space-around;
}
</style>
