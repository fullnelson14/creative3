<template>
  <div id="total-box">
    <div id="slanted-box"></div>
    <div id="img-container">
      <img id="desert-img" src="../assets/desert.jpg" alt="A desert landscape" />
    </div>

    <div id="container">
      <NavBox></NavBox>
      <div id="inner">
        <slot></slot>
      </div>
      <FooterBox></FooterBox>
    </div>
  </div>
</template>

<script>
import NavBox from "./NavBox";
import FooterBox from "./FooterBox";
export default {
  name: "AppBox",
  components: {
    NavBox,
    FooterBox
  }
};
</script>

<style  scoped>
#total-box {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  overflow: hidden;
}

#slanted-box {
  position: absolute;
  height: 130vh;
  width: 130%;
  transform: rotate(15deg);
  background: rgb(255, 255, 253);
  background: linear-gradient(
    153deg,
    rgba(255, 255, 253, 1) 0%,
    rgba(253, 255, 178, 1) 100%
  );
  top: 125px;
  z-index: 2;
}
#container {
  position: relative;
  z-index: 4;
  height: 100vh;
  flex: 1;
  display: flex;
  flex-direction: column;
}
#inner {
  flex: 1;
}
#img-container {
  background-color: green;
  height: 45vh;
  width: 85%;
  position: absolute;
  top: 0;
  right: 0;
  overflow: hidden;
}
#desert-img {
  width: 100%;
}
</style>