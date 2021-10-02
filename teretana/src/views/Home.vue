<template>
  <div class="home">
    <div class="home_top">
      <div class="container">
        <div class="home_top_h1">
          <h1>
            BE <strong> STRONG </strong> TRANING <br />
            HARD
          </h1>
        </div>
      </div>
    </div>
    <div class="about">
      <!-- <div class="about_h1">
        <h1>O meni</h1>
      </div> -->
      <div class="about_img">
        <img src="../assets/Untitled-1.png" alt="" />
      </div>
      <div class="about_info">
        <div class="about_info_h2">
          <h3>Informacije o meni</h3>
          <h2>Ime Prezime personaltni trener</h2>
        </div>
        <div class="about_info_text">
          <p>
            Lorem Ipsum is simply dummy text of the printing and typesetting
            industry. Lorem Ipsum has been the industry's standard dummy text
            ever since the 1500s, when an unknown printer took a galley of type
            and scrambled it to make a type specimen book.
          </p>
        </div>
        <div class="about_info_list">
          <p>
            <i class="fas fa-long-arrow-alt-right"></i>Zenski fitnes i vezbanje
          </p>
          <p>
            <i class="fas fa-long-arrow-alt-right"></i>Muski fitnes i vezbanje
          </p>
          <p><i class="fas fa-long-arrow-alt-right"></i>Personalni treninzi</p>
        </div>
      </div>
    </div>
    <div class="services_offer">
      <div class="services">
        <div class="service-1">
          <div class="service-1-title">
            <h2>Kardio</h2>
          </div>
          <div class="service-1-text">
            <p>
              Kardio trening je najefikasniji način za skidanje masnih naslaga,
              postizanje i održavanja kondicije. Kardio-vežbe su neophodne za
              svaki efikasan program treninga jer podstiču sagorevanje masnoća
              ali su ujedno dobre i za celokupno zdravlje organizma.
            </p>
          </div>
          <div class="service-button">
            <button>More info</button>
          </div>
        </div>
        <div class="service-1">
          <div class="service-1-title">
            <h2>Kardio</h2>
          </div>
          <div class="service-1-text">
            <p>
              Kardio trening je najefikasniji način za skidanje masnih naslaga,
              postizanje i održavanja kondicije. Kardio-vežbe su neophodne za
              svaki efikasan program treninga jer podstiču sagorevanje masnoća
              ali su ujedno dobre i za celokupno zdravlje organizma.
            </p>
          </div>
          <div class="service-button">
            <button>More info</button>
          </div>
        </div>
        <div class="service-1">
          <div class="service-1-title">
            <h2>Kardio</h2>
          </div>
          <div class="service-1-text">
            <p>
              Kardio trening je najefikasniji način za skidanje masnih naslaga,
              postizanje i održavanja kondicije. Kardio-vežbe su neophodne za
              svaki efikasan program treninga jer podstiču sagorevanje masnoća
              ali su ujedno dobre i za celokupno zdravlje organizma.
            </p>
          </div>
          <div class="service-button">
            <button>More info</button>
          </div>
        </div>
        <!-- <div class="service"><div class="service_plan plan_1"><h2>Skidanje <br> kilograma</h2></div></div>
        <div class="service"><div class="service_plan plan_2"><h2>Kardio <br> fitnes</h2></div></div>
        <div class="service"><div class="service_plan plan_3"><h2>Povecanje <br> misica</h2></div></div>
        <div class="service"><div class="service_plan plan_4"><h2>Nesto <br> peto</h2></div></div> -->
      </div>
    </div>
    <div class="contact">
      <div class="contact_h2"><h2>Kontakt</h2></div>
      <div class="contact_form">
        <input type="text" placeholder="Ime" />
        <input type="text" placeholder="E-mail" />
        <textarea
          name=""
          id=""
          cols="30"
          rows="10"
          placeholder="Tvoja poruka ovde..."
        ></textarea>
        <button class="contact_submit">Posalji</button>
      </div>
      <div class="contact_info">
        <div><p>Tel: 0606665445</p></div>
        <div><p>Mail: nsasdn@gmail.com</p></div>
        <div>
          <i class="fab fa-instagram"></i><i class="fab fa-facebook-square"></i>
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
  height: 500px;
  background: url(/img/360_F_320459487_SAvrvfR4NN4CkFQccj49rBfmiLoYebuw.186bfd09.jpg);
  background-size: cover;
  display: flex;
  align-content: center;
  /* padding-top: 355px; */
  /* background-position: center center; */
  background-size: 100%;
  background-repeat: no-repeat;
}
.container {
  position: relative;
  width: 100%;
  /* padding-top: 200px; */
  display: flex;
  justify-content: flex-start;
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

.about {
  display: flex;
  flex-wrap: wrap;
  padding-left: 15%;
  padding-right: 15%;
  padding-top: 5%;
  padding-bottom: 5%;
}
.about_h1 {
  width: 100%;
  text-align: start;
}
.about_h1 h1 {
  font-family: "Oswald", sans-serif;
}
.about_img {
  width: 30%;
}
.about_info {
  width: 70%;
  display: flex;
  flex-direction: column;
  text-align: left;
}
.about_info_h2 {
  font-family: "Oswald", sans-serif;
}
.about_info_h2 h3,
h2 {
  margin: 0;
}
.about_info_h2 h3 {
  color: #e63946;
}
.about_info_text {
  font-family: "Poppins", sans-serif;
}
.about_info_list p {
  font-family: "Poppins", sans-serif;
}
.about_info_list i {
  color: #e63946;
  margin-right: 5px;
}
.services_offer {
  width: 100%;
  display: flex;
  background-color: #eff2f5;
  justify-content: center;
}
.services {
  padding-top: 100px;
  padding-bottom: 100px;
  display: flex;
  width: 70%;
  /* flex-wrap: wrap; */
}
.service {
  display: flex;
  justify-content: center;
  /* margin: 5px; */
  width: 50%;
  height: 400px;
  /* background-color: red; */
  margin-bottom: 20px;
  box-sizing: border-box;
  /* padding: 5px; */
}
.service-1 {
  width: 33%;
  /* height: 300px; */
  border: 1px solid #6d6d6d;
  border-radius: 3px;
  margin: 5px;
  box-sizing: border-box;
  background-color: white;
}
.service-1-title {
  padding: 50px;
  padding-bottom: 25px;
}
.service-1-title h2 {
  font-family: "Poppins", sans-serif;
  font-size: 35px;
}
.service-1-text {
  padding: 50px;
  padding-top: 0;
}
.service-1-text p {
  font-family: "Poppins", sans-serif;
}
.service-button {
  padding: 40px;
  padding-top: 0;
}
.service-button button {
  width: 120px;
  height: 40px;
  border: none;
  background-color: #219ebc;
  border-radius: 3px;
  color: white;
  font-size: 15px;
  font-weight: 500;
  font-family: "Poppins", sans-serif;
}
.service-button button:hover {
  cursor: pointer;
}
.service_plan {
  box-sizing: border-box;
  margin: 10px;
  width: 100%;
  height: 400px;
  /* background-color: white; */
  color: rgb(250, 84, 7);
  font-family: "Oswald", sans-serif;
  font-size: 25px;
  display: flex;
  align-items: center;
  justify-items: center;
  justify-content: center;
  /* background-image: url("../assets/thumb2-training-bodybuilding-fitness-gym-sport.jpg"); */
}
.plan_1 {
  background-repeat: no-repeat;
  /* background-size: cover; */
  /* background-position: center center; */
  background-size: cover;
  background-image: url("../assets/thumb2-training-bodybuilding-fitness-gym-sport.jpg");
}

.plan_2 {
  background-size: cover;
  background-image: url("../assets/Pull_Up_Alt1-1440x900.jpg");
  /* background-size: 200%; */
  background-repeat: no-repeat;
  /* background-size: cover; */
  /* background-position: center center; */
}
.plan_3 {
  /* background-size: 200%; */
  background-repeat: no-repeat;
  /* background-size: cover; */
  /* background-position: left center; */
  background-size: cover;
  background-image: url("../assets/360_F_320459487_SAvrvfR4NN4CkFQccj49rBfmiLoYebuw.jpg");
}
.plan_4 {
  /* background-size: 200%; */
  background-repeat: no-repeat;
  /* background-size: cover; */
  /* background-position: left center; */
  background-image: url("../assets/RTQ3_06A0632.jpg");
}

.contact {
  padding-top: 50px;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.contact_h2 {
  font-family: "Oswald", sans-serif;
  padding-bottom: 50px;
}
.contact_form {
  display: flex;
  align-items: center;
  flex-direction: column;
  width: 30%;
}
.contact_form input {
  width: 70%;
  height: 25px;
  margin: 5px;
  border: 1px solid rgb(85, 85, 85);
  font-family: "Poppins";
  border-radius: 5px;
}
.contact_form textarea {
  width: 70%;
  font-family: "Poppins";
  height: 150px;
  margin: 5px;
  border: 1px solid rgb(85, 85, 85);
}
.contact_submit {
  margin-top: 10px;
  width: 30%;
  height: 30px;
  background-color: tomato;
  border: none;
  border-radius: 5px;
}
@media only screen and (max-width: 600px) {
  .home_top {
    width: 100%;
    height: 1040px;
    background: url("../assets/Slika3.jpg");
    background-size: cover;
    display: flex;
    -ms-flex-line-pack: center;
    align-content: center;
    /* padding-top: 355px; */
    background-position: bottom right;
  }
  .home_top_h1 {
    max-width: 100%;
  }
}
</style>
