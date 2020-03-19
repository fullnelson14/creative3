<template>
  <router-link :to="getRoute" class="nav-link">
    <div class="link-box">
      <img
        v-if="imgNumber === 1"
        id="box-image"
        src="../assets/rv1.jpg"
        alt=""
      />
      <img
        v-if="imgNumber === 2"
        id="box-image"
        src="../assets/rv2.jpg"
        alt=""
      />
      <img
        v-if="imgNumber === 3"
        id="box-image"
        src="../assets/rv3.jpg"
        alt=""
      />
      <p>{{ boxTitle }}</p>
    </div>
  </router-link>
</template>

<script>
// @ is an alias to /src

export default {
  name: "LinkBox",
  components: {},
  props: ["boxTitle", "imgNumber"],
  computed: {
    getRoute() {
      if (this.imgNumber === 2) {
        return "/about";
      } else if (this.imgNumber === 3) {
        return "/schedule";
      } else {
        return "/";
      }
    }
  }
};
</script>

<style scoped>
.link-box {
  height: 250px;
  width: 200px;
  background-color: white;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-right: 50px;
  box-shadow: -8px 9px 24px -8px rgba(0, 0, 0, 0.75);
  border-radius: 6px;
  transition-duration: 300ms;
  color: black;
}
.link-box:hover {
  transform: scale(1.03);
}
a {
  text-decoration: none;
}

#box-image {
  height: 100px;
  border-radius: 4px;
  margin: 10px;
}
</style>
