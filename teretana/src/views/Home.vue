<template>
  <div class="home">
    <div class="home_top">
      <div class="container">
        <div class="home_top_h1">
          <h1>BE <strong> STRONG </strong> TRANING HARD</h1>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Home",
  components: {},
};
</script>
<style scoped>
.home {
  width: 100%;
}
.home_top {
  width: 100%;
  height: 1040px;
  background: url("../assets/1_toyr_4D7HNbvnynMj5XjXw.jpeg");
  background-size: cover;
  display: flex;
  -ms-flex-line-pack: center;
  align-content: center;
  /* padding-top: 355px; */
  background-position: bottom center;
}
.container {
  width: 100%;
  padding-top: 200px;
  display: flex;
  justify-content: flex-end;
  padding-right: 10%;
  padding-left: 10%;
}
.home_top_h1 {
  max-width: 50%;
  display: flex;
  justify-content: flex-start;
  text-align: left;
}
.home_top_h1 h1 {
  font-size: 80px;
  color: #ffffff;
  font-weight: 700;
  text-transform: uppercase;
  line-height: 90px;
  margin-bottom: 42px;
  position: relative;
  top: 100px;
  font-family: "Oswald", sans-serif;
  /* opacity: 0; */
}
.home_top_h1 h1 strong {
  color: #f36100;
}
</style>
