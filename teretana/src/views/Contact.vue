<template>
  <div class="about">
    <div class="about_top">
      <h1>Contact</h1>
    </div>
  </div>
</template>


<style  scoped>
.about {
  width: 100%;
}
.about_top {
  width: 100%;
  height: 250px;
  background: url("../assets/Slika.jpg");
  background-size: cover;
  padding-top: 230px;
  background-repeat: no-repeat;
    background-size: cover;
    background-position:bottom ;
    /* background-attachment: fixed; */
}
.about_top h1 {
  font-size: 60px;
  color: #ffffff;
  font-weight: 600;
  text-transform: uppercase;
  margin-bottom: 15px;
  font-family: "Oswald", sans-serif;
}

@media only screen and (max-width: 600px) {
  .about_top {
     background: url("../assets/Slika2.jpg");
     background-position:bottom right;
     background-repeat: no-repeat;
    background-size: cover;
  }
}
</style>