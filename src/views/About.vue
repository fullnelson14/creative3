<template>
  <div class="about">
    <h1>About Us</h1>
    <div id="about-text">
      <p>
        We are a humble husband-and-wife team that aims to provide the best RV
        park service that you've ever had. That's quite a lofty goal, but we are
        committed to making it happen.
      </p>
      <p>
        We got started back in '85 when we ourselves took our first RV trip as a
        couple. We were disappointed by the service and amenities of all of the
        parks that we stayed at, so we decided to do it better! We bought our
        land and started operation in 2002, and haven't looked back since.
      </p>
      <p>We hope you enjoy your stay</p>
      <router-link to="/" class="nav-link">Back to Home</router-link>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "About",
  components: {}
};
</script>

<style scoped>
.about {
  flex: 1;
  display: flex;
  flex-direction: column;
  padding: 45px;
}

#about-text {
  padding-top: 50px;
  width: 50%;
}
#about-text p {
  padding: 20px 0;
}
</style>
